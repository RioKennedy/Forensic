```
D:\Forensic\G140A006\VolatilityWorkbench>.\vol.exe -f .\OtterCTF.vmem windows.statistics.Statistics
Volatility 3 Framework 2.5.0
Progress:  100.00               PDB scanning finished
Valid pages (all)       Valid pages (large)     Swapped Pages (all)     Swapped Pages (large)   Invalid Pages (all)   Invalid Pages (large)   Other Invalid Pages (all)
Progress:  6553696.48           Reading memory
0       0       0       0       18484   18484   1
```


# windows.statistics.Statistics 分析

## 1. 執行指令

```bash
.\vol.exe -f .\OtterCTF.vmem windows.statistics.Statistics
```

---

## 2. Plugin 功能說明

`windows.statistics.Statistics` 是 Volatility 3 中用來檢查記憶體映像檔頁面狀態的 Plugin。

它主要用來統計記憶體中的 Page 狀態，例如：

* 有效記憶體頁面
* Large Page 數量
* Swapped Page 數量
* Invalid Page 數量
* 其他無效頁面數量

這個 Plugin 不會直接找出惡意程式或可疑行程，而是用來輔助判斷記憶體映像檔的完整性與可解析狀態。

---

## 3. 執行結果

```text
Valid pages (all)       Valid pages (large)     Swapped Pages (all)     Swapped Pages (large)   Invalid Pages (all)   Invalid Pages (large)   Other Invalid Pages (all)
0                       0                       0                       0                       18484                 18484                   1
```

---

## 4. 結果整理

| 欄位                        |    數值 | 說明                   |
| ------------------------- | ----: | -------------------- |
| Valid pages (all)         |     0 | 所有有效記憶體頁面數量          |
| Valid pages (large)       |     0 | 有效 Large Page 數量     |
| Swapped Pages (all)       |     0 | 被交換到磁碟的記憶體頁面數量       |
| Swapped Pages (large)     |     0 | 被交換出去的 Large Page 數量 |
| Invalid Pages (all)       | 18484 | 無效或無法解析的記憶體頁面數量      |
| Invalid Pages (large)     | 18484 | 無效 Large Page 數量     |
| Other Invalid Pages (all) |     1 | 其他類型的無效頁面數量          |

---

## 5. 重要欄位分析

### 5.1 Valid pages

```text
Valid pages (all) = 0
Valid pages (large) = 0
```

`Valid pages` 代表 Volatility 能夠成功判斷並解析的有效記憶體頁面。

本次結果中，Valid Pages 為 0，代表此 Plugin 在頁面統計時沒有列出有效頁面。

不過，這不代表 `OtterCTF.vmem` 無法分析，因為前面的 `windows.info.Info` 已經成功取得系統資訊，例如 Kernel Base、DTB、Symbol、Windows 版本與系統時間。因此，這裡的 `Valid pages = 0` 比較適合視為此 Plugin 對該記憶體映像檔的統計結果，而不是判斷檔案損壞的唯一依據。

---

### 5.2 Swapped Pages

```text
Swapped Pages (all) = 0
Swapped Pages (large) = 0
```

`Swapped Pages` 代表被交換到磁碟的記憶體頁面。

本次結果顯示 Swapped Pages 為 0，代表 Volatility 沒有在此記憶體映像檔中統計到 Swap Page。

這表示目前的分析結果沒有額外顯示記憶體頁面被交換到磁碟的情況。

---

### 5.3 Invalid Pages

```text
Invalid Pages (all) = 18484
Invalid Pages (large) = 18484
```

`Invalid Pages` 代表 Volatility 無法正常解析、無法轉換，或被判定為無效的記憶體頁面。

本次結果中，Invalid Pages 為 18484，而且 Invalid Large Pages 也是 18484，代表這些無效頁面主要集中在 Large Page。

這是本次結果中最重要的地方。

可能原因包含：

1. 記憶體映像檔是 `.vmem` 格式，部分頁面結構不一定能被此 Plugin 完整統計。
2. 記憶體擷取時可能沒有保存所有頁面資料。
3. 部分 Large Page 在解析時被 Volatility 判斷為 invalid。
4. 此 Plugin 的統計方式可能不適合單獨用來判斷整份記憶體檔案是否損壞。

