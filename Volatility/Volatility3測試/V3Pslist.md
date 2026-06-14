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

`windows.pslist.PsList` 是 Volatility 3 中用來列出 Windows 記憶體映像檔中行程的 Plugin。

它可以顯示目前仍存在於 Active Process List 中的行程資訊，例如 PID、PPID、行程名稱、建立時間、結束時間、Thread 數量、Handle 數量與 Session ID。

在 Windows 記憶體鑑識中，`pslist` 是非常重要的基礎分析工具，通常用來確認系統中有哪些行程，以及初步找出可疑行程。

---

## 3. PsList 欄位簡單說明

| 欄位           | 說明                                                                            |
| ------------ | ----------------------------------------------------------------------------- |
| PID          | Process ID，行程編號，用來識別每一個 Process。                                              |
| PPID         | Parent Process ID，父行程編號，表示這個 Process 是由哪一個 Process 啟動的。                       |
| Process Name | 行程名稱，也就是執行中的程式名稱，例如 `explorer.exe`、`cmd.exe`。                                 |
| Process 建立時間 | Process 開始執行的時間，可用來建立事件時間線。                                                   |
| Process 結束時間 | Process 結束的時間。如果顯示 `N/A`，代表擷取記憶體時該 Process 仍在執行。                              |
| Thread 數量    | 該 Process 內部執行緒的數量。數量異常偏高時，可能需要進一步確認。                                         |
| Handle 數量    | 該 Process 開啟的資源數量，例如檔案、Registry、Mutex、Process 等。                              |
| Session ID   | Process 所屬的登入 Session。`0` 多為系統服務，`1` 通常是使用者桌面環境。                              |
| Wow64        | 判斷是否為 32-bit 程式在 64-bit Windows 上執行。`True` 代表 32-bit 程式，`False` 代表非 Wow64 程式。 |

簡單來說，`pslist` 的重點是透過 PID、PPID、行程名稱與建立時間，判斷系統中有哪些 Process，以及它們之間的父子關係。

如果出現不熟悉的 Process、奇怪的父子關係，或短時間建立又結束的 Process，就需要進一步分析。

---

## 4. 系統正常行程分析

本次結果中，可以看到多個 Windows 正常系統行程：

| PID | PPID | Process      | 說明                            |
| --: | ---: | ------------ | ----------------------------- |
|   4 |    0 | System       | Windows 系統核心行程                |
| 260 |    4 | smss.exe     | Session Manager               |
| 348 |  336 | csrss.exe    | Client Server Runtime Process |
| 388 |  380 | csrss.exe    | 使用者 Session 的 csrss           |
| 396 |  336 | wininit.exe  | Windows 初始化行程                 |
| 432 |  380 | winlogon.exe | 使用者登入行程                       |
| 492 |  396 | services.exe | Windows 服務管理行程                |
| 500 |  396 | lsass.exe    | 帳號驗證與安全性相關行程                  |
| 508 |  396 | lsm.exe      | Local Session Manager         |

這些行程屬於 Windows 正常開機後常見的系統行程，父子關係大致正常。

---

## 5. VMware 相關行程

本次結果中出現多個 VMware 相關行程：

|  PID | PPID | Process        | 說明                   |
| ---: | ---: | -------------- | -------------------- |
|  668 |  492 | vmacthlp.exe   | VMware Tools 相關服務    |
| 1428 |  492 | vmtoolsd.exe   | VMware Tools Service |
| 2804 | 2728 | vmtoolsd.exe   | 使用者層 VMware Tools    |
| 3720 | 3820 | vmware-tray.ex | VMware Tray 程式       |

這代表此記憶體映像檔很可能來自 VMware 虛擬機器環境。

這也符合檔案名稱 `OtterCTF.vmem`，因為 `.vmem` 通常是 VMware 產生的記憶體映像檔。

---

## 6. 使用者層行程

### 6.1 explorer.exe

```text
PID: 2728
PPID: 2696
Process: explorer.exe
CreateTime: 2018-08-04 19:27:04
```

`explorer.exe` 是 Windows 桌面與檔案總管行程。

本次結果中，多個使用者程式都是由 `explorer.exe` 啟動，例如：

|  PID | Process        |
| ---: | -------------- |
| 2836 | BitTorrent.exe |
| 2844 | WebCompanion.e |
|  708 | LunarMS.exe    |
| 4076 | chrome.exe     |
| 3820 | Rick And Morty |

