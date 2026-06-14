# 測試內容
- vol.exe -f .\OtterCTF.vmem windows.cmdline.CmdLine

```
D:\Forensic\G140A006\VolatilityWorkbench>.\vol.exe -f .\OtterCTF.vmem windows.cmdline.CmdLine
Volatility 3 Framework 2.5.0
Progress:  100.00               PDB scanning finished
PID     Process Args

4       System  Required memory at 0x20 is not valid (process exited?)
260     smss.exe        \SystemRoot\System32\smss.exe
348     csrss.exe       %SystemRoot%\system32\csrss.exe ObjectDirectory=\Windows SharedSection=1024,20480,768 Windows=On SubSystemType=Windows ServerDll=basesrv,1 ServerDll=winsrv:UserServerDllInitialization,3 ServerDll=winsrv:ConServerDllInitialization,2 ServerDll=sxssrv,4 ProfileControl=Off MaxRequestThreads=16
388     csrss.exe       %SystemRoot%\system32\csrss.exe ObjectDirectory=\Windows SharedSection=1024,20480,768 Windows=On SubSystemType=Windows ServerDll=basesrv,1 ServerDll=winsrv:UserServerDllInitialization,3 ServerDll=winsrv:ConServerDllInitialization,2 ServerDll=sxssrv,4 ProfileControl=Off MaxRequestThreads=16
396     wininit.exe     wininit.exe
432     winlogon.exe    winlogon.exe
492     services.exe    C:\Windows\system32\services.exe
500     lsass.exe       C:\Windows\system32\lsass.exe
508     lsm.exe C:\Windows\system32\lsm.exe
604     svchost.exe     C:\Windows\system32\svchost.exe -k DcomLaunch
668     vmacthlp.exe    "C:\Program Files\VMware\VMware Tools\vmacthlp.exe"
712     svchost.exe     C:\Windows\system32\svchost.exe -k RPCSS
808     svchost.exe     C:\Windows\System32\svchost.exe -k LocalServiceNetworkRestricted
844     svchost.exe     C:\Windows\System32\svchost.exe -k LocalSystemNetworkRestricted
868     svchost.exe     C:\Windows\system32\svchost.exe -k netsvcs
960     audiodg.exe     C:\Windows\system32\AUDIODG.EXE 0x2fc
1012    svchost.exe     C:\Windows\system32\svchost.exe -k LocalService
620     svchost.exe     C:\Windows\system32\svchost.exe -k NetworkService
1120    spoolsv.exe     C:\Windows\System32\spoolsv.exe
1164    svchost.exe     C:\Windows\system32\svchost.exe -k LocalServiceNoNetwork
1356    VGAuthService.  "C:\Program Files\VMware\VMware Tools\VMware VGAuth\VGAuthService.exe"
1428    vmtoolsd.exe    "C:\Program Files\VMware\VMware Tools\vmtoolsd.exe"
1800    WmiPrvSE.exe    C:\Windows\system32\wbem\wmiprvse.exe
1948    svchost.exe     C:\Windows\system32\svchost.exe -k bthsvcs
1324    dllhost.exe     C:\Windows\system32\dllhost.exe /Processid:{02D4B3F1-FD88-11D1-960D-00805FC79235}
1436    msdtc.exe       C:\Windows\System32\msdtc.exe
2136    WmiPrvSE.exe    C:\Windows\system32\wbem\wmiprvse.exe
2344    taskhost.exe    "taskhost.exe"
2500    sppsvc.exe      C:\Windows\system32\sppsvc.exe
2704    dwm.exe "C:\Windows\system32\Dwm.exe"
2728    explorer.exe    C:\Windows\Explorer.EXE
2804    vmtoolsd.exe    "C:\Program Files\VMware\VMware Tools\vmtoolsd.exe" -n vmusr
2836    BitTorrent.exe  "C:\Users\Rick\AppData\Roaming\BitTorrent\BitTorrent.exe"  /MINIMIZED
2844    WebCompanion.e  Required memory at 0x7efdf020 is not valid (process exited?)
3064    SearchIndexer.  C:\Windows\system32\SearchIndexer.exe /Embedding
2308    bittorrentie.e  "C:\Users\Rick\AppData\Roaming\BitTorrent\updates\7.10.3_44495\bittorrentie.exe" BitTorrent_2836_00313D08_590648902 BT4823DF041B09 BitTorrent
2624    bittorrentie.e  "C:\Users\Rick\AppData\Roaming\BitTorrent\updates\7.10.3_44495\bittorrentie.exe" BitTorrent_2836_00313978_1933444659 BT4823DF041B09 BitTorrent
708     LunarMS.exe     "C:\Nexon\MapleStory\LunarMS.exe"
724     PresentationFo  C:\Windows\Microsoft.Net\Framework64\v3.0\WPF\PresentationFontCache.exe
412     mscorsvw.exe    C:\Windows\Microsoft.NET\Framework\v4.0.30319\mscorsvw.exe
164     svchost.exe     C:\Windows\system32\svchost.exe -k LocalServiceAndNoImpersonation
3124    mscorsvw.exe    C:\Windows\Microsoft.NET\Framework64\v4.0.30319\mscorsvw.exe
3196    svchost.exe     C:\Windows\System32\svchost.exe -k secsvcs
4076    chrome.exe      "C:\Program Files (x86)\Google\Chrome\Application\chrome.exe"
4084    chrome.exe      "C:\Program Files (x86)\Google\Chrome\Application\chrome.exe" --type=crashpad-handler "--user-data-dir=C:\Users\Rick\AppData\Local\Google\Chrome\User Data" /prefetch:7 --monitor-self-annotation=ptype=crashpad-handler "--database=C:\Users\Rick\AppData\Local\Google\Chrome\User Data\Crashpad" "--metrics-dir=C:\Users\Rick\AppData\Local\Google\Chrome\User Data" --url=https://clients2.google.com/cr/report --annotation=channel= --annotation=plat=Win64 --annotation=prod=Chrome --annotation=ver=68.0.3440.84 --initial-client-data=0x7c,0x80,0x84,0x78,0x88,0x7feeb3324d0,0x7feeb3324e0,0x7feeb3324f0
576     chrome.exe      "C:\Program Files (x86)\Google\Chrome\Application\chrome.exe" --type=watcher --main-thread-id=4080 --on-initialized-event-handle=304 --parent-handle=308 /prefetch:6
1808    chrome.exe      "C:\Program Files (x86)\Google\Chrome\Application\chrome.exe" --type=gpu-process --field-trial-handle=984,15358569600588498425,3475374789430647391,131072 --gpu-preferences=KAAAAAAAAACAAwBAAQAAAAAAAAAAAGAAEAAAAAAAAAAAAAAAAAAAACgAAAAEAAAAIAAAAAAAAAAoAAAAAAAAADAAAAAAAAAAOAAAAAAAAAAQAAAAAAAAAAAAAAAKAAAAEAAAAAAAAAAAAAAACwAAABAAAAAAAAAAAQAAAAoAAAAQAAAAAAAAAAEAAAALAAAA --service-request-channel-token=4939AD179421E7F7FF934CA7C25FCD34 --mojo-platform-channel-handle=1004 --ignored=" --type=renderer " /prefetch:2
3924    chrome.exe      "C:\Program Files (x86)\Google\Chrome\Application\chrome.exe" --type=renderer --field-trial-handle=984,15358569600588498425,3475374789430647391,131072 --service-pipe-token=BB216EAECD5332095D1836CB17604E02 --lang=en-US --enable-offline-auto-reload --enable-offline-auto-reload-visible-only --device-scale-factor=1 --num-raster-threads=1 --service-request-channel-token=BB216EAECD5332095D1836CB17604E02 --renderer-client-id=9 --mojo-platform-channel-handle=2440 /prefetch:1
2748    chrome.exe      "C:\Program Files (x86)\Google\Chrome\Application\chrome.exe" --type=renderer --field-trial-handle=984,15358569600588498425,3475374789430647391,131072 --service-pipe-token=5B96B12CED256E93CD66ABC8626426FB --lang=en-US --enable-offline-auto-reload --enable-offline-auto-reload-visible-only --device-scale-factor=1 --num-raster-threads=1 --service-request-channel-token=5B96B12CED256E93CD66ABC8626426FB --renderer-client-id=22 --mojo-platform-channel-handle=2104 /prefetch:1
3820    Rick And Morty  "C:\Torrents\Rick And Morty season 1 download.exe"
3720    vmware-tray.ex  "C:\Users\Rick\AppData\Local\Temp\RarSFX0\vmware-tray.exe"
3880    WebCompanionIn  "C:\Program Files (x86)\Lavasoft\Web Companion\Application\WebCompanionInstaller.exe" --update --prod --partner=BT170701 --version=4.3.1908.3686
3648    chrome.exe      "C:\Program Files (x86)\Google\Chrome\Application\chrome.exe" --type=renderer --field-trial-handle=984,15358569600588498425,3475374789430647391,131072 --service-pipe-token=66BB0CC3FE10242BC701AB87A5940738 --lang=en-US --enable-offline-auto-reload --enable-offline-auto-reload-visible-only --device-scale-factor=1 --num-raster-threads=1 --service-request-channel-token=66BB0CC3FE10242BC701AB87A5940738 --renderer-client-id=30 --mojo-platform-channel-handle=4516 /prefetch:1
1796    chrome.exe      "C:\Program Files (x86)\Google\Chrome\Application\chrome.exe" --type=renderer --field-trial-handle=984,15358569600588498425,3475374789430647391,131072 --service-pipe-token=86C637812F74263DD98834CC0FE01CE7 --lang=en-US --enable-offline-auto-reload --enable-offline-auto-reload-visible-only --device-scale-factor=1 --num-raster-threads=1 --service-request-channel-token=86C637812F74263DD98834CC0FE01CE7 --renderer-client-id=31 --mojo-platform-channel-handle=4412 /prefetch:1
3208    sc.exe  Required memory at 0x7efdf020 is not valid (process exited?)
452     sc.exe  Required memory at 0x7efdf020 is not valid (process exited?)
3504    sc.exe  Required memory at 0x7efdf020 is not valid (process exited?)
2028    sc.exe  Required memory at 0x7efdf020 is not valid (process exited?)
3496    Lavasoft.WCAss  "C:\Program Files (x86)\Lavasoft\Web Companion\Application\Lavasoft.WCAssistant.WinService.exe"
3856    WebCompanion.e  "C:\Program Files (x86)\Lavasoft\Web Companion\Application\WebCompanion.exe" --silent --update
3304    notepad.exe     "C:\Windows\system32\NOTEPAD.EXE" C:\Users\Rick\Desktop\Flag.txt.WINDOWS
3916    cmd.exe Required memory at 0x7fffffdd020 is not valid (process exited?)
2420    conhost.exe     \??\C:\Windows\system32\conhost.exe
```


