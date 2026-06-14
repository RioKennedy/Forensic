# 測試內容
- vol.exe -f .\OtterCTF.vmem windows.pslist.PsList

```
D:\Forensic\G140A006\VolatilityWorkbench>.\vol.exe -f .\OtterCTF.vmem windows.pslist.PsList
Volatility 3 Framework 2.5.0
Progress:  100.00               PDB scanning finished
PID     PPID    ImageFileName   Offset(V)       Threads Handles SessionId       Wow64   CreateTime      ExitTime       File output

4       0       System  0xfa8018d44740  95      411     N/A     False   2018-08-04 19:26:03.000000      N/A     Disabled
260     4       smss.exe        0xfa801947e4d0  2       30      N/A     False   2018-08-04 19:26:03.000000      N/A    Disabled
348     336     csrss.exe       0xfa801a0c8380  9       563     0       False   2018-08-04 19:26:10.000000      N/A    Disabled
388     380     csrss.exe       0xfa80198d3b30  11      460     1       False   2018-08-04 19:26:11.000000      N/A    Disabled
396     336     wininit.exe     0xfa801a2ed060  3       78      0       False   2018-08-04 19:26:11.000000      N/A    Disabled
432     380     winlogon.exe    0xfa801aaf4060  3       113     1       False   2018-08-04 19:26:11.000000      N/A    Disabled
492     396     services.exe    0xfa801ab377c0  11      242     0       False   2018-08-04 19:26:12.000000      N/A    Disabled
500     396     lsass.exe       0xfa801ab3f060  7       610     0       False   2018-08-04 19:26:12.000000      N/A    Disabled
508     396     lsm.exe 0xfa801ab461a0  10      148     0       False   2018-08-04 19:26:12.000000      N/A     Disabled
604     492     svchost.exe     0xfa8018e3c890  11      376     0       False   2018-08-04 19:26:16.000000      N/A    Disabled
668     492     vmacthlp.exe    0xfa801abbdb30  3       56      0       False   2018-08-04 19:26:16.000000      N/A    Disabled
712     492     svchost.exe     0xfa801abebb30  8       301     0       False   2018-08-04 19:26:17.000000      N/A    Disabled
808     492     svchost.exe     0xfa801ac2e9e0  22      508     0       False   2018-08-04 19:26:18.000000      N/A    Disabled
844     492     svchost.exe     0xfa801ac31b30  17      396     0       False   2018-08-04 19:26:18.000000      N/A    Disabled
868     492     svchost.exe     0xfa801ac4db30  45      1114    0       False   2018-08-04 19:26:18.000000      N/A    Disabled
960     808     audiodg.exe     0xfa801ac753a0  7       151     0       False   2018-08-04 19:26:19.000000      N/A    Disabled
1012    492     svchost.exe     0xfa801ac97060  12      554     0       False   2018-08-04 19:26:20.000000      N/A    Disabled
620     492     svchost.exe     0xfa801acd37e0  19      415     0       False   2018-08-04 19:26:21.000000      N/A    Disabled
1120    492     spoolsv.exe     0xfa801ad5ab30  14      346     0       False   2018-08-04 19:26:22.000000      N/A    Disabled
1164    492     svchost.exe     0xfa801ad718a0  18      312     0       False   2018-08-04 19:26:23.000000      N/A    Disabled
1356    492     VGAuthService.  0xfa801ae0f630  3       85      0       False   2018-08-04 19:26:25.000000      N/A    Disabled
1428    492     vmtoolsd.exe    0xfa801ae92920  9       313     0       False   2018-08-04 19:26:27.000000      N/A    Disabled
1800    604     WmiPrvSE.exe    0xfa8019124b30  9       222     0       False   2018-08-04 19:26:39.000000      N/A    Disabled
1948    492     svchost.exe     0xfa801afe7800  6       96      0       False   2018-08-04 19:26:42.000000      N/A    Disabled
1324    492     dllhost.exe     0xfa801ae7f630  15      207     0       False   2018-08-04 19:26:42.000000      N/A    Disabled
1436    492     msdtc.exe       0xfa801aff3b30  14      155     0       False   2018-08-04 19:26:43.000000      N/A    Disabled
2136    604     WmiPrvSE.exe    0xfa801b112060  12      324     0       False   2018-08-04 19:26:51.000000      N/A    Disabled
2344    492     taskhost.exe    0xfa801b1e9b30  8       193     1       False   2018-08-04 19:26:57.000000      N/A    Disabled
2500    492     sppsvc.exe      0xfa801b232060  4       149     0       False   2018-08-04 19:26:58.000000      N/A    Disabled
2704    844     dwm.exe 0xfa801b1fab30  4       97      1       False   2018-08-04 19:27:04.000000      N/A     Disabled
2728    2696    explorer.exe    0xfa801b27e060  33      854     1       False   2018-08-04 19:27:04.000000      N/A    Disabled
2804    2728    vmtoolsd.exe    0xfa801b1cdb30  6       190     1       False   2018-08-04 19:27:06.000000      N/A    Disabled
2836    2728    BitTorrent.exe  0xfa801b290b30  24      471     1       True    2018-08-04 19:27:07.000000      N/A    Disabled
2844    2728    WebCompanion.e  0xfa801b2f02e0  0       -       1       False   2018-08-04 19:27:07.000000      2018-08-04 19:33:33.000000      Disabled
3064    492     SearchIndexer.  0xfa801b3aab30  11      610     0       False   2018-08-04 19:27:14.000000      N/A    Disabled
2308    2836    bittorrentie.e  0xfa801b4a7b30  15      337     1       True    2018-08-04 19:27:19.000000      N/A    Disabled
2624    2836    bittorrentie.e  0xfa801b4c9b30  13      316     1       True    2018-08-04 19:27:21.000000      N/A    Disabled
708     2728    LunarMS.exe     0xfa801b5cb740  18      346     1       True    2018-08-04 19:27:39.000000      N/A    Disabled
724     492     PresentationFo  0xfa801988c2d0  6       148     0       False   2018-08-04 19:27:52.000000      N/A    Disabled
412     492     mscorsvw.exe    0xfa801b603610  7       86      0       True    2018-08-04 19:28:42.000000      N/A    Disabled
164     492     svchost.exe     0xfa801a6af9f0  12      147     0       False   2018-08-04 19:28:42.000000      N/A    Disabled
3124    492     mscorsvw.exe    0xfa801a6c2700  7       77      0       False   2018-08-04 19:28:43.000000      N/A    Disabled
3196    492     svchost.exe     0xfa801a6e4b30  14      352     0       False   2018-08-04 19:28:44.000000      N/A    Disabled
4076    2728    chrome.exe      0xfa801a4e3870  44      1160    1       False   2018-08-04 19:29:30.000000      N/A    Disabled
4084    4076    chrome.exe      0xfa801a4eab30  8       86      1       False   2018-08-04 19:29:30.000000      N/A    Disabled
576     4076    chrome.exe      0xfa801a502b30  2       58      1       False   2018-08-04 19:29:31.000000      N/A    Disabled
1808    4076    chrome.exe      0xfa801a4f7b30  13      229     1       False   2018-08-04 19:29:32.000000      N/A    Disabled
3924    4076    chrome.exe      0xfa801aa00a90  16      228     1       False   2018-08-04 19:29:51.000000      N/A    Disabled
2748    4076    chrome.exe      0xfa801a7f98f0  15      181     1       False   2018-08-04 19:31:15.000000      N/A    Disabled
3820    2728    Rick And Morty  0xfa801b486b30  4       185     1       True    2018-08-04 19:32:55.000000      N/A    Disabled
3720    3820    vmware-tray.ex  0xfa801a4c5b30  8       147     1       True    2018-08-04 19:33:02.000000      N/A    Disabled
3880    1484    WebCompanionIn  0xfa801b18f060  15      522     0       True    2018-08-04 19:33:07.000000      N/A    Disabled
3648    4076    chrome.exe      0xfa801a635240  16      207     1       False   2018-08-04 19:33:38.000000      N/A    Disabled
1796    4076    chrome.exe      0xfa801a5ef1f0  15      170     1       False   2018-08-04 19:33:41.000000      N/A    Disabled
3208    3880    sc.exe  0xfa801b08f060  0       -       0       False   2018-08-04 19:33:47.000000      2018-08-04 19:33:48.000000      Disabled
452     3880    sc.exe  0xfa801aeb6890  0       -       0       False   2018-08-04 19:33:48.000000      2018-08-04 19:33:48.000000      Disabled
3504    3880    sc.exe  0xfa801aa72b30  0       -       0       False   2018-08-04 19:33:48.000000      2018-08-04 19:33:48.000000      Disabled
2028    3880    sc.exe  0xfa801ac01060  0       -       0       False   2018-08-04 19:33:49.000000      2018-08-04 19:34:03.000000      Disabled
3496    492     Lavasoft.WCAss  0xfa801aad1060  14      473     0       False   2018-08-04 19:33:49.000000      N/A    Disabled
3856    3880    WebCompanion.e  0xfa801a6268b0  15      386     0       True    2018-08-04 19:34:05.000000      N/A    Disabled
3304    3132    notepad.exe     0xfa801b1fd960  2       79      1       False   2018-08-04 19:34:10.000000      N/A    Disabled
3916    1428    cmd.exe 0xfa801a572b30  0       -       0       False   2018-08-04 19:34:22.000000      2018-08-04 19:34:22.000000      Disabled
2420    348     conhost.exe     0xfa801a6643d0  0       30      0       False   2018-08-04 19:34:22.000000      2018-08-04 19:34:22.000000      Disabled
```