這些行程屬於使用者層活動，需要進一步判斷是否正常。
```
D:\Forensic\G140A006\VolatilityWorkbench>.\vol.exe -f .\OtterCTF.vmem windows.pslist.PsList | findstr 2728
2728ress269600.0explorer.exe    0xfa801b27e060in33hed   854     1       False   2018-08-04 19:27:04.000000      N/A    Disabled
2804    2728    vmtoolsd.exe    0xfa801b1cdb30  6       190     1       False   2018-08-04 19:27:06.000000      N/A    Disabled
2836    2728    BitTorrent.exe  0xfa801b290b30  24      471     1       True    2018-08-04 19:27:07.000000      N/A    Disabled
2844    2728    WebCompanion.e  0xfa801b2f02e0  0       -       1       False   2018-08-04 19:27:07.000000      2018-08-04 19:33:33.000000      Disabled
708     2728    LunarMS.exe     0xfa801b5cb740  18      346     1       True    2018-08-04 19:27:39.000000      N/A    Disabled
4076    2728    chrome.exe      0xfa801a4e3870  44      1160    1       False   2018-08-04 19:29:30.000000      N/A    Disabled
3820    2728    Rick And Morty  0xfa801b486b30  4       185     1       True    2018-08-04 19:32:55.000000      N/A    Disabled
```

---

## 7. 可疑或需要注意的行程

本次 `pslist` 中較需要注意的行程如下：

|  PID | PPID | Process        | 注意原因                     |
| ---: | ---: | -------------- | ------------------------ |
| 2836 | 2728 | BitTorrent.exe | P2P 下載軟體，可能與可疑檔案下載有關     |
| 2308 | 2836 | bittorrentie.e | BitTorrent 子行程           |
| 2624 | 2836 | bittorrentie.e | BitTorrent 子行程           |
|  708 | 2728 | LunarMS.exe    | 非 Windows 預設行程，需要進一步分析   |
| 3820 | 2728 | Rick And Morty | 行程名稱可疑，需優先分析             |
| 3880 | 1484 | WebCompanionIn | WebCompanion 相關行程        |
| 3856 | 3880 | WebCompanion.e | WebCompanion 子行程         |
| 3496 |  492 | Lavasoft.WCAss | Lavasoft WebCompanion 服務 |
| 3208 | 3880 | sc.exe         | 短時間執行，可能操作服務             |
|  452 | 3880 | sc.exe         | 短時間執行，可能操作服務             |
| 3504 | 3880 | sc.exe         | 短時間執行，可能操作服務             |
| 2028 | 3880 | sc.exe         | 短時間執行，可能操作服務             |
| 3304 | 3132 | notepad.exe    | 需要確認開啟內容                 |
| 3916 | 1428 | cmd.exe        | 短時間執行，需確認命令內容            |
| 2420 |  348 | conhost.exe    | 與 cmd.exe 同時間出現          |

---

## 8. 重要可疑行程分析

### 8.1 BitTorrent.exe

```text
PID: 2836
PPID: 2728
Process: BitTorrent.exe
Wow64: True
CreateTime: 2018-08-04 19:27:07
```

`BitTorrent.exe` 是 P2P 下載軟體。

它本身不一定是惡意程式，但在鑑識分析中需要注意，因為 P2P 軟體可能用來下載未知或可疑檔案。

本次 `BitTorrent.exe` 是由 `explorer.exe` 啟動，表示可能是使用者主動執行。

另外，它也產生了兩個子行程：

```text
PID 2308 bittorrentie.e
PID 2624 bittorrentie.e
```

```
D:\Forensic\G140A006\VolatilityWorkbench>.\vol.exe -f .\OtterCTF.vmem windows.pslist.PsList | findstr 2836
2836ress272800.0BitTorrent.exe  0xfa801b290b30in24hed   471     1       True    2018-08-04 19:27:07.000000      N/A    Disabled
2308    2836    bittorrentie.e  0xfa801b4a7b30  15      337     1       True    2018-08-04 19:27:19.000000      N/A    Disabled
2624    2836    bittorrentie.e  0xfa801b4c9b30  13      316     1       True    2018-08-04 19:27:21.000000      N/A    Disabled
```

後續應搭配 `cmdline` 與 `netscan` 檢查 BitTorrent 的執行路徑與網路連線。

---

### 8.2 LunarMS.exe

```text
PID: 708
PPID: 2728
Process: LunarMS.exe
Wow64: True
CreateTime: 2018-08-04 19:27:39
```

