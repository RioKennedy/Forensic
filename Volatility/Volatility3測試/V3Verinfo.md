# 測試內容


- vol.exe -f .\OtterCTF.vmem windows.verinfo.VerInfo | findstr 3820
```
D:\Forensic\G140A006\VolatilityWorkbench>.\vol.exe -f .\OtterCTF.vmem windows.verinfo.VerInfo | findstr 3820
3820ressRick And Morty  0x400000PDB scanRick And Morty season 1 download.exe    -       -       --
3820    Rick And Morty  0x776f0000      ntdll.dll       -       -       -       -
3820    Rick And Morty  0x75210000      wow64.dll       -       -       -       -
3820    Rick And Morty  0x751b0000      wow64win.dll    -       -       -       -
3820    Rick And Morty  0x751a0000      wow64cpu.dll    -       -       -       -
```

- vol.exe -f .\OtterCTF.vmem windows.verinfo.VerInfo | findstr 3720
```
D:\Forensic\G140A006\VolatilityWorkbench>.\vol.exe -f .\OtterCTF.vmem windows.verinfo.VerInfo | findstr 3720
3720ressvmware-tray.ex  0xec0000PDB scanvmware-tray.exe 1       0       0       0
3720    vmware-tray.ex  0x776f0000      ntdll.dll       -       -       -       -
3720    vmware-tray.ex  0x75210000      wow64.dll       -       -       -       -
3720    vmware-tray.ex  0x751b0000      wow64win.dll    -       -       -       -
3720    vmware-tray.ex  0x751a0000      wow64cpu.dll    -       -       -       -
```

# windows.verinfo.VerInfo 分析

## 1. Plugin 功能說明

`windows.verinfo.VerInfo` 用來查看記憶體中 EXE / DLL 的版本資訊，例如：

* File Description
* File Version
* Product Name
* Company Name
* Product Version

此 Plugin 可用來判斷檔案是否具有正常軟體資訊，或是否有偽裝成正常程式的情況。

---

## 2. 執行方式

`VerInfo` 不支援 `--pid`，因此本次先執行完整結果，再用 `findstr` 篩選指定 PID：

```bash
.\vol.exe -f .\OtterCTF.vmem windows.verinfo.VerInfo | findstr 3820
.\vol.exe -f .\OtterCTF.vmem windows.verinfo.VerInfo | findstr 3720
```

---

## 3. PID 3820 - Rick And Morty 分析

### 結果重點

```text
3820 Rick And Morty 0x400000 Rick And Morty season 1 download.exe - - - -
```

### 分析

`Rick And Morty season 1 download.exe` 沒有明顯版本資訊，結果多數欄位顯示為 `-`。

這代表該檔案沒有正常軟體常見的公司名稱、產品名稱或版本描述。

再加上檔名偽裝成影片下載，且位於 Torrent 下載目錄，因此可疑程度高。

### 判斷

```text
PID 3820 Rick And Morty 沒有正常版本資訊，支持其為可疑執行檔。
```

---

## 4. PID 3720 - vmware-tray.exe 分析

### 結果重點

```text
3720 vmware-tray.ex 0xec0000 vmware-tray.exe 1 0 0 0
```

### 分析

`vmware-tray.exe` 雖然有出現版本數字 `1.0.0.0`，但沒有看到 VMware 相關的公司名稱、產品名稱或完整描述。

如果是正常 VMware Tools 元件，通常應該會有 VMware 相關版本資訊。

但本次此檔案的路徑是：

```text
\Users\Rick\AppData\Local\Temp\RarSFX0\vmware-tray.exe
```

此路徑不屬於正常 VMware Tools 安裝位置，因此即使有簡單版本號，也不能視為正常 VMware 程式。

### 判斷

```text
PID 3720 vmware-tray.exe 缺少正常 VMware 版本資訊，且位於 Temp\RarSFX0，具有偽裝特徵。
```

---

## 5. 綜合判斷

本次 `VerInfo` 沒有發現這兩個可疑檔案具有可信的正常軟體版本資訊。

|  PID | Process           | VerInfo 判斷                |
| ---: | ----------------- | ------------------------- |
| 3820 | `Rick And Morty`  | 無正常版本資訊，高度可疑              |
| 3720 | `vmware-tray.exe` | 僅有簡單版本號，缺少 VMware 資訊，高度可疑 |

綜合前面分析，可判斷：

```text
Rick And Morty season 1 download.exe
↓
Temp\RarSFX0\vmware-tray.exe
```

這兩個檔案都缺少可信的版本資訊，因此更支持它們屬於同一條可疑執行鏈。

---

## 6. 結論

`windows.verinfo.VerInfo` 結果顯示，`Rick And Morty season 1 download.exe` 沒有正常版本資訊，而 `vmware-tray.exe` 雖然有版本號 `1.0.0.0`，但缺少 VMware 公司名稱或產品資訊。

因此，`vmware-tray.exe` 不像正常 VMware Tools 元件，而比較像是假冒 VMware 名稱的可疑程式。

本次 `VerInfo` 結果補強前面判斷：`Rick And Morty` 是主要可疑執行檔，`vmware-tray.exe` 是其釋放或啟動的可疑子程式。
