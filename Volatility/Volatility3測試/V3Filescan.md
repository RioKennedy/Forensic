# 測試內容


- .\vol.exe -f .\OtterCTF.vmem windows.filescan.FileScan
```
D:\Forensic\G140A006\VolatilityWorkbench>.\vol.exe -f .\OtterCTF.vmem windows.filescan.FileScan
Volatility 3 Framework 2.5.0
Progress:  100.00               PDB scanning finished
Offset  Name    Size

0x5def290       \$Directory     216
0x5df67f0       \Windows\System32       216
0x7d402680      \Nexon\MapleStory\l3codeca.acm  216
0x7d405270      \Users\Rick\AppData\Roaming\BitTorrent\dlimagecache\165F6EF40A81DD175FFAEA69E77ABFD30B27E71C     216
0x7d405d20      \Windows\System32\config\systemprofile\AppData\LocalLow\Microsoft\CryptnetUrlCache\MetaData\DDA81A73291E20E6ACF6CACA76D5C942_4D9486FF3A1DA70CF6B67432FCEC9330    216
0x7d406510      \Windows\assembly\NativeImages_v2.0.50727_32\SMDiagnostics\8218dc4808b77f3585fb048c61597af1\SMDiagnostics.ni.dll 216
0x7d413930      \Windows\Microsoft.NET\Framework64\v2.0.50727\CONFIG\machine.config     216
0x7d414dc0      \Windows\System32\en-US\setupapi.dll.mui        216
0x7d418290      \Windows\System32\Tasks\Microsoft\Windows Defender\MP Scheduled Scan    216
0x7d418f20      \Windows\SysWOW64\dinput8.dll   216
0x7d42b7b0      \Endpoint       216
0x7d42c5b0      \Windows\SysWOW64\hid.dll       216
0x7d42d070      \Windows\AppPatch\AcLayers.dll  216
0x7d42d3f0      \Windows\AppPatch\AcGenral.dll  216
0x7d42d540      \Windows\SysWOW64\SortServer2003Compat.dll      216
0x7d42dad0      \Windows\System32\srvcli.dll    216
0x7d42dc20      \Windows\SysWOW64\shunimpl.dll  216
0x7d42dd70      \Windows\SysWOW64\samcli.dll    216
0x7d436370      \Windows\Globalization\Sorting\SortServer2003Compat.nls 216
0x7d436550      \Windows\SysWOW64\sfc.dll       216
0x7d436770      \Users\Rick\AppData\Local\Microsoft\Windows\WER\ERC     216
0x7d436c80      \Users\Rick\AppData\Local\Temp\nstB409.tmp      216
0x7d436dd0      \Windows\System32\catroot\{F750E6C3-38EE-11D1-85E5-00C04FC295EE}\ntph.cat       216
0x7d436f20      \Users\Rick\AppData\Local\Temp\nstB3D5.tmp      216
0x7d43f180      \Nexon\MapleStory\Mob.wz        216
0x7d43fdd0      \Windows\winsxs\x86_microsoft.windows.common-controls_6595b64144ccf1df_5.82.7601.17514_none_ec83dffa859149af\comctl32.dll        216
0x7d440660      \$Directory     216
0x7d440a80      \Windows\SysWOW64\en-US\setupapi.dll.mui        216
0x7d4413d0      \Windows\SysWOW64\icmp.dll      216
0x7d441f20      \Nexon\MapleStory       216
0x7d44a3e0      \Windows\System32\en-US\mf.dll.mui      216
0x7d44b420      \Windows\System32\IPHLPAPI.DLL  216
0x7d44b570      \Users\Rick\AppData\Local\Temp\nstB395.tmp      216
0x7d44bf20      \Nexon\MapleStory\nmconew.dll   216
...
....
.....
```

- .\vol.exe -f .\OtterCTF.vmem windows.filescan.FileScan | findstr "Flag READ_IT"
```
D:\Forensic\G140A006\VolatilityWorkbench>.\vol.exe -f .\OtterCTF.vmem windows.filescan.FileScan | findstr "Flag READ_IT"
0x7d61b070 100.0\Users\Rick\AppData\Roaming\Microsoft\Windows\Recent\Flag.txt.WINDOWS.lnk       216
0x7d660500      \Users\Rick\Desktop\READ_IT.txt 216
```

