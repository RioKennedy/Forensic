# 測試內容
- .\vol.exe -f .\OtterCTF.vmem windows.bigpools.BigPools
  
```
D:\Forensic\G140A006\VolatilityWorkbench>.\vol.exe -f .\OtterCTF.vmem windows.bigpools.BigPools
Volatility 3 Framework 2.5.0
Progress:  100.00               PDB scanning finished
Allocation      Tag     PoolType        NumberOfBytes   Status

0xf8a003c09000  CM31    PagedPoolCacheAligned   0x1000  Allocated
0xf8a0040cb000  CM31    PagedPoolCacheAligned   0x1000  Allocated
0xf8a00032c000  CMA     PagedPool       0x1000  Allocated
0xf8a00458d000  CM31    PagedPoolCacheAligned   0x1000  Allocated
0xfa8019cfd000  Cont    NonPagedPool    0x1000  Allocated
0xf8a004a4f000  CM31    PagedPoolCacheAligned   0x1000  Allocated
0xf8a000cb0000  CM25    PagedPool       0x1000  Allocated
0xf8a004f11000  CM31    PagedPoolCacheAligned   0x1000  Allocated
0xf8a001172000  CM25    PagedPool       0x1000  Allocated
0xf8a0053d3000  CM31    PagedPoolCacheAligned   0x1000  Allocated
0xfa8019cc2000  Cont    NonPagedPool    0x1000  Allocated
0xf8a005d57000  CM31    PagedPoolCacheAligned   0x3000  Allocated
0xf8a005ce1000  CM31    PagedPoolCacheAligned   0x1000  Allocated
0xfa80193b4000  Cont    NonPagedPool    0x1250  Allocated
0xf8a006665000  MmSt    Unknown choice 2147483649       0x1000  Allocated
0xfa8019876000  Dev     NonPagedPool    0x18f0  Allocated
0xfa8019d38000  Cont    NonPagedPool    0x1000  Allocated
0xfa801a1fa000  VM3D    NonPagedPool    0x1000  Allocated
0xf8a003bce000  CM31    PagedPoolCacheAligned   0x1000  Allocated
0xf8a004090000  CM31    PagedPoolCacheAligned   0x1000  Allocated
0xf8a0002f1000  CMA     PagedPool       0x1000  Allocated
0xf8a004552000  CM31    PagedPoolCacheAligned   0x1000  Allocated
0xf8a0007b3000  CM25    PagedPool       0x1000  Allocated
0xf8a004a14000  CM31    PagedPoolCacheAligned   0x1000  Allocated
0xf8a000c75000  CM25    PagedPool       0x1000  Allocated
0xf8a004ed6000  CM31    PagedPoolCacheAligned   0x1000  Allocated
0xf8a001137000  CM25    PagedPool       0x1000  Allocated
0xf8a005398000  CM31    PagedPoolCacheAligned   0x1000  Allocated
0xf8a00585a000  CM31    PagedPoolCacheAligned   0x1000  Allocated
0xf8a004141000  CM31    PagedPoolCacheAligned   0x1000  Allocated
0xfa8019d73000  Cont    NonPagedPool    0x1000  Allocated
0xf8a000864000  CM25    PagedPool       0x1000  Allocated
0xf8a004ac5000  CM31    PagedPoolCacheAligned   0x1000  Allocated
0xf8a000d26000  CM25    PagedPool       0x1000  Allocated
0xf8a004f87000  CM31    PagedPoolCacheAligned   0x1000  Allocated
0xf8a0011e8000  CM25    PagedPool       0x1000  Allocated
0xf8a005449000  CM31    PagedPoolCacheAligned   0x1000  Allocated
0xf8a00590b000  CM31    PagedPoolCacheAligned   0x1000  Allocated
0xf8a005dcd000  CM31    PagedPoolCacheAligned   0x2000  Allocated
...
....
.....
```

# 測試內容
- .\vol.exe -f .\OtterCTF.vmem windows.bigpools.BigPools | findstr "Rick Morty
- .\vol.exe -f .\OtterCTF.vmem windows.bigpools.BigPools | findstr "Torrents Temp AppData Users Rick"
- .\vol.exe -f .\OtterCTF.vmem windows.bigpools.BigPools | findstr "vmware tray"
- .\vol.exe -f .\OtterCTF.vmem windows.bigpools.BigPools | findstr "Rick And Morty"
- .\vol.exe -f .\OtterCTF.vmem windows.bigpools.BigPools | findstr /c:"Rick And Morty"
```
D:\Forensic\G140A006\VolatilityWorkbench>.\vol.exe -f .\OtterCTF.vmem windows.bigpools.BigPools | findstr "Rick Morty vmware-tray RarSFX READ_IT ransom encrypt crypt"
Progress:  100.00               PDB scanning finished
D:\Forensic\G140A006\VolatilityWorkbench>.\vol.exe -f .\OtterCTF.vmem windows.bigpools.BigPools | findstr "Torrents Temp AppData Users Rick"
Progress:  100.00               PDB scanning finished
D:\Forensic\G140A006\VolatilityWorkbench>.\vol.exe -f .\OtterCTF.vmem windows.bigpools.BigPools | findstr "vmware tray"
Progress:  100.00               PDB scanning finished
D:\Forensic\G140A006\VolatilityWorkbench>.\vol.exe -f .\OtterCTF.vmem windows.bigpools.BigPools | findstr "Rick And Morty"
Progress:  100.00               PDB scanning finished
D:\Forensic\G140A006\VolatilityWorkbench>.\vol.exe -f .\OtterCTF.vmem windows.bigpools.BigPools | findstr /c:"Rick And Morty"
Progress:  100.00               PDB scanning finished
```