# windows.cmdline.CmdLine 分析

## 1. 執行指令

```bash
.\vol.exe -f .\OtterCTF.vmem windows.cmdline.CmdLine
```

---

## 2. Plugin 功能簡述

`windows.cmdline.CmdLine` 用來顯示 Process 的完整執行命令與路徑。

它可以協助確認：

* 程式從哪個路徑執行
* 是否有可疑參數
* 可疑 Process 是否由使用者執行
* 短時間執行的程式是否留下命令列紀錄

此 Plugin 通常會搭配 `pslist`、`pstree`、`psscan` 一起分析。

---

## 3. 重要結果整理

|                      PID | Process                               | Command Line / Path                                                                                                                              | 判斷                         |
| -----------------------: | ------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------ | -------------------------- |
|                     2836 | `BitTorrent.exe`                      | `C:\Users\Rick\AppData\Roaming\BitTorrent\BitTorrent.exe /MINIMIZED`                                                                             | P2P 下載軟體                   |
|                     2308 | `bittorrentie.exe`                    | `C:\Users\Rick\AppData\Roaming\BitTorrent\updates\7.10.3_44495\bittorrentie.exe`                                                                 | BitTorrent 子行程             |
|                     2624 | `bittorrentie.exe`                    | `C:\Users\Rick\AppData\Roaming\BitTorrent\updates\7.10.3_44495\bittorrentie.exe`                                                                 | BitTorrent 子行程             |
|                      708 | `LunarMS.exe`                         | `C:\Nexon\MapleStory\LunarMS.exe`                                                                                                                | 遊戲相關程式，仍需確認                |
|                     3820 | `Rick And Morty`                      | `C:\Torrents\Rick And Morty season 1 download.exe`                                                                                               | 高度可疑                       |
|                     3720 | `vmware-tray.exe`                     | `C:\Users\Rick\AppData\Local\Temp\RarSFX0\vmware-tray.exe`                                                                                       | 可疑，從 Temp/RarSFX 執行        |
|                     3880 | `WebCompanionInstaller.exe`           | `C:\Program Files (x86)\Lavasoft\Web Companion\Application\WebCompanionInstaller.exe --update --prod --partner=BT170701 --version=4.3.1908.3686` | WebCompanion 安裝/更新行為       |
|                     3496 | `Lavasoft.WCAssistant.WinService.exe` | `C:\Program Files (x86)\Lavasoft\Web Companion\Application\Lavasoft.WCAssistant.WinService.exe`                                                  | WebCompanion 服務            |
|                     3856 | `WebCompanion.exe`                    | `C:\Program Files (x86)\Lavasoft\Web Companion\Application\WebCompanion.exe --silent --update`                                                   | 靜默更新                       |
|                     3304 | `notepad.exe`                         | `C:\Windows\system32\NOTEPAD.EXE C:\Users\Rick\Desktop\Flag.txt.WINDOWS`                                                                         | 重要線索                       |
|                     3916 | `cmd.exe`                             | `Required memory ... is not valid`                                                                                                               | Process 已結束，無法取得完整命令       |
| 3208 / 452 / 3504 / 2028 | `sc.exe`                              | `Required memory ... is not valid`                                                                                                               | Process 已結束，需用其他 Plugin 補充 |