# windows.pslist.PsList 分析

## 1. 執行指令

```bash
.\vol.exe -f .\OtterCTF.vmem windows.pslist.PsList
```

---

## 2. Plugin 功能說明

`windows.pslist.PsList` 是 Volatility 3 中用來列出 Windows 記憶體映像檔中正在執行或仍存在於 Active Process List 中的 Process。

它可以顯示：

* PID
* PPID
* Process Name
* Process 建立時間
* Process 結束時間
* Thread 數量
* Handle 數量
* Session ID
* 是否為 Wow64 程序

在 Windows 記憶體鑑識中，`pslist` 是非常重要的基礎 Plugin。
它通常是行程分析的第一步，用來了解系統中有哪些 Process，以及哪些 Process 可能可疑。

---

## 3. 執行結果摘要

本次 `windows.pslist.PsList` 成功列出系統中的 Process。

從結果可以判斷，此記憶體映像檔擷取時，系統中包含一般 Windows 系統行程、VMware 相關行程、瀏覽器行程，以及數個可疑或需要進一步分析的行程。

---

## 4. 系統基本行程分析

以下為正常 Windows 開機後常見的系統行程：

| PID | PPID | Process      | 說明                            |
| --: | ---: | ------------ | ----------------------------- |
|   4 |    0 | System       | Windows 系統核心行程                |
| 260 |    4 | smss.exe     | Session Manager               |
| 348 |  336 | csrss.exe    | Client Server Runtime Process |
| 388 |  380 | csrss.exe    | 使用者 Session 的 csrss           |
| 396 |  336 | wininit.exe  | Windows 初始化行程                 |
| 432 |  380 | winlogon.exe | 使用者登入管理                       |
| 492 |  396 | services.exe | 服務管理行程                        |
| 500 |  396 | lsass.exe    | Local Security Authority      |
| 508 |  396 | lsm.exe      | Local Session Manager         |

