# 測試內容

- vol.exe -f .\OtterCTF.vmem windows.register.hivescan.HiveScan
```
D:\Forensic\G140A006\VolatilityWorkbench>.\vol.exe -f .\OtterCTF.vmem windows.registry.hivescan.HiveScan
Volatility 3 Framework 2.5.0
Progress:  100.00               PDB scanning finished
Offset

0x2d49b94
0x9aaa66e
0xb92b010
0xdb41410
0x1da8455b
0x1da84573
0x1da84593
0x1da8460e
0x206db410
0x211eb010
0x214e1010
0x24912010
0x29cb4410
0x2a958410
0x2a983010
0x2d4c1010
0x2d50c010
0x2d5bb320
0x624162d0
0x76396ca7
0x76396cf6
```


# windows.registry.hivescan.HiveScan 分析

## 1. Plugin 功能說明

`windows.registry.hivescan.HiveScan` 用來掃描記憶體中可能存在的 Windows Registry Hive 結構。

Registry Hive 是 Windows 登錄檔的重要資料庫，可能包含系統設定、使用者設定、服務設定、帳號資訊與使用者操作紀錄。

`HiveScan` 主要用於尋找記憶體中的 Hive 結構位置，尤其在某些 Hive 沒有被正常列出，或需要補充確認 Registry Hive 是否仍存在於記憶體中時，可以使用此 Plugin。

---

## 2. 執行指令

```bash
.\vol.exe -f .\OtterCTF.vmem windows.registry.hivescan.HiveScan
```

---

## 3. 欄位說明

| 欄位       | 說明                                                                 |
| -------- | ------------------------------------------------------------------ |
| `Offset` | 掃描到的 Registry Hive 結構在記憶體中的位置。此欄位只代表可能的 Hive 位址，不會直接顯示 Hive 路徑或名稱。 |

---

## 4. 執行結果

本次 `HiveScan` 掃描到多個 Registry Hive 結構 Offset：

```text
0x2d49b94
0x9aaa66e
0xb92b010
0xdb41410
0x1da8455b
0x1da84573
0x1da84593
0x1da8460e
0x206db410
0x211eb010
0x214e1010
0x24912010
0x29cb4410
0x2a958410
0x2a983010
0x2d4c1010
0x2d50c010
0x2d5bb320
0x624162d0
0x76396ca7
0x76396cf6
```

---

## 5. 分析結果

`HiveScan` 成功掃描到多個可能的 Registry Hive 結構位置。

不過，`HiveScan` 的結果只顯示 Offset，沒有顯示 Registry Hive 的完整路徑，因此單獨使用時不容易判斷每一個 Offset 對應到哪一個 Hive。

因此，本案應搭配前面的 `HiveList` 結果一起判斷。

前面 `HiveList` 已確認系統中存在以下重要 Hive：

```text
\REGISTRY\MACHINE\SYSTEM
\SystemRoot\System32\Config\SOFTWARE
\SystemRoot\System32\Config\SAM
\??\C:\Users\Rick\ntuser.dat
\??\C:\Users\Rick\AppData\Local\Microsoft\Windows\UsrClass.dat
```

其中最重要的是 Rick 使用者相關 Hive：

```text
\??\C:\Users\Rick\ntuser.dat
\??\C:\Users\Rick\AppData\Local\Microsoft\Windows\UsrClass.dat
```

這些 Hive 可作為後續分析 Rick 使用者操作紀錄的基礎。

---

## 6. HiveScan 與 HiveList 比較

| Plugin     | 主要用途                       | 結果內容                | 本案用途                   |
| ---------- | -------------------------- | ------------------- | ---------------------- |
| `HiveScan` | 掃描記憶體中可能的 Registry Hive 結構 | 只顯示 Offset          | 輔助確認記憶體中存在 Hive 結構     |
| `HiveList` | 列出已載入的 Registry Hive       | 顯示 Offset 與 Hive 路徑 | 主要用來確認重要 Registry Hive |

---

## 7. 鑑識判斷

本次 `HiveScan` 結果顯示記憶體中存在多個 Registry Hive 結構，代表系統 Registry 資料仍可被 Volatility 掃描到。

不過，由於 `HiveScan` 沒有直接顯示 Hive 路徑，因此本案主要採用 `HiveList` 的結果作為 Registry Hive 判斷依據。

`HiveScan` 可作為輔助證據，確認記憶體中確實存在多個 Registry Hive 結構。
