# 測試內容
- vol.exe -f .\OtterCTF.vmem windows.dumpfiles.DumpFiles


```
D:\Forensic\G140A006\VolatilityWorkbench>.\vol.exe -f .\OtterCTF.vmem -o dump windows.dumpfiles.DumpFiles --physaddr 0x7d660500
Volatility 3 Framework 2.5.0
Progress:  100.00               PDB scanning finished
Cache   FileObject      FileName        Result

DataSectionObject       0x7d660500      READ_IT.txt     file.0x7d660500.0xfa801b2def10.DataSectionObject.READ_IT.txt.dat

D:\Forensic\G140A006\VolatilityWorkbench>.\vol.exe -f .\OtterCTF.vmem -o dump windows.dumpfiles.DumpFiles --physaddr 0x7d61b070
Volatility 3 Framework 2.5.0
Progress:  100.00               PDB scanning finished
Cache   FileObject      FileName        Result

DataSectionObject       0x7d61b070      Flag.txt.WINDOWS.lnk    file.0x7d61b070.0xfa801ab60450.DataSectionObject.Flag.txt.WINDOWS.lnk.dat

D:\Forensic\G140A006\VolatilityWorkbench>.\vol.exe -f .\OtterCTF.vmem -o dump windows.dumpfiles.DumpFiles --physaddr 0x7d63dbc0
Volatility 3 Framework 2.5.0
Progress:  100.00               PDB scanning finished
Cache   FileObject      FileName        Result

DataSectionObject       0x7d63dbc0      Rick And Morty season 1 download.exe    file.0x7d63dbc0.0xfa801b5a8d10.DataSectionObject.Rick And Morty season 1 download.exe.dat
ImageSectionObject      0x7d63dbc0      Rick And Morty season 1 download.exe    file.0x7d63dbc0.0xfa801a79c860.ImageSectionObject.Rick And Morty season 1 download.exe.img

D:\Forensic\G140A006\VolatilityWorkbench>.\vol.exe -f .\OtterCTF.vmem -o dump windows.dumpfiles.DumpFiles --physaddr 0x7daad840
Volatility 3 Framework 2.5.0
Progress:  100.00               PDB scanning finished
Cache   FileObject      FileName        Result

DataSectionObject       0x7daad840      vmware-tray.exe file.0x7daad840.0xfa801ab15890.DataSectionObject.vmware-tray.exe.dat
ImageSectionObject      0x7daad840      vmware-tray.exe file.0x7daad840.0xfa801b494c30.ImageSectionObject.vmware-tray.exe.img
```


# windows.dumpfiles.DumpFiles 分析

## 1. Plugin 功能說明

`windows.dumpfiles.DumpFiles` 用來根據記憶體中的 File Object，將檔案內容從記憶體映像中匯出。

此 Plugin 常搭配 `windows.filescan.FileScan` 使用：

```text
FileScan 找到檔案 Offset
↓
DumpFiles 使用 Offset 匯出檔案
```

---

## 2. 執行結果

本次根據 `FileScan` 找到的重要檔案 Offset，使用 `DumpFiles` 進行匯出。

一開始使用 `--virtaddr` 沒有成功產生結果，後續改用 `--physaddr` 後成功 dump。

---

## 3. READ_IT.txt Dump 結果

### 指令

```bash
.\vol.exe -f .\OtterCTF.vmem -o dump windows.dumpfiles.DumpFiles --physaddr 0x7d660500
```

### 結果

```text
DataSectionObject       0x7d660500      READ_IT.txt     file.0x7d660500.0xfa801b2def10.DataSectionObject.READ_IT.txt.dat
```

### 分析

`READ_IT.txt` 成功匯出，檔案名稱為：

```text
file.0x7d660500.0xfa801b2def10.DataSectionObject.READ_IT.txt.dat
```

此檔案位於 Rick 的 Desktop，可能是提示檔、攻擊說明或事件相關文字檔，應優先開啟檢查內容。

---

## 4. Flag.txt.WINDOWS.lnk Dump 結果

### 指令

```bash
.\vol.exe -f .\OtterCTF.vmem -o dump windows.dumpfiles.DumpFiles --physaddr 0x7d61b070
```

### 結果

