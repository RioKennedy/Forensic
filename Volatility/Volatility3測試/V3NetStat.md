# 測試內容
- vol.exe -f .\OtterCTF.vmem windows.netstat.NetStat

```
D:\Forensic\G140A006\VolatilityWorkbench>.\vol.exe -f .\OtterCTF.vmem windows.netstat.NetStat
Volatility 3 Framework 2.5.0
Progress:  100.00               PDB scanning finished
Offset  Proto   LocalAddr       LocalPort       ForeignAddr     ForeignPort     State   PID     Owner    Created


Volatility was unable to read a requested page:
Page error 0x0 in layer layer_name (Page Fault at entry 0x0 in page entry)

        * Memory smear during acquisition (try re-acquiring if possible)
        * An intentionally invalid page lookup (operating system protection)
        * A bug in the plugin/volatility3 (re-run with -vvv and file a bug)

No further results will be produced
```

# windows.netstat.NetStat 分析

## 1. Plugin 功能說明

`windows.netstat.NetStat` 用來列出系統中的網路連線資訊，功能類似 Windows 內建的 `netstat` 指令。

此 Plugin 可以查看：

* TCP / UDP 連線
* 本機 IP 與 Port
* 遠端 IP 與 Port
* 連線狀態
* 對應的 PID 與 Process
* 連線建立時間

`NetStat` 主要用來分析系統當時有哪些網路連線，以及哪些 Process 正在進行網路活動。

---

## 2. Plugin 欄位說明

| 欄位            | 說明                                       |
| ------------- | ---------------------------------------- |
| `Offset`      | 網路連線物件在記憶體中的位置                           |
| `Proto`       | 通訊協定，例如 TCPv4、UDPv4、TCPv6                |
| `LocalAddr`   | 本機 IP 位址                                 |
| `LocalPort`   | 本機 Port                                  |
| `ForeignAddr` | 遠端 IP 位址                                 |
| `ForeignPort` | 遠端 Port                                  |
| `State`       | TCP 連線狀態，例如 LISTENING、CLOSED、ESTABLISHED |
| `PID`         | 對應的 Process ID                           |
| `Owner`       | 對應的 Process 名稱                           |
| `Created`     | 連線建立時間                                   |

---

## 3. 執行指令

本次執行指令如下：

```bash
.\vol.exe -f .\OtterCTF.vmem windows.netstat.NetStat
```

---

## 4. 執行結果

執行後 Plugin 有顯示欄位名稱：

```text
Offset  Proto   LocalAddr   LocalPort   ForeignAddr   ForeignPort   State   PID   Owner   Created
```

但後續出現錯誤：

```text
Volatility was unable to read a requested page:
Page error 0x0 in layer layer_name (Page Fault at entry 0x0 in page entry)

        * Memory smear during acquisition (try re-acquiring if possible)
        * An intentionally invalid page lookup (operating system protection)
        * A bug in the plugin/volatility3 (re-run with -vvv and file a bug)

No further results will be produced
```

---

## 5. 錯誤分析

本次 `NetStat` 無法成功產生結果，原因是 Volatility 在讀取記憶體頁面時發生錯誤。

錯誤重點為：

```text
Page error 0x0
No further results will be produced
```

可能原因包含：

| 可能原因                | 說明                             |
| ------------------- | ------------------------------ |
| Memory smear        | 記憶體擷取過程中資料狀態不一致                |
| Invalid page lookup | Plugin 嘗試讀取無效的記憶體頁面            |
| Plugin 問題           | Volatility 3 Plugin 在解析此映像檔時失敗 |

此錯誤不一定代表記憶體映像檔損毀，也不一定代表惡意行為。
它只表示本次 `NetStat` Plugin 無法順利解析網路連線資料。

---

## 6. 與 NetScan 的比較

本次 `NetStat` 執行失敗，但前面已成功執行：

```bash
.\vol.exe -f .\OtterCTF.vmem windows.netscan.NetScan
```

`NetScan` 是透過掃描記憶體中的網路連線結構來取得結果，通常比 `NetStat` 更適合記憶體鑑識分析。

簡單比較如下：

| Plugin                    | 分析方式                | 本次結果   |
| ------------------------- | ------------------- | ------ |
| `windows.netstat.NetStat` | 類似系統 netstat，列出網路連線 | 執行失敗   |
| `windows.netscan.NetScan` | 掃描記憶體中的網路連線結構       | 成功取得結果 |

因此，本次網路分析以 `NetScan` 結果作為主要依據。

---

## 7. 鑑識判斷

由於 `NetStat` 執行時發生 Page Error，無法取得完整網路連線結果，因此本 Plugin 不作為主要證據來源。

不過，`NetScan` 已成功顯示系統中的網路活動，包括：

```text
BitTorrent.exe 大量 P2P 連線
WebCompanion 相關 Process 的 HTTP 連線
LunarMS.exe 的對外連線紀錄
Windows 系統服務的正常監聽 Port
```

因此，本案的網路連線分析仍可透過 `NetScan` 完成。

---

## 8. 結論

本次執行 `windows.netstat.NetStat` 時發生 Page Error，導致 Plugin 無法繼續產生結果。

此錯誤可能與記憶體擷取狀態、無效記憶體頁面或 Plugin 解析問題有關，不能直接判斷為惡意行為。

由於 `windows.netscan.NetScan` 已成功取得網路連線資料，因此本次網路分析改以 `NetScan` 為主要依據。

結論如下：

```text
NetStat 執行失敗，未產生可用結果。
NetScan 執行成功，可作為本案網路連線分析依據。
本案網路重點仍為 BitTorrent.exe 的大量 P2P 連線，以及可疑檔案可能來自 Torrent 下載活動。
```
