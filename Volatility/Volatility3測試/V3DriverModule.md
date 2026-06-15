# 測試內容
- .\vol.exe -f .\OtterCTF.vmem windows.drivermodule.DriverModule

```
D:\Forensic\G140A006\VolatilityWorkbench>.\vol.exe -f .\OtterCTF.vmem windows.drivermodule.DriverModule
Volatility 3 Framework 2.5.0
Progress:  100.00               PDB scanning finished
Offset  Known Exception Driver Name     Service Key     Alternative Name

0x5dfe060       False   N/A             \FileSystem\RAW
0x12ab0301      False   N/A     N/A     N/A
0x7ac546dc      False   N/A     N/A     N/A
```

# windows.drivermodule.DriverModule 分析

## 1. Plugin 功能說明

`windows.drivermodule.DriverModule` 用來比對 Windows Kernel 中的 Driver Object 與已載入的 Kernel Module。

此 Plugin 可用來檢查 Driver Object 是否能對應到正常載入的 Driver Module。

在 Rootkit 或惡意 Driver 分析中，如果出現 Driver Object 無法對應正常 Module，可能代表：

```text
隱藏 Driver
被卸載但仍殘留的 Driver Object
可疑 Kernel Object
Driver Module 對應異常
```

因此，`DriverModule` 可作為 Kernel Rootkit 或 Driver 隱藏行為的輔助檢查。

---

## 2. 執行指令

```bash
.\vol.exe -f .\OtterCTF.vmem windows.drivermodule.DriverModule
```

---

## 3. 欄位說明

| 欄位                 | 說明                       |
| ------------------ | ------------------------ |
| `Offset`           | Driver Object 在記憶體中的位置   |
| `Known`            | 是否為已知或可對應的 Driver Module |
| `Exception`        | 是否出現例外狀況                 |
| `Driver Name`      | Driver Object 名稱         |
| `Service Key`      | 對應的服務登錄機碼                |
| `Alternative Name` | 其他可辨識名稱                  |

---

## 4. 執行結果

本次結果如下：

```text
Offset      Known   Exception   Driver Name       Service Key     Alternative Name
0x5dfe060   False   N/A         \FileSystem\RAW
0x12ab0301  False   N/A         N/A               N/A             N/A
0x7ac546dc  False   N/A         N/A               N/A             N/A
```

---

## 5. 結果分析

### 5.1 `\FileSystem\RAW`

結果中出現：

```text
\FileSystem\RAW
```

這是 Windows 用來處理 RAW 檔案系統的正常 File System Driver Object。

雖然 `Known` 顯示為 `False`，但 `\FileSystem\RAW` 本身不屬於明顯惡意名稱，且前面的 `Modules`、`ModScan`、`SSDT`、`Callbacks`、`DriverIrp` 也沒有發現明顯 Kernel Hook，因此目前不視為主要可疑證據。

---

### 5.2 兩筆 N/A 項目

另外兩筆結果為：

```text
0x12ab0301  N/A
0x7ac546dc  N/A
```

這兩筆沒有顯示 Driver Name、Service Key 或 Alternative Name。

這種情況可能是記憶體中殘留的 Driver Object、解析不完整的結構，或記憶體映像中的資料不完整造成。

由於目前沒有更多名稱、路徑或模組資訊，不能單獨判斷為惡意。

---

## 6. 鑑識判斷

本次 `DriverModule` 結果沒有看到以下明顯可疑情況：

```text
可疑 Driver 名稱
可疑 Service Key
與 Rick And Morty 或 vmware-tray.exe 相關的 Driver
明顯未知 Driver Hook
明確的 Kernel Rootkit 痕跡
```

雖然有兩筆 `N/A` 項目，但缺乏可疑名稱、路徑或其他 Kernel Hook 證據，因此只能作為輔助觀察。

---

## 7. 與本案關聯

本案主要證據集中於 User-mode 執行鏈：

```text
BitTorrent 下載活動
Rick And Morty season 1 download.exe
Temp\RarSFX0\vmware-tray.exe
Malfind / VadInfo 可疑記憶體區段
READ_IT.txt 加密提示檔
```

而 `DriverModule` 主要檢查 Driver Object 與 Kernel Module 的對應狀況。

本次沒有發現明顯 Driver Module 異常，因此本案目前仍較不像 Kernel Driver Rootkit，而是使用者執行可疑 EXE 後造成的 User-mode 感染與加密行為。

---

## 8. 結論

`windows.drivermodule.DriverModule` 成功執行，結果僅顯示少量 Driver Object 對應資訊。

其中 `\FileSystem\RAW` 屬於 Windows 正常檔案系統相關 Driver Object；另外兩筆 `N/A` 項目缺乏 Driver 名稱與 Service Key，無法單獨判定為惡意。

綜合前面 `Callbacks`、`SSDT`、`DriverIrp` 等 Kernel 檢查結果，目前沒有發現明顯 Kernel Driver Rootkit 或 Driver Module Hook 跡象。

本案重點仍應放在：

```text
Rick 使用者執行可疑 Torrent EXE
Rick And Morty 啟動 vmware-tray.exe
vmware-tray.exe 出現可疑記憶體區段
READ_IT.txt 顯示檔案遭加密
```
