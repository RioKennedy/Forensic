# 測試內容

- .\vol.exe -f .\OtterCTF.vmem windows.poolscanner.PoolScanner

```
D:\Forensic\G140A006\VolatilityWorkbench>.\vol.exe -f .\OtterCTF.vmem windows.poolscanner.PoolScanner
Volatility 3 Framework 2.5.0
Progress:  100.00               PDB scanning finished
Tag     Offset  Layer   Name

symbol_table_name1!_OBJECT_SYMBOLIC_LINK        0x156508a       memory_layer    N/A
symbol_table_name1!_OBJECT_SYMBOLIC_LINK        0x1c2f640       memory_layer    N/A
symbol_table_name1!_OBJECT_SYMBOLIC_LINK        0x1c2fad0       memory_layer    N/A
symbol_table_name1!_OBJECT_SYMBOLIC_LINK        0x1c2fb50       memory_layer    N/A
symbol_table_name1!_OBJECT_SYMBOLIC_LINK        0x2118b7d       memory_layer    N/A
symbol_table_name1!_LDR_DATA_TABLE_ENTRY        0x2b20881       memory_layer    N/A
symbol_table_name1!_RTL_ATOM_TABLE      0x2d30f6b       memory_layer    N/A
symbol_table_name1!_CMHIVE      0x2d49b84       memory_layer    N/A
symbol_table_name1!_LDR_DATA_TABLE_ENTRY        0x2e66297       memory_layer    N/A
symbol_table_name1!_LDR_DATA_TABLE_ENTRY        0x2eb4135       memory_layer    N/A
symbol_table_name1!_OBJECT_SYMBOLIC_LINK        0x34a8310       memory_layer    N/A
symbol_table_name1!_OBJECT_SYMBOLIC_LINK        0x34a8f80       memory_layer    N/A
symbol_table_name1!_DRIVER_OBJECT       0x5ded280       memory_layer    N/A
symbol_table_name1!_FILE_OBJECT 0x5def220       memory_layer    \$Directory
symbol_table_name1!_DRIVER_OBJECT       0x5df5280       memory_layer    N/A
symbol_table_name1!_KMUTANT     0x5df6310       memory_layer    N/A
symbol_table_name1!_FILE_OBJECT 0x5df6780       memory_layer    \Windows\System32
symbol_table_name1!_DRIVER_OBJECT       0x5dfe000       memory_layer    N/A
symbol_table_name1!_DRIVER_OBJECT       0x5dfe2b0       memory_layer    N/A
symbol_table_name1!_CMHIVE      0x9aaa65e       memory_layer    N/A
symbol_table_name1!_OBJECT_SYMBOLIC_LINK        0xb79b890       memory_layer    N/A
symbol_table_name1!_CMHIVE      0xb92b000       memory_layer    N/A
symbol_table_name1!_OBJECT_SYMBOLIC_LINK        0xc9dd510       memory_layer    N/A
symbol_table_name1!_CMHIVE      0xdb41400       memory_layer    N/A
symbol_table_name1!_OBJECT_SYMBOLIC_LINK        0xddc37b0       memory_layer    N/A
symbol_table_name1!_RTL_ATOM_TABLE      0xe614000       memory_layer    N/A
...
....
.....
```

# 測試內容

- .\vol.exe -f .\OtterCTF.vmem windows.poolscanner.PoolScanner | findstr "Rick Morty vmware-tray RarSFX READ_IT ransom encrypt crypt"