- .\vol.exe -f .\OtterCTF.vmem windows.filescan.FileScan | findstr "Rick Morty 
```
D:\Forensic\G140A006\VolatilityWorkbench>.\vol.exe -f .\OtterCTF.vmem windows.filescan.FileScan | findstr "Rick Morty download.exe"
0x7d405270 100.0\Users\Rick\AppData\Roaming\BitTorrent\dlimagecache\165F6EF40A81DD175FFAEA69E77ABFD30B27E71C     216
0x7d436770      \Users\Rick\AppData\Local\Microsoft\Windows\WER\ERC     216
0x7d436c80      \Users\Rick\AppData\Local\Temp\nstB409.tmp      216
0x7d436f20      \Users\Rick\AppData\Local\Temp\nstB3D5.tmp      216
0x7d44b570      \Users\Rick\AppData\Local\Temp\nstB395.tmp      216
0x7d44e520      \Users\Rick\AppData\Roaming\Microsoft\Windows\Recent\Downloads.lnk      216
0x7d44e770      \Users\Rick\AppData\Local\Temp\nstB3F7.tmp      216
0x7d44ea10      \Users\Rick\AppData\Local\Temp\nstB41B.tmp      216
0x7d44edd0      \Users\Rick\AppData\Local\Temp\nstB3F9.tmp      216
0x7d44f4a0      \Users\Rick\AppData\Local\Temp\nstB3C5.tmp      216
0x7d44ff20      \Users\Rick\AppData\Local\Temp\nstB3F8.tmp      216
0x7d450f20      \Users\Rick\AppData\Local\Temp\nstB3E6.tmp      216
0x7d452dd0      \Users\Rick\AppData\Local\Temp\nstB40A.tmp      216
0x7d45dcc0      \Users\Rick\AppData\Local\Google\Chrome\User Data\Default\History       216
0x7d60f2b0      \Users\Rick\AppData\Local\Google\Chrome\User Data\Default\Extension Rules\MANIFEST-000001        216
0x7d61b070      \Users\Rick\AppData\Roaming\Microsoft\Windows\Recent\Flag.txt.WINDOWS.lnk       216
0x7d62bdd0      \Users\Rick\AppData\Local\Microsoft\Windows\History\Low\History.IE5\MSHist012018080420180805\index.dat   216
0x7d63dbc0      \Torrents\Rick And Morty season 1 download.exe  216
0x7d63ec30      \Users\Rick\AppData\Local\Lavasoft\WebCompanion.exe_Url_siq0lwf3tzgxp2khfkllybk3idtbehng\4.3.1865.3518\user.configwcfg   216
0x7d651070      \Users\Rick\AppData\Local\Google\Chrome\User Data\Default\Extension Rules\CURRENT216
0x7d660500      \Users\Rick\Desktop\READ_IT.txt 216
0x7d679070      \Users\Rick\AppData\LocalLow\BitTorrent\BitTorrent_2836_00313D08_590648902      216
0x7d679300      \Users\Rick\AppData\Local\Google\Chrome\User Data\Default\Extension Rules\000003.log     216
0x7d68d4c0      \Users\Rick\AppData\LocalLow\Microsoft\CryptnetUrlCache\MetaData        216
0x7d68ff20      \Users\Rick\AppData\Local\Temp\SND49db.tmp      216
0x7d699660      \Users\Rick\AppData\Local\Temp\SND1fee.tmp      216
0x7d69ade0      \Users\Rick\AppData\Roaming\BitTorrent\updates\7.10.3_44495\bittorrentie.exe    216
0x7d6a7070      \Users\Rick\AppData\Roaming\BitTorrent\updates\7.10.3_44495\bittorrentie.exe    216
0x7d6b3a10      \Torrents\Rick and Morty - Season 3 (2017) [1080p]\Rick.and.Morty.S03E07.The.Ricklantis.Mixup.1080p.Amazon.WEB-DL.x264-Rapta.mkv 216
0x7d6cba20      \Users\Rick\AppData\Roaming\Microsoft\Windows\Start Menu        216
0x7d6da800      \Users\Rick\AppData\LocalLow\BitTorrent\BitTorrent_2836_00313978_1933444659     216
0x7d6e5bd0      \Users\Rick\AppData\Local\GDIPFONTCACHEV1.DAT   216
0x7d6ea820      \Users\Rick\AppData\Local\Microsoft\Windows\History\Low\History.IE5\index.dat   216
0x7d6ec1f0      \Users\Rick\AppData\Roaming\Microsoft\Windows\Cookies\Low\index.dat     216
0x7d6ed850      \Users\Rick\AppData\LocalLow\Microsoft\CryptnetUrlCache\MetaData\0DA515F703BB9B49479E8697ADB0B955_7DC3E633EDFAEFC3AA3C99552548EC2F       216
0x7d700640      \Users\Rick\AppData\Local\Google\Chrome\User Data\Subresource Filter\Indexed Rules\20\7.54\Ruleset Data  216
0x7d7176a0      \Users\Rick\AppData\Roaming\Microsoft\Windows\IETldCache\Low\index.dat  216
0x7d71b610      \Users\Rick\AppData\Local\Google\Chrome\User Data\Default\Extension Rules\LOCK  216
0x7d71bd10      \Users\Rick\AppData\Roaming\Microsoft\Internet Explorer\Quick Launch\User Pinned216
0x7d7354a0      \Users\Rick\AppData\Local\Temp\SND3f7f.tmp      216
0x7d74c2d0      \Users\Rick\Desktop     216
0x7d74c4e0      \Users\Rick\AppData\Roaming\Microsoft\Windows\Cookies\Low\index.dat     216
0x7d74cb30      \Users\Rick\AppData\Local\Microsoft\Windows\Temporary Internet Files\Low\Content.IE5\index.dat   216
0x7d74eb30      \Users\Rick\AppData\Local\Microsoft\Windows\History\Low\History.IE5\index.dat   216
0x7d750dd0      \Users\Rick\AppData\Roaming\Microsoft\Windows\IETldCache\Low\index.dat  216
0x7d762f20      \Users\Rick\AppData\Roaming\Microsoft\Crypto\RSA\S-1-5-21-1923827501-2510115606-422599235-1000\f84702e000b768c3eb589cfdb38d4468_8349e3fe-e027-4c9a-a69b-4865c51e6cb4     216
0x7d76b6f0      \Users\Rick\AppData\Local\Google\Chrome\User Data\Default\Login Data    216
0x7d76d580      \Users\Rick\AppData\Local\Google\Chrome\User Data\Default\Cache\f_000178        216
0x7d7766d0      \Users\Rick\AppData\Roaming\Microsoft\Windows\Network Shortcuts 216
0x7d7768e0      \Users\Rick\AppData\Local\Microsoft\Windows\Temporary Internet Files\Low\Content.IE5\6CYX5H6R\index[2].htm       216
0x7d7889b0      \Users\Rick\Links       216
```