這些行程大多是 Windows 7 系統正常啟動時會出現的 Process。

---

## 5. 重要正常行程說明

### 5.1 System

```text
PID: 4
PPID: 0
ImageFileName: System
CreateTime: 2018-08-04 19:26:03
```

`System` 是 Windows Kernel 的核心行程，PID 通常固定為 4。
本次結果中 PID 4 正常，沒有明顯異常。

---

### 5.2 smss.exe

```text
PID: 260
PPID: 4
ImageFileName: smss.exe
CreateTime: 2018-08-04 19:26:03
```

`smss.exe` 是 Session Manager Subsystem，通常由 `System` 建立。
本次結果中 `smss.exe` 的 PPID 為 4，符合正常父子關係。

---

### 5.3 wininit.exe、services.exe、lsass.exe

```text
wininit.exe  PID 396
services.exe PID 492
lsass.exe    PID 500
```

`wininit.exe` 是 Windows 初始化行程。
`services.exe` 負責管理 Windows Service。
`lsass.exe` 負責帳號驗證與安全性相關功能。

本次結果中：

| Process      | PID | PPID |
| ------------ | --: | ---: |
| wininit.exe  | 396 |  336 |
| services.exe | 492 |  396 |
| lsass.exe    | 500 |  396 |

這些關係大致符合 Windows 正常開機流程。