```
D:\Forensic\G140A006\VolatilityWorkbench>.\vol.exe -f .\OtterCTF.vmem windows.poolscanner.PoolScanner | findstr "Rick Morty vmware-tray RarSFX READ_IT ransom encrypt crypt"
symbol_table_name1!_FILE_OBJECT 0x7d405200ng finmemory_layer    \Users\Rick\AppData\Roaming\BitTorrent\dlimagecache\165F6EF40A81DD175FFAEA69E77ABFD30B27E71C
symbol_table_name1!_FILE_OBJECT 0x7d436700      memory_layer    \Users\Rick\AppData\Local\Microsoft\Windows\WER\ERC
symbol_table_name1!_FILE_OBJECT 0x7d436c10      memory_layer    \Users\Rick\AppData\Local\Temp\nstB409.tmp
symbol_table_name1!_FILE_OBJECT 0x7d436eb0      memory_layer    \Users\Rick\AppData\Local\Temp\nstB3D5.tmp
symbol_table_name1!_FILE_OBJECT 0x7d44b500      memory_layer    \Users\Rick\AppData\Local\Temp\nstB395.tmp
symbol_table_name1!_FILE_OBJECT 0x7d44e4b0      memory_layer    \Users\Rick\AppData\Roaming\Microsoft\Windows\Recent\Downloads.lnk
symbol_table_name1!_FILE_OBJECT 0x7d44e700      memory_layer    \Users\Rick\AppData\Local\Temp\nstB3F7.tmp
symbol_table_name1!_FILE_OBJECT 0x7d44e9a0      memory_layer    \Users\Rick\AppData\Local\Temp\nstB41B.tmp
symbol_table_name1!_FILE_OBJECT 0x7d44ed60      memory_layer    \Users\Rick\AppData\Local\Temp\nstB3F9.tmp
symbol_table_name1!_FILE_OBJECT 0x7d44f430      memory_layer    \Users\Rick\AppData\Local\Temp\nstB3C5.tmp
symbol_table_name1!_FILE_OBJECT 0x7d44feb0      memory_layer    \Users\Rick\AppData\Local\Temp\nstB3F8.tmp
symbol_table_name1!_FILE_OBJECT 0x7d450eb0      memory_layer    \Users\Rick\AppData\Local\Temp\nstB3E6.tmp
symbol_table_name1!_FILE_OBJECT 0x7d452d60      memory_layer    \Users\Rick\AppData\Local\Temp\nstB40A.tmp
symbol_table_name1!_FILE_OBJECT 0x7d45dc50      memory_layer    \Users\Rick\AppData\Local\Google\Chrome\User Data\Default\History
symbol_table_name1!_FILE_OBJECT 0x7d475340      memory_layer    \Windows\System32\en-US\crypt32.dll.mui
symbol_table_name1!_FILE_OBJECT 0x7d60f240      memory_layer    \Users\Rick\AppData\Local\Google\Chrome\User Data\Default\Extension Rules\MANIFEST-000001
symbol_table_name1!_FILE_OBJECT 0x7d61b000      memory_layer    \Users\Rick\AppData\Roaming\Microsoft\Windows\Recent\Flag.txt.WINDOWS.lnk
symbol_table_name1!_FILE_OBJECT 0x7d62bd60      memory_layer    \Users\Rick\AppData\Local\Microsoft\Windows\History\Low\History.IE5\MSHist012018080420180805\index.dat
symbol_table_name1!_FILE_OBJECT 0x7d63db50      memory_layer    \Torrents\Rick And Morty season 1 download.exe
symbol_table_name1!_FILE_OBJECT 0x7d63ebc0      memory_layer    \Users\Rick\AppData\Local\Lavasoft\WebCompanion.exe_Url_siq0lwf3tzgxp2khfkllybk3idtbehng\4.3.1865.3518\user.configwcfg
symbol_table_name1!_FILE_OBJECT 0x7d641c10      memory_layer    \Windows\System32\en-US\crypt32.dll.mui
symbol_table_name1!_FILE_OBJECT 0x7d6453e0      memory_layer    \Windows\SysWOW64\cryptnet.dll
symbol_table_name1!_FILE_OBJECT 0x7d651000      memory_layer    \Users\Rick\AppData\Local\Google\Chrome\User Data\Default\Extension Rules\CURRENT
symbol_table_name1!_FILE_OBJECT 0x7d660490      memory_layer    \Users\Rick\Desktop\READ_IT.txt
symbol_table_name1!_FILE_OBJECT 0x7d679000      memory_layer    \Users\Rick\AppData\LocalLow\BitTorrent\BitTorrent_2836_00313D08_590648902
symbol_table_name1!_FILE_OBJECT 0x7d679290      memory_layer    \Users\Rick\AppData\Local\Google\Chrome\User Data\Default\Extension Rules\000003.log
symbol_table_name1!_EPROCESS    0x7d686ad0      memory_layer    Rick And Morty
symbol_table_name1!_FILE_OBJECT 0x7d68d450      memory_layer    \Users\Rick\AppData\LocalLow\Microsoft\CryptnetUrlCache\MetaData
symbol_table_name1!_FILE_OBJECT 0x7d68feb0      memory_layer    \Users\Rick\AppData\Local\Temp\SND49db.tmp
symbol_table_name1!_FILE_OBJECT 0x7d6995f0      memory_layer    \Users\Rick\AppData\Local\Temp\SND1fee.tmp
symbol_table_name1!_FILE_OBJECT 0x7d69ad70      memory_layer    \Users\Rick\AppData\Roaming\BitTorrent\updates\7.10.3_44495\bittorrentie.exe
symbol_table_name1!_FILE_OBJECT 0x7d6a7000      memory_layer    \Users\Rick\AppData\Roaming\BitTorrent\updates\7.10.3_44495\bittorrentie.exe
symbol_table_name1!_FILE_OBJECT 0x7d6b39a0      memory_layer    \Torrents\Rick and Morty - Season 3 (2017) [1080p]\Rick.and.Morty.S03E07.The.Ricklantis.Mixup.1080p.Amazon.WEB-DL.x264-Rapta.mkv
symbol_table_name1!_FILE_OBJECT 0x7d6cb9b0      memory_layer    \Users\Rick\AppData\Roaming\Microsoft\Windows\Start Menu
symbol_table_name1!_FILE_OBJECT 0x7d6da790      memory_layer    \Users\Rick\AppData\LocalLow\BitTorrent\BitTorrent_2836_00313978_1933444659
symbol_table_name1!_FILE_OBJECT 0x7d6e5b60      memory_layer    \Users\Rick\AppData\Local\GDIPFONTCACHEV1.DAT
symbol_table_name1!_FILE_OBJECT 0x7d6ea7b0      memory_layer    \Users\Rick\AppData\Local\Microsoft\Windows\History\Low\History.IE5\index.dat
symbol_table_name1!_FILE_OBJECT 0x7d6ec180      memory_layer    \Users\Rick\AppData\Roaming\Microsoft\Windows\Cookies\Low\index.dat
symbol_table_name1!_FILE_OBJECT 0x7d6ed7e0      memory_layer    \Users\Rick\AppData\LocalLow\Microsoft\CryptnetUrlCache\MetaData\0DA515F703BB9B49479E8697ADB0B955_7DC3E633EDFAEFC3AA3C99552548EC2F
symbol_table_name1!_FILE_OBJECT 0x7d7005d0      memory_layer    \Users\Rick\AppData\Local\Google\Chrome\User Data\Subresource Filter\Indexed Rules\20\7.54\Ruleset Data
symbol_table_name1!_FILE_OBJECT 0x7d717630      memory_layer    \Users\Rick\AppData\Roaming\Microsoft\Windows\IETldCache\Low\index.dat
symbol_table_name1!_FILE_OBJECT 0x7d71b5a0      memory_layer    \Users\Rick\AppData\Local\Google\Chrome\User Data\Default\Extension Rules\LOCK
symbol_table_name1!_FILE_OBJECT 0x7d71bca0      memory_layer    \Users\Rick\AppData\Roaming\Microsoft\Internet Explorer\Quick Launch\User Pinned
symbol_table_name1!_FILE_OBJECT 0x7d735430      memory_layer    \Users\Rick\AppData\Local\Temp\SND3f7f.tmp
symbol_table_name1!_FILE_OBJECT 0x7d74c260      memory_layer    \Users\Rick\Desktop
symbol_table_name1!_FILE_OBJECT 0x7d74c470      memory_layer    \Users\Rick\AppData\Roaming\Microsoft\Windows\Cookies\Low\index.dat
symbol_table_name1!_FILE_OBJECT 0x7d74cac0      memory_layer    \Users\Rick\AppData\Local\Microsoft\Windows\Temporary Internet Files\Low\Content.IE5\index.dat
symbol_table_name1!_FILE_OBJECT 0x7d74eac0      memory_layer    \Users\Rick\AppData\Local\Microsoft\Windows\History\Low\History.IE5\index.dat
symbol_table_name1!_FILE_OBJECT 0x7d750d60      memory_layer    \Users\Rick\AppData\Roaming\Microsoft\Windows\IETldCache\Low\index.dat
symbol_table_name1!_FILE_OBJECT 0x7d762eb0      memory_layer    \Users\Rick\AppData\Roaming\Microsoft\Crypto\RSA\S-1-5-21-1923827501-2510115606-422599235-1000\f84702e000b768c3eb589cfdb38d4468_8349e3fe-e027-4c9a-a69b-4865c51e6cb4
symbol_table_name1!_FILE_OBJECT 0x7d76b680      memory_layer    \Users\Rick\AppData\Local\Google\Chrome\User Data\Default\Login Data
symbol_table_name1!_FILE_OBJECT 0x7d76d510      memory_layer    \Users\Rick\AppData\Local\Google\Chrome\User Data\Default\Cache\f_000178
symbol_table_name1!_FILE_OBJECT 0x7d776660      memory_layer    \Users\Rick\AppData\Roaming\Microsoft\Windows\Network Shortcuts
symbol_table_name1!_FILE_OBJECT 0x7d776870      memory_layer    \Users\Rick\AppData\Local\Microsoft\Windows\Temporary Internet Files\Low\Content.IE5\6CYX5H6R\index[2].htm
symbol_table_name1!_FILE_OBJECT 0x7d788940      memory_layer    \Users\Rick\Links
```