```text
DataSectionObject       0x7d61b070      Flag.txt.WINDOWS.lnk    file.0x7d61b070.0xfa801ab60450.DataSectionObject.Flag.txt.WINDOWS.lnk.dat
```

### 分析

`Flag.txt.WINDOWS.lnk` 成功匯出，代表記憶體中仍保留 Flag 相關捷徑檔案內容。

此檔案是 Windows Recent 捷徑，表示使用者 Rick 曾經開啟或存取過 `Flag.txt.WINDOWS`。

---

## 5. Rick And Morty season 1 download.exe Dump 結果

### 指令

```bash
.\vol.exe -f .\OtterCTF.vmem -o dump windows.dumpfiles.DumpFiles --physaddr 0x7d63dbc0
```

### 結果

```text
DataSectionObject       0x7d63dbc0      Rick And Morty season 1 download.exe    file.0x7d63dbc0.0xfa801b5a8d10.DataSectionObject.Rick And Morty season 1 download.exe.dat
ImageSectionObject      0x7d63dbc0      Rick And Morty season 1 download.exe    file.0x7d63dbc0.0xfa801a79c860.ImageSectionObject.Rick And Morty season 1 download.exe.img
```

### 分析

此可疑執行檔成功匯出兩種內容：

| 類型                   | 說明                   |
| -------------------- | -------------------- |
| `DataSectionObject`  | 檔案資料快取內容             |
| `ImageSectionObject` | 程式映像載入內容，通常與執行檔分析較相關 |

`Rick And Morty season 1 download.exe` 位於 `\Torrents` 目錄，檔名偽裝成影片下載，但實際上是 `.exe` 執行檔，因此是本案主要可疑檔案。

---

## 6. vmware-tray.exe Dump 結果

### 指令

```bash
.\vol.exe -f .\OtterCTF.vmem -o dump windows.dumpfiles.DumpFiles --physaddr 0x7daad840
```

### 結果

```text
DataSectionObject       0x7daad840      vmware-tray.exe file.0x7daad840.0xfa801ab15890.DataSectionObject.vmware-tray.exe.dat
ImageSectionObject      0x7daad840      vmware-tray.exe file.0x7daad840.0xfa801b494c30.ImageSectionObject.vmware-tray.exe.img
```

### 分析

`vmware-tray.exe` 成功匯出兩種內容：

| 類型                   | 說明       |
| -------------------- | -------- |
| `DataSectionObject`  | 檔案資料快取內容 |
| `ImageSectionObject` | 程式映像載入內容 |

此檔案路徑原本位於：

```text
\Users\Rick\AppData\Local\Temp\RarSFX0\vmware-tray.exe
```

雖然檔名看起來像 VMware 工具，但它不是從正常 VMware 安裝目錄執行，而是從使用者 Temp 的 `RarSFX0` 目錄執行，因此具有高度可疑性。

---

## 7. 重要 Dump 檔案整理

| 原始檔案                                   |       Offset | Dump 結果              | 判斷        |
| -------------------------------------- | -----------: | -------------------- | --------- |
| `READ_IT.txt`                          | `0x7d660500` | 成功匯出 `.dat`          | 重要提示檔     |
| `Flag.txt.WINDOWS.lnk`                 | `0x7d61b070` | 成功匯出 `.dat`          | Flag 相關捷徑 |
| `Rick And Morty season 1 download.exe` | `0x7d63dbc0` | 成功匯出 `.dat` 與 `.img` | 主要可疑程式    |
| `vmware-tray.exe`                      | `0x7daad840` | 成功匯出 `.dat` 與 `.img` | 可疑子程式     |

<img width="656" height="329" alt="image" src="https://github.com/user-attachments/assets/789a6342-18bd-438d-a1ea-8049384f916e" />

---

## 8. 鑑識判斷

本次 `DumpFiles` 成功匯出多個重要檔案，包含 Flag 相關捷徑、提示檔，以及兩個可疑執行檔。

其中最重要的是：

```text
\Torrents\Rick And Morty season 1 download.exe
\Users\Rick\AppData\Local\Temp\RarSFX0\vmware-tray.exe
```

這兩個檔案可進一步進行 hash、字串分析與靜態分析。