# windows.bigpools.BigPools 分析

## 1. Plugin 功能說明

`windows.bigpools.BigPools` 用來列出 Windows Kernel Big Pool allocation。

Big Pool 是 Windows Kernel 在配置較大型記憶體區塊時使用的機制。
每一筆 allocation 會包含記憶體位置、Pool Tag、Pool 類型、大小與狀態。

在數位鑑識中，`BigPools` 可以作為 Kernel 層面的輔助檢查，用來觀察是否存在可疑的 Kernel memory allocation、異常 Pool Tag，或可能與 Rootkit、惡意 Driver 有關的記憶體配置。

---

## 2. 執行指令

```bash
.\vol.exe -f .\OtterCTF.vmem windows.bigpools.BigPools
```

由於輸出結果較多，因此另外使用 `findstr` 搜尋與本案相關的關鍵字：

```bash
.\vol.exe -f .\OtterCTF.vmem windows.bigpools.BigPools | findstr "Rick Morty vmware-tray RarSFX READ_IT ransom encrypt crypt"
```

```bash
.\vol.exe -f .\OtterCTF.vmem windows.bigpools.BigPools | findstr "Torrents Temp AppData Users Rick"
```

```bash
.\vol.exe -f .\OtterCTF.vmem windows.bigpools.BigPools | findstr "vmware tray"
```

```bash
.\vol.exe -f .\OtterCTF.vmem windows.bigpools.BigPools | findstr "Rick And Morty"
```

```bash
.\vol.exe -f .\OtterCTF.vmem windows.bigpools.BigPools | findstr /c:"Rick And Morty"
```

---

## 3. 欄位說明

`BigPools` 的輸出欄位如下：

| 欄位              | 中文說明     | 意義                                       |
| --------------- | -------- | ---------------------------------------- |
| `Allocation`    | 記憶體配置位址  | Big Pool allocation 在 Kernel memory 中的位置 |
| `Tag`           | Pool Tag | Windows Kernel 用來標記該記憶體區塊用途的 4 字元代碼      |
| `PoolType`      | Pool 類型  | 表示該記憶體屬於 Paged Pool、NonPaged Pool 或其他類型  |
| `NumberOfBytes` | 配置大小     | 該 Big Pool allocation 使用的記憶體大小           |
| `Status`        | 狀態       | 表示該記憶體區塊目前是否仍被配置使用                       |

---

## 4. 欄位範例說明

本次結果中可看到以下範例：

```text
0xf8a003c09000  CM31  PagedPoolCacheAligned  0x1000  Allocated
```

此筆資料可解釋如下：

| 欄位              | 值                       | 說明                                                       |
| --------------- | ----------------------- | -------------------------------------------------------- |
| `Allocation`    | `0xf8a003c09000`        | Kernel Big Pool allocation 的記憶體位址                        |
| `Tag`           | `CM31`                  | Pool Tag，通常與 Windows Configuration Manager / Registry 相關 |
| `PoolType`      | `PagedPoolCacheAligned` | 表示此記憶體區塊屬於 Paged Pool，且有 Cache Aligned 對齊                |
| `NumberOfBytes` | `0x1000`                | 配置大小為 `0x1000` bytes，也就是 4096 bytes                      |
| `Status`        | `Allocated`             | 表示該記憶體區塊目前仍處於已配置狀態                                       |

---

## 5. Pool Type 說明

`PoolType` 代表 Kernel memory 的配置類型。

常見類型如下：

| Pool Type               | 說明                              |
| ----------------------- | ------------------------------- |
| `PagedPool`             | 可被換出到磁碟的 Kernel memory          |
| `NonPagedPool`          | 不可被換出到磁碟，必須常駐記憶體的 Kernel memory |
| `PagedPoolCacheAligned` | 經過 Cache 對齊的 Paged Pool         |
| `Unknown`               | Volatility 無法明確解析的 Pool 類型      |