---

## 6. VMware 相關行程

本次結果中出現多個 VMware 相關行程：

|  PID | PPID | Process        | 說明                   |
| ---: | ---: | -------------- | -------------------- |
|  668 |  492 | vmacthlp.exe   | VMware Tools 相關服務    |
| 1428 |  492 | vmtoolsd.exe   | VMware Tools Service |
| 2804 | 2728 | vmtoolsd.exe   | 使用者層 VMware Tools    |
| 3720 | 3820 | vmware-tray.ex | VMware Tray 程式       |

這代表此記憶體映像檔很可能來自 VMware 虛擬機器環境。
這與檔案名稱 `OtterCTF.vmem` 也相符，`.vmem` 通常是 VMware 的記憶體映像檔格式。

---

## 7. 使用者層行程分析

### 7.1 explorer.exe

```text
PID: 2728
PPID: 2696
ImageFileName: explorer.exe
CreateTime: 2018-08-04 19:27:04
```

`explorer.exe` 是 Windows 使用者桌面與檔案總管行程。
大部分使用者開啟的程式都可能由 `explorer.exe` 啟動。

本次結果中，多個應用程式是由 `explorer.exe` 啟動，例如：

|  PID | Process        |
| ---: | -------------- |
| 2836 | BitTorrent.exe |
| 2844 | WebCompanion.e |
|  708 | LunarMS.exe    |
| 4076 | chrome.exe     |
| 3820 | Rick And Morty |

這些行程都需要進一步注意，因為它們屬於使用者層執行的程式。

---

## 8. 可疑或需要注意的行程

本次 `pslist` 結果中，以下行程較值得關注：

|  PID | PPID | Process        | 原因                           |
| ---: | ---: | -------------- | ---------------------------- |
| 2836 | 2728 | BitTorrent.exe | P2P 軟體，可能涉及下載可疑檔案            |
| 2308 | 2836 | bittorrentie.e | BitTorrent 子行程               |
| 2624 | 2836 | bittorrentie.e | BitTorrent 子行程               |
|  708 | 2728 | LunarMS.exe    | 非系統常見行程，需進一步分析               |
| 3820 | 2728 | Rick And Morty | 檔名可疑，可能是誘餌或惡意程式              |
| 3880 | 1484 | WebCompanionIn | Lavasoft WebCompanion 相關，需注意 |
| 3856 | 3880 | WebCompanion.e | WebCompanion 子行程             |
| 3496 |  492 | Lavasoft.WCAss | Lavasoft WebCompanion 服務     |
| 3208 | 3880 | sc.exe         | 短時間執行，可能建立或操作服務              |
|  452 | 3880 | sc.exe         | 短時間執行，可能建立或操作服務              |
| 3504 | 3880 | sc.exe         | 短時間執行，可能建立或操作服務              |
| 2028 | 3880 | sc.exe         | 短時間執行，可能建立或操作服務              |
| 3304 | 3132 | notepad.exe    | 需要確認內容或來源                    |
| 3916 | 1428 | cmd.exe        | 短時間執行，需搭配 cmdline 分析         |
| 2420 |  348 | conhost.exe    | 與 cmd.exe 同時間出現              |

---

## 9. 重要可疑行程分析

### 9.1 BitTorrent.exe