---

## 4. 關鍵發現

### 4.1 可疑下載檔案

```text
PID 3820
Process: Rick And Morty
Path: C:\Torrents\Rick And Morty season 1 download.exe
```

這是本次 `cmdline` 最重要的發現。

原因：

* 檔案位於 `C:\Torrents`
* 檔名偽裝成影片下載
* 副檔名是 `.exe`
* 與前面 `BitTorrent.exe` 的存在互相呼應

判斷：

```text
Rick And Morty season 1 download.exe 很可能是使用者透過 torrent 下載並執行的可疑程式。
```

---

### 4.2 BitTorrent 下載活動

```text
C:\Users\Rick\AppData\Roaming\BitTorrent\BitTorrent.exe
```

系統中存在 BitTorrent 主程式與子行程：

```text
BitTorrent.exe
bittorrentie.exe
bittorrentie.exe
```

這代表主機可能有 P2P 下載活動。

搭配 `Rick And Morty season 1 download.exe` 的路徑，可以推測可疑檔案可能與 torrent 下載有關。

---

### 4.3 可疑 Temp 執行檔

```text
C:\Users\Rick\AppData\Local\Temp\RarSFX0\vmware-tray.exe
```

`vmware-tray.exe` 從 `Temp\RarSFX0` 執行，這點可疑。