在鑑識分析中，`NonPagedPool` 較常被關注，因為 Driver、Device Object 或 Kernel-level 元件常會使用 NonPaged Pool。

但單純看到 `NonPagedPool` 並不代表惡意，仍需要搭配 Pool Tag、Driver、DeviceTree、DriverIrp 等結果一起判斷。

---

## 6. 原始結果觀察

完整執行 `BigPools` 後，可以看到大量 Kernel Pool allocation，例如：

```text
CM31
CMA
CM25
Cont
MmSt
Dev
VM3D
```

這些 Pool Tag 大多屬於 Windows Kernel 或 VMware 環境中的常見配置。

常見 Tag 說明如下：

| Tag                     | 可能意義                                           |
| ----------------------- | ---------------------------------------------- |
| `CM31` / `CM25` / `CMA` | 多與 Windows Configuration Manager / Registry 相關 |
| `Cont`                  | Kernel memory 中常見的 pool tag                    |
| `MmSt`                  | Memory Manager 相關                              |
| `Dev`                   | Device Object 相關                               |
| `VM3D`                  | VMware 3D / VMware 顯示相關元件                      |

這些 Pool Tag 本身不代表惡意，必須搭配其他異常現象一起判斷。

---

## 7. 關鍵字搜尋結果

本次使用 `findstr` 搜尋與本案主線相關的關鍵字，包括：

```text
Rick
Morty
Rick And Morty
vmware-tray
RarSFX
READ_IT
ransom
encrypt
crypt
Torrents
Temp
AppData
Users
```

搜尋結果皆沒有回傳符合資料，只顯示：

```text
Progress: 100.00 PDB scanning finished
```

這代表 Volatility 掃描成功完成，但 `BigPools` 中沒有找到與本案主線相關的關鍵字。

---

## 8. 鑑識判斷

本次 `BigPools` 沒有發現與以下可疑項目相關的 Kernel Pool 痕跡：

```text
Rick And Morty season 1 download.exe
vmware-tray.exe
RarSFX0
READ_IT.txt
ransom
encrypt
crypt
```

因此，`BigPools` 沒有提供直接證據來支持 Kernel Pool 層面的惡意活動。

需要注意的是，`BigPools` 主要是檢查 Kernel memory allocation，不是用來尋找一般使用者程式路徑或檔案名稱。

所以沒有找到 `Rick And Morty`、`RarSFX0` 或 `READ_IT` 是合理的，因為這些主要是 User-mode Process 或檔案系統證據，不一定會出現在 Big Pool allocation 中。

---

## 9. 與本案主線的關聯

本案目前主要證據仍集中在 User-mode 感染鏈：

```text
Rick 使用者
→ BitTorrent 下載活動
→ Rick And Morty season 1 download.exe
→ Temp\RarSFX0\vmware-tray.exe
→ 可疑記憶體區段
→ READ_IT.txt 加密提示
```

而 `BigPools` 沒有找到相關 Kernel Pool evidence，因此本案目前不偏向 Kernel Rootkit 或 Driver-level 攻擊。

---

## 10. 與其他 Kernel Plugin 的關聯

本次結果與前面其他 Kernel 層 Plugin 的分析結果一致：

```text
Modules：未發現明確可疑 Kernel Module
ModScan：未發現明確隱藏 Driver
Callbacks：未發現明確可疑 Callback
SSDT：未發現明確 SSDT Hook
DriverIrp：未發現明確 Driver Hook
DriverScan：未發現明確惡意 Driver
DeviceTree：未發現可疑 Device Stack 附掛
BigPools：未發現與本案主線相關的 Kernel Pool 痕跡
```

因此，整體 Kernel 層分析結果支持：本案目前不像是 Kernel-mode Rootkit 或 Driver-level 攻擊。

---

## 11. 結論

`windows.bigpools.BigPools` 成功列出 Windows Kernel Big Pool allocation。

結果中雖然可看到多個正常 Kernel Pool Tag，例如 `CM31`、`CMA`、`CM25`、`Cont`、`MmSt`、`Dev`、`VM3D`，但未發現與 `Rick And Morty`、`vmware-tray.exe`、`RarSFX0`、`READ_IT` 或加密相關字串有關的項目。

因此，`BigPools` 在本案中沒有提供直接惡意證據，只能作為 Kernel memory 輔助排查。

綜合判斷，本案目前仍偏向 User-mode 惡意程式執行與檔案加密行為，而不是 Kernel Pool / Rootkit 型攻擊。

---

## 12. 簡短結論

`BigPools` 成功執行，但未發現與 `Rick And Morty`、`vmware-tray.exe`、`RarSFX0`、`READ_IT` 或加密相關的 Kernel Pool 痕跡。

因此，本案目前沒有 Big Pool 層面的明確可疑證據，主線仍偏向 Rick 使用者執行可疑程式後造成的 User-mode 感染鏈。