```text
PID: 2836
PPID: 2728
ImageFileName: BitTorrent.exe
Wow64: True
CreateTime: 2018-08-04 19:27:07
```

`BitTorrent.exe` 是 P2P 下載軟體。
它本身不一定是惡意程式，但在鑑識分析中需要特別注意，因為 P2P 軟體常用於下載檔案，可能與惡意檔案來源有關。

本次結果中，`BitTorrent.exe` 是由 `explorer.exe` 啟動，代表可能是使用者主動開啟。

此外，它還建立了子行程：

```text
PID 2308 bittorrentie.e
PID 2624 bittorrentie.e
```

建議後續使用：

```bash
.\vol.exe -f .\OtterCTF.vmem windows.cmdline.CmdLine
.\vol.exe -f .\OtterCTF.vmem windows.netscan.NetScan
```

確認 BitTorrent 是否有可疑下載路徑或網路連線。

---

### 9.2 LunarMS.exe

```text
PID: 708
PPID: 2728
ImageFileName: LunarMS.exe
Wow64: True
CreateTime: 2018-08-04 19:27:39
```

`LunarMS.exe` 是本次結果中非常值得注意的行程。

原因如下：

1. 它不是 Windows 預設系統行程。
2. 它由 `explorer.exe` 啟動，代表可能是使用者執行。
3. 它是 Wow64 程序，代表 32-bit 程式在 64-bit Windows 上執行。
4. 在 OtterCTF 類型的記憶體題目中，非系統常見 EXE 通常需要優先分析。

後續建議針對 PID 708 進行深入分析：

```bash
.\vol.exe -f .\OtterCTF.vmem windows.cmdline.CmdLine --pid 708
.\vol.exe -f .\OtterCTF.vmem windows.dlllist.DllList --pid 708
.\vol.exe -f .\OtterCTF.vmem windows.malfind.Malfind --pid 708
.\vol.exe -f .\OtterCTF.vmem windows.handles.Handles --pid 708
```

---

### 9.3 Rick And Morty

```text
PID: 3820
PPID: 2728
ImageFileName: Rick And Morty
Wow64: True
CreateTime: 2018-08-04 19:32:55
```

`Rick And Morty` 是非常可疑的行程名稱。

原因如下：

1. 不是 Windows 系統行程。
2. 名稱不像正常應用程式。
3. 由 `explorer.exe` 啟動，代表可能是使用者執行的檔案。
4. 是 Wow64 程序，代表 32-bit 程式。
5. 建立時間接近記憶體擷取時間。

此行程很可能與本次 CTF 題目或可疑活動有關。

建議後續分析：

```bash
.\vol.exe -f .\OtterCTF.vmem windows.cmdline.CmdLine --pid 3820
.\vol.exe -f .\OtterCTF.vmem windows.dlllist.DllList --pid 3820
.\vol.exe -f .\OtterCTF.vmem windows.malfind.Malfind --pid 3820
.\vol.exe -f .\OtterCTF.vmem windows.handles.Handles --pid 3820
```

---

### 9.4 WebCompanion 相關行程

本次結果中出現多個 WebCompanion / Lavasoft 相關行程：

```text
PID 2844 WebCompanion.e
PID 3880 WebCompanionIn
PID 3496 Lavasoft.WCAss
PID 3856 WebCompanion.e
```

WebCompanion 通常與 Lavasoft Web Companion 相關。
它不一定是惡意程式，但常被視為不需要的軟體或潛在不需要程式 PUP。

需要注意的是，`WebCompanionIn` 建立後，後續出現多個 `sc.exe`：

```text
PID 3208 sc.exe
PID 452  sc.exe
PID 3504 sc.exe
PID 2028 sc.exe
```

`sc.exe` 是 Windows 服務控制工具，可以用來建立、啟動、停止或刪除 Service。

因此這裡的重點是：

> WebCompanion 相關行程可能透過 `sc.exe` 操作 Windows Service。

建議後續使用 `cmdline` 確認 `sc.exe` 執行了什麼命令。

---

### 9.5 sc.exe