原因：

* 正常 VMware 程式通常不應該從使用者 Temp 目錄執行
* `RarSFX0` 通常與 WinRAR 自解壓檔有關
* 可能是某個壓縮檔或自解壓程式釋放出的檔案

此行程在前面的 `pstree` 中是 `Rick And Morty` 的子行程，因此關聯性很高。

重要關係：

```text
Rick And Morty → vmware-tray.exe
```

---

### 4.4 WebCompanion / Lavasoft 行為

```text
WebCompanionInstaller.exe --update --prod --partner=BT170701
WebCompanion.exe --silent --update
Lavasoft.WCAssistant.WinService.exe
```

這代表系統中存在 Lavasoft Web Companion 相關程式。

重點：

* 有安裝或更新行為
* 有靜默更新參數 `--silent --update`
* 有 Windows Service 元件
* 前面 `pstree` 顯示它曾啟動多個 `sc.exe`

判斷：

```text
WebCompanion 可能正在執行安裝、更新或服務操作，需搭配 svcscan 確認服務狀態。
```

---

### 4.5 Flag 檔案線索

```text
notepad.exe C:\Users\Rick\Desktop\Flag.txt.WINDOWS
```

這是非常重要的 CTF 線索。

代表使用者曾經用 Notepad 開啟：

```text
C:\Users\Rick\Desktop\Flag.txt.WINDOWS
```

判斷：

```text
Flag.txt.WINDOWS 很可能是本題重要目標檔案。
```

後續可嘗試透過檔案掃描或 dump 方式找出該檔案內容。