`LunarMS.exe` 是本次結果中非常值得注意的行程。

原因如下：

1. 不是 Windows 預設系統行程。
2. 由 `explorer.exe` 啟動，可能是使用者執行。
3. `Wow64=True`，代表它是 32-bit 程式在 64-bit Windows 上執行。
4. 在記憶體鑑識題目中，非系統常見 EXE 通常需要優先分析。

後續建議針對 PID 708 執行：

```bash
.\vol.exe -f .\OtterCTF.vmem windows.cmdline.CmdLine --pid 708
.\vol.exe -f .\OtterCTF.vmem windows.dlllist.DllList --pid 708
.\vol.exe -f .\OtterCTF.vmem windows.malfind.Malfind --pid 708
```

---

### 8.3 Rick And Morty

```text
PID: 3820
PPID: 2728
Process: Rick And Morty
Wow64: True
CreateTime: 2018-08-04 19:32:55
```

`Rick And Morty` 是非常可疑的行程名稱。

原因如下：

1. 不是 Windows 系統行程。
2. 名稱不像一般正式軟體。
3. 由 `explorer.exe` 啟動。
4. 建立時間接近記憶體擷取時間。
5. `Wow64=True`，代表它是 32-bit 程式。

此行程很可能與本次 CTF 題目或可疑活動有關，應列為優先分析目標。

後續建議執行：

```bash
.\vol.exe -f .\OtterCTF.vmem windows.cmdline.CmdLine --pid 3820
.\vol.exe -f .\OtterCTF.vmem windows.dlllist.DllList --pid 3820
.\vol.exe -f .\OtterCTF.vmem windows.malfind.Malfind --pid 3820
```

---

### 8.4 WebCompanion / Lavasoft 相關行程

本次出現多個 WebCompanion / Lavasoft 相關行程：

```text
PID 2844 WebCompanion.e
PID 3880 WebCompanionIn
PID 3496 Lavasoft.WCAss
PID 3856 WebCompanion.e
```

WebCompanion 通常與 Lavasoft Web Companion 相關，可能屬於 PUP，也就是潛在不需要程式。

需要注意的是，`WebCompanionIn` 後續啟動了多個 `sc.exe`。

這代表 WebCompanion 相關行程可能正在操作 Windows Service。

---

### 8.5 sc.exe

```text
PID 3208 sc.exe  CreateTime 2018-08-04 19:33:47  ExitTime 2018-08-04 19:33:48
PID 452  sc.exe  CreateTime 2018-08-04 19:33:48  ExitTime 2018-08-04 19:33:48
PID 3504 sc.exe  CreateTime 2018-08-04 19:33:48  ExitTime 2018-08-04 19:33:48
PID 2028 sc.exe  CreateTime 2018-08-04 19:33:49  ExitTime 2018-08-04 19:34:03
```
```
D:\Forensic\G140A006\VolatilityWorkbench>.\vol.exe -f .\OtterCTF.vmem windows.pslist.PsList | findstr sc.exe
3208ress388000.0sc.exe  0xfa801b08f060an0ing fin-shed   0       False   2018-08-04 19:33:47.000000      2018-08-04 19:33:48.000000      Disabled
452     3880    sc.exe  0xfa801aeb6890  0       -       0       False   2018-08-04 19:33:48.000000      2018-08-04 19:33:48.000000      Disabled
3504    3880    sc.exe  0xfa801aa72b30  0       -       0       False   2018-08-04 19:33:48.000000      2018-08-04 19:33:48.000000      Disabled
2028    3880    sc.exe  0xfa801ac01060  0       -       0       False   2018-08-04 19:33:49.000000      2018-08-04 19:34:03.000000      Disabled
```

`sc.exe` 是 Windows 內建的服務控制工具。

它可以用來：

* 建立服務
* 啟動服務
* 停止服務
* 刪除服務
* 修改服務設定

本次多個 `sc.exe` 在短時間內出現，而且父行程是 `WebCompanionIn`，因此需要注意是否有服務被建立或修改。

後續應使用 `cmdline` 查看 `sc.exe` 的完整命令內容。

---

### 8.6 cmd.exe 與 conhost.exe

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

`conhost.exe` 是 Console Window Host，通常會與 `cmd.exe` 一起出現。

本次 `cmd.exe` 和 `conhost.exe` 出現在 `2018-08-04 19:34:22`，這個時間非常接近記憶體擷取時間，因此需要進一步確認是否有命令列操作。

---

## 9. 時間線整理