# windows.poolscanner.PoolScanner 分析

## 1. Plugin 功能說明

`windows.poolscanner.PoolScanner` 用來掃描 Windows Kernel Pool 中殘留的物件。

此 Plugin 可以找出記憶體中的多種 Kernel Object，例如：

```text
_FILE_OBJECT
_EPROCESS
_DRIVER_OBJECT
_KMUTANT
_OBJECT_SYMBOLIC_LINK
_CMHIVE
_LDR_DATA_TABLE_ENTRY
```

在數位鑑識中，`PoolScanner` 可以用來尋找已配置或殘留在記憶體中的物件，包含 Process、File Object、Driver Object、Registry Hive 等。

它常用於輔助確認可疑 Process、檔案路徑或系統物件是否曾經存在於記憶體中。

---

## 2. 執行指令

```bash
.\vol.exe -f .\OtterCTF.vmem windows.poolscanner.PoolScanner
```

由於輸出結果非常多，因此使用 `findstr` 搜尋本案相關關鍵字：

```bash
.\vol.exe -f .\OtterCTF.vmem windows.poolscanner.PoolScanner | findstr "Rick Morty vmware-tray RarSFX READ_IT ransom encrypt crypt"
```

---

## 3. 欄位說明

| 欄位       | 說明                          |
| -------- | --------------------------- |
| `Tag`    | 掃描到的 Kernel Object 類型       |
| `Offset` | 該物件在記憶體中的位址                 |
| `Layer`  | 所在記憶體層，通常為 `memory_layer`   |
| `Name`   | 物件名稱，例如檔案路徑、Process 名稱或物件名稱 |

