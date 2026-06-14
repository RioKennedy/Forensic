# 測試內容
- vol.exe -f .\OtterCTF.vmem windows.symlinkscan.SymlinkScan

```
D:\Forensic\G140A006\VolatilityWorkbench>.\vol.exe -f .\OtterCTF.vmem windows.symlinkscan.SymlinkScan
Volatility 3 Framework 2.5.0
Progress:  100.00               PDB scanning finished
Offset  CreateTime      From Name       To Name
```

# windows.symlinkscan.SymlinkScan 分析

## 1. Plugin 功能說明

`windows.symlinkscan.SymlinkScan` 用來掃描 Windows Object Manager 中的 Symbolic Link 物件。

Symbolic Link 可用來建立系統物件或裝置路徑之間的對應關係，例如：

```text
\GLOBAL??\C:
\Device\HarddiskVolume
\??\C:
```

此 Plugin 可用來輔助分析系統路徑、裝置連結與可能的異常 symbolic link。

---

## 2. 執行指令

```bash
.\vol.exe -f .\OtterCTF.vmem windows.symlinkscan.SymlinkScan
```

---

## 3. 執行結果

本次執行結果如下：

```text
Offset  CreateTime  From Name  To Name
```

結果中僅出現欄位名稱，沒有列出任何 symbolic link 紀錄。

---

## 4. 分析結果

`SymlinkScan` 成功執行，但未發現可分析的 symbolic link 物件。

因此，本 Plugin 在本案中沒有提供與可疑程式、勒索訊息或使用者檔案加密相關的直接證據。

---

## 5. 結論

本次 `windows.symlinkscan.SymlinkScan` 未發現有效 symbolic link 紀錄。

因此，目前沒有證據顯示本案與異常 symbolic link、裝置路徑偽裝或 Object Manager symbolic link 操作有關。

本案主要證據仍集中於：

```text
Rick And Morty season 1 download.exe
Temp\RarSFX0\vmware-tray.exe
READ_IT.txt
Flag.txt.WINDOWS.lnk
BitTorrent 下載痕跡
```