| 時間                  | 事件                               |
| ------------------- | -------------------------------- |
| 19:26:03            | System、smss.exe 啟動               |
| 19:26:10 - 19:26:12 | Windows 核心行程與服務啟動                |
| 19:27:04            | explorer.exe 啟動                  |
| 19:27:07            | BitTorrent.exe、WebCompanion.e 啟動 |
| 19:27:39            | LunarMS.exe 啟動                   |
| 19:29:30            | chrome.exe 啟動                    |
| 19:32:55            | Rick And Morty 啟動                |
| 19:33:07            | WebCompanionIn 啟動                |
| 19:33:47 - 19:34:03 | 多個 sc.exe 執行                     |
| 19:34:05            | WebCompanion.e 再次啟動              |
| 19:34:10            | notepad.exe 啟動                   |
| 19:34:22            | cmd.exe、conhost.exe 短暫執行         |

可疑活動主要集中在：

```text
2018-08-04 19:32:55 - 19:34:22
```

這段時間出現了 `Rick And Morty`、`WebCompanionIn`、多個 `sc.exe`、`notepad.exe` 與 `cmd.exe`。

---

## 10. 本次 PsList 鑑識重點

本次 `pslist` 分析中，重要發現如下：

1. 系統行程大致正常。
2. 記憶體映像檔來自 VMware 虛擬機器環境。
3. `BitTorrent.exe` 正在執行，可能與下載活動有關。
4. `LunarMS.exe` 不是 Windows 預設行程，需進一步分析。
5. `Rick And Morty` 行程名稱可疑，應列為優先分析目標。
6. WebCompanion / Lavasoft 相關行程出現，可能屬於 PUP。
7. 多個 `sc.exe` 短時間執行，可能代表服務操作。
8. `cmd.exe` 在記憶體擷取時間附近短暫出現，需確認命令內容。

---

## 11. 後續建議分析指令

建議下一步先執行 `cmdline`：

```bash
.\vol.exe -f .\OtterCTF.vmem windows.cmdline.CmdLine
```

針對可疑 PID：

```bash
.\vol.exe -f .\OtterCTF.vmem windows.cmdline.CmdLine --pid 708
.\vol.exe -f .\OtterCTF.vmem windows.cmdline.CmdLine --pid 3820
.\vol.exe -f .\OtterCTF.vmem windows.cmdline.CmdLine --pid 3880
```

接著分析網路連線：

```bash
.\vol.exe -f .\OtterCTF.vmem windows.netscan.NetScan
```

針對可疑行程做 DLL 與注入分析：

```bash
.\vol.exe -f .\OtterCTF.vmem windows.dlllist.DllList --pid 708
.\vol.exe -f .\OtterCTF.vmem windows.malfind.Malfind --pid 708

.\vol.exe -f .\OtterCTF.vmem windows.dlllist.DllList --pid 3820
.\vol.exe -f .\OtterCTF.vmem windows.malfind.Malfind --pid 3820
```

因為本次有多個 `sc.exe`，也建議分析服務：

```bash
.\vol.exe -f .\OtterCTF.vmem windows.svcscan.SvcScan
```

---

## 12. 報告用結論

本次使用 Volatility 3 的 `windows.pslist.PsList` Plugin 分析 `OtterCTF.vmem`，成功列出記憶體映像檔中的行程資訊。

分析結果顯示，系統中存在多個正常 Windows 系統行程，例如 `System`、`smss.exe`、`csrss.exe`、`wininit.exe`、`services.exe`、`lsass.exe` 與多個 `svchost.exe`。同時也發現 VMware 相關行程，例如 `vmtoolsd.exe`、`vmacthlp.exe` 與 `vmware-tray.exe`，代表此記憶體映像檔來自 VMware 虛擬機器環境。

在可疑行程方面，本次發現 `BitTorrent.exe`、`LunarMS.exe`、`Rick And Morty`、WebCompanion 相關行程，以及多個短時間執行的 `sc.exe`。其中 `Rick And Morty` 與 `LunarMS.exe` 不是 Windows 預設行程，且由使用者層的 `explorer.exe` 啟動，因此需要列為後續分析重點。

另外，多個 `sc.exe` 由 `WebCompanionIn` 啟動，可能代表服務建立、修改或刪除行為。`cmd.exe` 與 `conhost.exe` 則在記憶體擷取時間附近短暫出現，需要透過 `cmdline` 進一步確認執行內容。

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

## 13. 簡短結論

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