---

## 4. 原始結果觀察

完整執行 `PoolScanner` 後，可以看到許多不同類型的 Kernel Object，例如：

```text
_OBJECT_SYMBOLIC_LINK
_LDR_DATA_TABLE_ENTRY
_RTL_ATOM_TABLE
_CMHIVE
_DRIVER_OBJECT
_FILE_OBJECT
_KMUTANT
```

這代表 Plugin 成功從記憶體中掃描出多種 Kernel Pool 物件。

其中大部分物件名稱為 `N/A`，這在 Pool Scanner 結果中屬於常見情況，不能單獨判斷為異常。

---

## 5. 本案關鍵搜尋結果

本次針對本案主線關鍵字搜尋後，找到多個重要物件。

### 5.1 可疑 Process：Rick And Morty

搜尋結果中出現：

```text
_EPROCESS    0x7d686ad0    memory_layer    Rick And Morty
```

這表示 `PoolScanner` 在 Kernel Pool 中掃描到 `Rick And Morty` 的 EPROCESS 物件。

此結果可補強前面 `PsList`、`PsTree`、`CmdLine` 中看到的可疑 Process。

---

### 5.2 可疑執行檔：Rick And Morty season 1 download.exe

搜尋結果中出現：

```text
_FILE_OBJECT    0x7d63db50    memory_layer    \Torrents\Rick And Morty season 1 download.exe
```

此檔案位於 `\Torrents` 目錄，名稱看似影片下載內容，但副檔名為 `.exe`。

這與前面 `CmdLine` 結果一致，該檔案是本案主要可疑執行檔。

此結果可補強：

```text
Rick 使用者曾經執行或存取該可疑 EXE
```

---

### 5.3 加密提示檔：READ_IT.txt

搜尋結果中出現：

```text
_FILE_OBJECT    0x7d660490    memory_layer    \Users\Rick\Desktop\READ_IT.txt
```

`READ_IT.txt` 是本案非常重要的檔案，前面 DumpFiles 已經確認其內容包含：

```text
Your files have been encrypted.
Read the Program for more information
```

因此，PoolScanner 掃到 `READ_IT.txt` 的 File Object，可以補強系統中存在加密提示檔。

---

### 5.4 Flag shortcut：Flag.txt.WINDOWS.lnk

搜尋結果中出現：

```text
_FILE_OBJECT    0x7d61b000    memory_layer    \Users\Rick\AppData\Roaming\Microsoft\Windows\Recent\Flag.txt.WINDOWS.lnk
```

這代表系統中存在 `Flag.txt.WINDOWS.lnk` 的 Recent shortcut。

此結果與前面 `Filescan` 和 `MFTScan` 的結果一致，可作為使用者曾經接觸或開啟該檔案的輔助跡證。

---