```text
PID 3208 sc.exe CreateTime 2018-08-04 19:33:47 ExitTime 2018-08-04 19:33:48
PID 452  sc.exe CreateTime 2018-08-04 19:33:48 ExitTime 2018-08-04 19:33:48
PID 3504 sc.exe CreateTime 2018-08-04 19:33:48 ExitTime 2018-08-04 19:33:48
PID 2028 sc.exe CreateTime 2018-08-04 19:33:49 ExitTime 2018-08-04 19:34:03
```

`sc.exe` 是 Windows 內建服務控制程式。
它本身是正常工具，但在鑑識分析中非常重要，因為攻擊者或可疑程式可能使用它來：

* 建立服務
* 啟動服務
* 停止服務
* 刪除服務
* 修改服務設定

本次出現多個短時間執行的 `sc.exe`，而且父行程是：

```text
PPID 3880 WebCompanionIn
```

這是重要鑑識線索。

建議後續執行：

```bash
.\vol.exe -f .\OtterCTF.vmem windows.cmdline.CmdLine
```

確認這些 `sc.exe` 是否有執行 `create`、`start`、`delete` 等服務操作。

---

### 9.6 cmd.exe 與 conhost.exe

```text
PID 3916 cmd.exe
PPID 1428 vmtoolsd.exe
CreateTime 2018-08-04 19:34:22
ExitTime   2018-08-04 19:34:22

PID 2420 conhost.exe
PPID 348 csrss.exe
CreateTime 2018-08-04 19:34:22
ExitTime   2018-08-04 19:34:22
```

`cmd.exe` 是 Windows 命令提示字元。
`conhost.exe` 是 Console Window Host，通常會與 `cmd.exe` 搭配出現。

本次 `cmd.exe` 與 `conhost.exe` 建立與結束時間都非常接近記憶體擷取時間：

```text
2018-08-04 19:34:22
```

這個時間也接近 `windows.info.Info` 中的 SystemTime：

```text
2018-08-04 19:34:22
```

代表記憶體擷取時，可能剛好有命令列操作發生。

建議後續用 `cmdline` 確認 `cmd.exe` 的執行內容。

---

## 10. 時間線分析

根據 Process 建立時間，可以整理出以下重要時間線：

| 時間                  | 事件                                 |
| ------------------- | ---------------------------------- |
| 19:26:03            | System、smss.exe 啟動                 |
| 19:26:10 - 19:26:12 | Windows 核心服務與登入相關行程啟動              |
| 19:27:04            | explorer.exe 啟動                    |
| 19:27:07            | BitTorrent.exe、WebCompanion.e 啟動   |
| 19:27:39            | LunarMS.exe 啟動                     |
| 19:29:30            | chrome.exe 啟動                      |
| 19:32:55            | Rick And Morty 啟動                  |
| 19:33:07            | WebCompanionIn 啟動                  |
| 19:33:47 - 19:34:03 | 多個 sc.exe 執行                       |
| 19:34:05            | WebCompanion.e 再次啟動                |
| 19:34:10            | notepad.exe 啟動                     |
| 19:34:22            | cmd.exe、conhost.exe 短暫執行，接近記憶體擷取時間 |

此時間線顯示，可疑活動主要集中在：

```text
2018-08-04 19:32:55 - 19:34:22
```

尤其是 `Rick And Morty`、`WebCompanionIn`、多個 `sc.exe`、`cmd.exe` 與 `notepad.exe`。

---

## 11. 本次 pslist 鑑識重點

本次 `pslist` 分析中，最重要的發現如下：

1. 系統是正常 Windows 7 SP1 開機環境。
2. 記憶體映像檔來自 VMware 虛擬機器環境。
3. `BitTorrent.exe` 正在執行，可能與可疑檔案下載有關。
4. `LunarMS.exe` 是非系統常見行程，需要進一步分析。
5. `Rick And Morty` 是非常可疑的行程名稱，建議列為優先分析目標。
6. WebCompanion / Lavasoft 相關行程出現，可能為 PUP 或可疑軟體。
7. 多個 `sc.exe` 短時間執行，可能代表服務操作行為。
8. `cmd.exe` 與 `conhost.exe` 在記憶體擷取時間附近短暫出現，需要透過 `cmdline` 確認執行內容。