- .\vol.exe -f .\OtterCTF.vmem windows.filescan.FileScan | findstr "torrent BitTorrent"
```
D:\Forensic\G140A006\VolatilityWorkbench>.\vol.exe -f .\OtterCTF.vmem windows.filescan.FileScan | findstr "torrent BitTorrent"
0x7d405270 100.0\Users\Rick\AppData\Roaming\BitTorrent\dlimagecache\165F6EF40A81DD175FFAEA69E77ABFD30B27E71C     216
0x7d66d9d0      \BitTorrent_2836_00313D08_590648902     216
0x7d679070      \Users\Rick\AppData\LocalLow\BitTorrent\BitTorrent_2836_00313D08_590648902      216
0x7d699d50      \BitTorrent_2836_00313D08_590648902     216
0x7d69ade0      \Users\Rick\AppData\Roaming\BitTorrent\updates\7.10.3_44495\bittorrentie.exe    216
0x7d6a7070      \Users\Rick\AppData\Roaming\BitTorrent\updates\7.10.3_44495\bittorrentie.exe    216
0x7d6c3070      \BitTorrent_2836_00313978_1933444659    216
0x7d6d8720      \BitTorrent_2836_00313978_1933444659    216
0x7d6da800      \Users\Rick\AppData\LocalLow\BitTorrent\BitTorrent_2836_00313978_1933444659     216
```

# windows.filescan.FileScan 分析

## 1. Plugin 功能說明

`windows.filescan.FileScan` 用來掃描記憶體中的 File Object，找出系統曾經開啟、載入或仍存在於記憶體中的檔案路徑。

此 Plugin 可以用來尋找：

* 可疑執行檔
* 使用者開啟過的檔案
* 暫存檔
* 下載檔案
* Recent 捷徑
* Torrent 相關檔案
* 可能的 Flag 或提示檔案

---

## 2. Plugin 欄位說明

| 欄位       | 說明               |
| -------- | ---------------- |
| `Offset` | 檔案物件在記憶體中的位址     |
| `Name`   | 檔案路徑或物件名稱        |
| `Size`   | File Object 結構大小 |

---

## 3. 執行指令

本次先執行完整 `FileScan`：

```bash
.\vol.exe -f .\OtterCTF.vmem windows.filescan.FileScan
```

由於輸出內容過多，因此再使用 `findstr` 篩選關鍵字。

---

## 4. Flag 與提示檔案

### 執行指令

```bash
.\vol.exe -f .\OtterCTF.vmem windows.filescan.FileScan | findstr "Flag READ_IT"
```

### 結果

```text
0x7d61b070  \Users\Rick\AppData\Roaming\Microsoft\Windows\Recent\Flag.txt.WINDOWS.lnk
0x7d660500  \Users\Rick\Desktop\READ_IT.txt
```

### 分析