### 5.5 BitTorrent 相關檔案

搜尋結果中也看到多個 BitTorrent 相關物件，例如：

```text
\Users\Rick\AppData\Roaming\BitTorrent\dlimagecache\...
\Users\Rick\AppData\LocalLow\BitTorrent\BitTorrent_2836_...
\Users\Rick\AppData\Roaming\BitTorrent\updates\7.10.3_44495\bittorrentie.exe
```

這些結果與前面 `PsList`、`NetScan`、`UserAssist` 中看到的 BitTorrent 活動一致。

因此，PoolScanner 也補強了本案與 BitTorrent 下載活動有關。

---

### 5.6 Rick 使用者活動路徑

結果中大量出現 Rick 使用者目錄，例如：

```text
\Users\Rick\AppData\Local\Temp\
\Users\Rick\AppData\Local\Google\Chrome\User Data\Default\History
\Users\Rick\AppData\Local\Google\Chrome\User Data\Default\Login Data
\Users\Rick\AppData\Roaming\Microsoft\Windows\Recent\
\Users\Rick\Desktop
```

這些結果顯示 Rick 使用者環境中存在瀏覽器、暫存檔、Recent shortcut、桌面檔案與 BitTorrent 相關活動。

---

## 6. 與本案主線的關聯

`PoolScanner` 搜尋結果可與前面證據互相補強：

```text
PsList / PsTree：發現 Rick And Morty process
CmdLine：確認 Rick And Morty season 1 download.exe 來自 Torrents 目錄
UserAssist：確認 Rick 使用者曾執行可疑 EXE
Filescan：發現 READ_IT.txt、Flag.txt.WINDOWS.lnk、可疑 EXE
DumpFiles：成功還原 READ_IT.txt 與可疑 EXE
PoolScanner：從 Kernel Pool 中再次找到相關 EPROCESS 與 FILE_OBJECT
```

因此，`PoolScanner` 在本案中提供的是輔助證據，證明這些可疑 Process 與 File Object 確實存在於記憶體物件中。

---

## 7. 與 BigPools 的差異

前面 `BigPools` 沒有找到本案關鍵字，因為 BigPools 主要列出大型 Kernel memory allocation 與 Pool Tag。

而 `PoolScanner` 是掃描具體 Kernel Object，例如 Process Object 與 File Object。

因此，本案中：

```text
BigPools：沒有直接證據
PoolScanner：有找到 Rick And Morty、READ_IT.txt、Torrents EXE 等相關物件
```

所以 `PoolScanner` 的價值比 `BigPools` 更高。

---

## 8. 鑑識判斷

本次 `PoolScanner` 發現以下重要項目：

```text
1. _EPROCESS：Rick And Morty
2. _FILE_OBJECT：\Torrents\Rick And Morty season 1 download.exe
3. _FILE_OBJECT：\Users\Rick\Desktop\READ_IT.txt
4. _FILE_OBJECT：\Users\Rick\AppData\Roaming\Microsoft\Windows\Recent\Flag.txt.WINDOWS.lnk
5. 多個 BitTorrent 相關 File Object
6. 多個 Rick 使用者 AppData / Temp / Chrome / Recent 路徑
```

這些結果支持本案主線：

```text
Rick 使用者
→ BitTorrent 下載活動
→ 執行 Rick And Morty season 1 download.exe
→ 系統出現 READ_IT.txt 加密提示
```

不過，`PoolScanner` 本身不直接證明加密行為，它主要是證明相關物件存在於記憶體中。

---

## 9. 結論

`windows.poolscanner.PoolScanner` 成功掃描 Kernel Pool 中的物件。

本次結果中發現與本案主線直接相關的 `Rick And Morty` EPROCESS、`\Torrents\Rick And Morty season 1 download.exe`、`\Users\Rick\Desktop\READ_IT.txt`、`Flag.txt.WINDOWS.lnk` 以及多個 BitTorrent 相關 File Object。

因此，`PoolScanner` 可作為本案的重要輔助證據，補強前面 `PsList`、`PsTree`、`CmdLine`、`UserAssist`、`Filescan` 與 `DumpFiles` 的分析結果。

綜合判斷，本案仍偏向 Rick 使用者執行可疑 Torrent EXE 後，啟動後續惡意行為並產生加密提示檔的 User-mode 感染鏈。

本案主線如下：

```text
Rick 使用者
→ BitTorrent 下載活動
→ \Torrents\Rick And Morty season 1 download.exe
→ Temp\RarSFX0\vmware-tray.exe
→ 可疑記憶體區段
→ \Users\Rick\Desktop\READ_IT.txt
```