---

## 12. 後續建議分析指令

建議下一步執行 `cmdline`，確認可疑 Process 的完整執行路徑與參數：

```bash
.\vol.exe -f .\OtterCTF.vmem windows.cmdline.CmdLine
```

若要針對特定 PID，可以使用：

```bash
.\vol.exe -f .\OtterCTF.vmem windows.cmdline.CmdLine --pid 708
.\vol.exe -f .\OtterCTF.vmem windows.cmdline.CmdLine --pid 3820
.\vol.exe -f .\OtterCTF.vmem windows.cmdline.CmdLine --pid 3880
```

接著建議分析網路連線：

```bash
.\vol.exe -f .\OtterCTF.vmem windows.netscan.NetScan
```

再針對可疑 Process 進行 DLL 與注入分析：

```bash
.\vol.exe -f .\OtterCTF.vmem windows.dlllist.DllList --pid 708
.\vol.exe -f .\OtterCTF.vmem windows.malfind.Malfind --pid 708

.\vol.exe -f .\OtterCTF.vmem windows.dlllist.DllList --pid 3820
.\vol.exe -f .\OtterCTF.vmem windows.malfind.Malfind --pid 3820
```

也建議分析服務資訊：

```bash
.\vol.exe -f .\OtterCTF.vmem windows.svcscan.SvcScan
```

因為本次出現多個 `sc.exe`，可能與服務建立或修改有關。

---

## 13. 報告用結論

本次使用 Volatility 3 的 `windows.pslist.PsList` Plugin 分析 `OtterCTF.vmem`，成功列出記憶體映像檔中的行程資訊。

分析結果顯示，系統中存在多個正常 Windows 系統行程，例如 `System`、`smss.exe`、`csrss.exe`、`wininit.exe`、`services.exe`、`lsass.exe` 與多個 `svchost.exe`。此外，也可以看到 VMware 相關行程，例如 `vmtoolsd.exe`、`vmacthlp.exe` 與 `vmware-tray.exe`，代表此記憶體映像檔應來自 VMware 虛擬機器環境。

在可疑行程方面，本次發現 `BitTorrent.exe`、`LunarMS.exe`、`Rick And Morty`、`WebCompanion` 相關行程，以及多個短時間執行的 `sc.exe`。其中，`Rick And Morty` 與 `LunarMS.exe` 不是 Windows 預設行程，且由使用者層的 `explorer.exe` 啟動，因此需要列為後續分析重點。

另外，多個 `sc.exe` 由 `WebCompanionIn` 啟動，且在短時間內建立與結束，可能代表有服務建立、修改或刪除行為。最後，`cmd.exe` 與 `conhost.exe` 在記憶體擷取時間附近短暫出現，需透過 `cmdline` 進一步確認其執行內容。

綜合判斷，本次 `pslist` 的主要可疑目標為：

```text
LunarMS.exe
Rick And Morty
BitTorrent.exe
WebCompanionIn
sc.exe
cmd.exe
```

後續應優先使用 `cmdline`、`pstree`、`netscan`、`dlllist`、`malfind` 與 `svcscan` 進一步交叉分析。

---

## 14. 簡短結論

`windows.pslist.PsList` 成功列出系統行程，確認此記憶體映像檔可正常進行行程分析。

本次結果中大部分 Windows 系統行程正常，但有數個需要注意的行程：

```text
BitTorrent.exe
LunarMS.exe
Rick And Morty
WebCompanionIn
sc.exe
cmd.exe
```

其中 `Rick And Morty`、`LunarMS.exe` 與多個短時間執行的 `sc.exe` 是後續分析重點。

建議下一步執行：

```bash
.\vol.exe -f .\OtterCTF.vmem windows.cmdline.CmdLine
.\vol.exe -f .\OtterCTF.vmem windows.pstree.PsTree
.\vol.exe -f .\OtterCTF.vmem windows.netscan.NetScan
.\vol.exe -f .\OtterCTF.vmem windows.malfind.Malfind
```