---

### 5.4 Other Invalid Pages

```text
Other Invalid Pages (all) = 1
```

`Other Invalid Pages` 代表其他類型的無效頁面。

本次結果為 1，數量非常少，因此不是本次分析的主要重點。

---

## 6. 鑑識重點分析

本次 `windows.statistics.Statistics` 的重點不是找出攻擊行為，而是觀察記憶體映像檔的頁面狀態。

從結果來看，最需要注意的是：

```text
Invalid Pages (all) = 18484
Invalid Pages (large) = 18484
```

這代表 Volatility 在統計時發現大量無效 Large Page。

但是，這個結果不能單獨判斷記憶體檔案損壞，原因是：

* `windows.info.Info` 已經成功解析系統資訊
* Symbol 已成功載入
* Kernel Base 與 DTB 已成功辨識
* 後續其他 Plugin 仍然可以繼續執行

因此，本次結果應該解讀為：

> 此記憶體映像檔在頁面統計上存在大量 invalid page，但整體仍可被 Volatility 解析，後續分析不應停止。

---

## 7. 本次結果判斷

根據執行結果，可以得到以下判斷：

| 項目                 | 判斷                              |
| ------------------ | ------------------------------- |
| 記憶體檔案是否能分析         | 可以，因為 `windows.info.Info` 已成功解析 |
| Valid Pages 是否正常   | 此 Plugin 顯示為 0，需注意              |
| Invalid Pages 是否偏高 | 是，數量為 18484                     |
| 是否代表檔案損壞           | 不能直接這樣判斷                        |
| 是否影響後續分析           | 不一定，仍可繼續執行其他 Plugin             |
| 鑑識價值               | 作為記憶體頁面狀態與完整性參考                 |

---

## 8. 後續建議分析

由於 `windows.statistics.Statistics` 只能提供記憶體頁面統計，無法直接確認可疑行為，因此後續應繼續執行以下 Plugin：

```bash
.\vol.exe -f .\OtterCTF.vmem windows.pslist.PsList
.\vol.exe -f .\OtterCTF.vmem windows.pstree.PsTree
.\vol.exe -f .\OtterCTF.vmem windows.psscan.PsScan
.\vol.exe -f .\OtterCTF.vmem windows.cmdline.CmdLine
.\vol.exe -f .\OtterCTF.vmem windows.netscan.NetScan
```

建議下一步優先執行：

```bash
.\vol.exe -f .\OtterCTF.vmem windows.pslist.PsList
```

原因是 `pslist` 可以列出系統中的行程，是 Windows 記憶體鑑識中最基本、也是最重要的分析步驟之一。

---

## 9. 報告用結論

本次使用 Volatility 3 的 `windows.statistics.Statistics` Plugin 針對 `OtterCTF.vmem` 進行記憶體頁面統計分析。

分析結果顯示，Valid Pages 與 Swapped Pages 皆為 0，而 Invalid Pages 數量為 18484，且 Invalid Large Pages 同樣為 18484。此結果代表 Volatility 在此 Plugin 的統計過程中，將大量 Large Page 判定為無效或無法完整解析。

然而，前一步 `windows.info.Info` 已經成功解析出 Kernel Base、DTB、Symbol、Windows 版本與系統時間，因此不能單純根據 `statistics` 的結果判斷記憶體映像檔損壞。

綜合判斷，本次 `windows.statistics.Statistics` 的結果可作為記憶體頁面狀態與完整性的輔助參考，但不屬於直接判斷惡意程式或攻擊行為的 Plugin。後續仍應繼續進行行程、網路連線、命令列與惡意程式注入相關分析。

---

## 10. 簡短結論

`windows.statistics.Statistics` 顯示本次記憶體映像檔中存在大量 Invalid Pages，主要集中在 Large Page。

不過，由於 `windows.info.Info` 已成功解析系統基本資訊，因此 `OtterCTF.vmem` 仍可繼續分析。

此結果的重點是提醒分析人員：記憶體頁面統計存在異常，但不能直接視為檔案損壞或攻擊證據。後續應繼續使用 `pslist`、`pstree`、`cmdline`、`netscan` 與 `malfind` 等 Plugin 進一步調查。