建議指令：

```bash
.\vol.exe -f .\OtterCTF.vmem windows.filescan.FileScan
```

可搭配關鍵字尋找：

```text
Flag.txt.WINDOWS
```

---

## 5. 已結束 Process 的情況

本次有些 Process 顯示：

```text
Required memory at 0x7efdf020 is not valid (process exited?)
```

例如：

```text
WebCompanion.e
sc.exe
cmd.exe
```

意思是這些 Process 可能已經結束，Volatility 無法再從記憶體中取得完整命令列內容。

這不代表錯誤，也不代表檔案壞掉，只是該 Process 的部分記憶體資料已經不可讀。

---

## 6. 本次 CmdLine 鑑識重點

本次 `cmdline` 最重要的發現如下：

1. `Rick And Morty` 的實際路徑是：

   ```text
   C:\Torrents\Rick And Morty season 1 download.exe
   ```

2. 可疑程式是 `.exe`，但檔名偽裝成影片下載。

3. 系統中存在 BitTorrent，可能與可疑檔案下載有關。

4. `Rick And Morty` 啟動了：

   ```text
   C:\Users\Rick\AppData\Local\Temp\RarSFX0\vmware-tray.exe
   ```

5. `notepad.exe` 開啟了：

   ```text
   C:\Users\Rick\Desktop\Flag.txt.WINDOWS
   ```

6. WebCompanion 有安裝、更新與服務相關行為。

---

## 7. 後續建議分析

### 7.1 分析可疑程式 DLL

```bash
.\vol.exe -f .\OtterCTF.vmem windows.dlllist.DllList --pid 3820
```

### 7.2 檢查是否有程式碼注入

```bash
.\vol.exe -f .\OtterCTF.vmem windows.malfind.Malfind --pid 3820
```

### 7.3 分析可疑子行程

```bash
.\vol.exe -f .\OtterCTF.vmem windows.dlllist.DllList --pid 3720
.\vol.exe -f .\OtterCTF.vmem windows.malfind.Malfind --pid 3720
```

### 7.4 搜尋 Flag 檔案

```bash
.\vol.exe -f .\OtterCTF.vmem windows.filescan.FileScan
```

搜尋關鍵字：

```text
Flag.txt.WINDOWS
```

### 7.5 分析網路連線

```bash
.\vol.exe -f .\OtterCTF.vmem windows.netscan.NetScan
```

---

## 8. 報告用結論

本次使用 `windows.cmdline.CmdLine` 分析 Process 的完整執行命令與路徑。

分析結果顯示，最重要的可疑程式是：

```text
C:\Torrents\Rick And Morty season 1 download.exe
```

該檔案名稱偽裝成影片下載，但實際上是 `.exe` 執行檔，且系統中同時存在 BitTorrent 下載軟體，因此推測此可疑程式可能與 torrent 下載活動有關。

此外，`Rick And Morty` 啟動了位於 Temp 目錄的：

```text
C:\Users\Rick\AppData\Local\Temp\RarSFX0\vmware-tray.exe
```

此路徑不屬於正常 VMware 安裝位置，具有可疑性。

另外，`notepad.exe` 開啟了：

```text
C:\Users\Rick\Desktop\Flag.txt.WINDOWS
```

這是本次分析中的重要 CTF 線索，後續應透過 `filescan` 或其他檔案分析方式尋找該檔案內容。

綜合判斷，本次 `cmdline` 分析確認了可疑程式來源、執行路徑與重要 Flag 檔案線索。後續應優先分析 `Rick And Morty`、`vmware-tray.exe`、`Flag.txt.WINDOWS` 與相關網路連線。

---

## 9. 簡短結論

`cmdline` 顯示本次最重要的可疑執行檔為：

```text
C:\Torrents\Rick And Morty season 1 download.exe
```

此檔案偽裝成影片下載，但實際為 `.exe`，高度可疑。

另一個重要線索是：

```text
C:\Users\Rick\Desktop\Flag.txt.WINDOWS
```

該檔案曾被 Notepad 開啟，可能是本題的 Flag 相關檔案。

後續建議優先分析：

```text
PID 3820 - Rick And Morty
PID 3720 - vmware-tray.exe
Flag.txt.WINDOWS
netscan 網路連線
```