此結果顯示系統中存在 `Flag.txt.WINDOWS.lnk` 的 Recent 捷徑，代表使用者 Rick 曾經開啟或存取過 `Flag.txt.WINDOWS`。

另外，`READ_IT.txt` 位於 Rick 的 Desktop，可能是提示檔、說明檔或攻擊後留下的文字檔。

### 判斷

```text
Flag.txt.WINDOWS.lnk 顯示 Flag 檔案曾被使用者開啟。
READ_IT.txt 是需要優先 dump 的重要文字檔。
```

---

## 5. Rick And Morty 可疑執行檔

### 執行指令

```bash
.\vol.exe -f .\OtterCTF.vmem windows.filescan.FileScan | findstr "Rick Morty download.exe"
```

### 重要結果

```text
0x7d63dbc0  \Torrents\Rick And Morty season 1 download.exe
```
```
D:\Forensic\G140A006\VolatilityWorkbench>.\vol.exe -f .\OtterCTF.vmem windows.filescan.FileScan | findstr 0x7d63dbc0
0x7d63dbc0 100.0\Torrents\Rick And Morty season 1 download.exe  216
```

### 分析

`Rick And Morty season 1 download.exe` 位於 `\Torrents` 目錄，檔名看起來像影片下載，但副檔名為 `.exe`。

這符合常見偽裝手法：利用影片名稱吸引使用者執行惡意程式。

### 判斷

```text
Rick And Morty season 1 download.exe 是本案主要可疑執行檔。
```

---

## 6. BitTorrent 相關痕跡

### 執行指令

```bash
.\vol.exe -f .\OtterCTF.vmem windows.filescan.FileScan | findstr "torrent BitTorrent"
```

### 重要結果

```text
\Users\Rick\AppData\Roaming\BitTorrent\dlimagecache\165F6EF40A81DD175FFAEA69E77ABFD30B27E71C
\Users\Rick\AppData\Roaming\BitTorrent\updates\7.10.3_44495\bittorrentie.exe
\Users\Rick\AppData\LocalLow\BitTorrent\BitTorrent_2836_00313D08_590648902
\Users\Rick\AppData\LocalLow\BitTorrent\BitTorrent_2836_00313978_1933444659
```

### 分析

系統中有多個 BitTorrent 相關檔案與暫存資料，代表使用者 Rick 當時有使用 BitTorrent。

前面 `NetScan` 也顯示 `BitTorrent.exe` 有大量 P2P 連線，因此可推論可疑檔案可能與 Torrent 下載活動有關。

### 判斷

```text
BitTorrent 活動與 \Torrents\Rick And Morty season 1 download.exe 具有關聯性。
```

---

## 7. 重要證據整理

| 類別         |       Offset | 檔案路徑                                                                           | 判斷            |
| ---------- | -----------: | ------------------------------------------------------------------------------ | ------------- |
| Flag 線索    | `0x7d61b070` | `\Users\Rick\AppData\Roaming\Microsoft\Windows\Recent\Flag.txt.WINDOWS.lnk`    | Flag 曾被開啟     |
| 提示檔        | `0x7d660500` | `\Users\Rick\Desktop\READ_IT.txt`                                              | 優先 dump       |
| 可疑 EXE     | `0x7d63dbc0` | `\Torrents\Rick And Morty season 1 download.exe`                               | 主要可疑檔案        |
| Torrent 痕跡 | `0x7d69ade0` | `\Users\Rick\AppData\Roaming\BitTorrent\updates\7.10.3_44495\bittorrentie.exe` | BitTorrent 相關 |
| Torrent 暫存 | `0x7d679070` | `\Users\Rick\AppData\LocalLow\BitTorrent\BitTorrent_2836_00313D08_590648902`   | P2P 使用痕跡      |

---

## 8. 建議 Dump 順序

依照鑑識價值，建議優先 dump：

```text
1. \Users\Rick\Desktop\READ_IT.txt
2. \Users\Rick\AppData\Roaming\Microsoft\Windows\Recent\Flag.txt.WINDOWS.lnk
3. \Torrents\Rick And Morty season 1 download.exe
```

### Dump 指令

```bash
mkdir dump
```

Dump `READ_IT.txt`：

```bash
.\vol.exe -f .\OtterCTF.vmem -o dump windows.dumpfiles.DumpFiles --virtaddr 0x7d660500
```

Dump `Flag.txt.WINDOWS.lnk`：

```bash
.\vol.exe -f .\OtterCTF.vmem -o dump windows.dumpfiles.DumpFiles --virtaddr 0x7d61b070
```

Dump `Rick And Morty season 1 download.exe`：

```bash
.\vol.exe -f .\OtterCTF.vmem -o dump windows.dumpfiles.DumpFiles --virtaddr 0x7d63dbc0
```
