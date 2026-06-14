# 測試內容
- vol.exe -f .\OtterCTF.vmem windows.psscan.PsScan

```
D:\Forensic\G140A006\VolatilityWorkbench>.\vol.exe -f .\OtterCTF.vmem windows.psscan.PsScan
Volatility 3 Framework 2.5.0
Progress:  100.00               PDB scanning finished
PID     PPID    ImageFileName   Offset(V)       Threads Handles SessionId       Wow64   CreateTime      ExitTime       File output

412     492     mscorsvw.exe    0x7d403610      7       86      0       True    2018-08-04 19:28:42.000000      N/A     Disabled
3820    2728    Rick And Morty  0x7d686b30      4       185     1       True    2018-08-04 19:32:55.000000      N/A     Disabled
2308    2836    bittorrentie.e  0x7d6a7b30      15      337     1       True    2018-08-04 19:27:19.000000      N/A     Disabled
2624    2836    bittorrentie.e  0x7d6c9b30      13      316     1       True    2018-08-04 19:27:21.000000      N/A     Disabled
708     2728    LunarMS.exe     0x7d7cb740      18      346     1       True    2018-08-04 19:27:39.000000      N/A     Disabled
2500    492     sppsvc.exe      0x7d832060      4       149     0       False   2018-08-04 19:26:58.000000      N/A     Disabled
2728    2696    explorer.exe    0x7d87e060      33      854     1       False   2018-08-04 19:27:04.000000      N/A     Disabled
2836    2728    BitTorrent.exe  0x7d890b30      24      471     1       True    2018-08-04 19:27:07.000000      N/A     Disabled
2844    2728    WebCompanion.e  0x7d8f02e0      0       -       1       False   2018-08-04 19:27:07.000000      2018-08-04 19:33:33.000000      Disabled
3064    492     SearchIndexer.  0x7d9aab30      11      610     0       False   2018-08-04 19:27:14.000000      N/A     Disabled
3208    3880    sc.exe  0x7da8f060      0       -       0       False   2018-08-04 19:33:47.000000      2018-08-04 19:33:48.000000      Disabled
2136    604     WmiPrvSE.exe    0x7db12060      12      324     0       False   2018-08-04 19:26:51.000000      N/A     Disabled
3880    1484    WebCompanionIn  0x7db8f060      15      522     0       True    2018-08-04 19:33:07.000000      N/A     Disabled
2804    2728    vmtoolsd.exe    0x7dbcdb30      6       190     1       False   2018-08-04 19:27:06.000000      N/A     Disabled
2344    492     taskhost.exe    0x7dbe9b30      8       193     1       False   2018-08-04 19:26:57.000000      N/A     Disabled
2704    844     dwm.exe 0x7dbfab30      4       97      1       False   2018-08-04 19:27:04.000000      N/A     Disabled
3304    3132    notepad.exe     0x7dbfd960      2       79      1       False   2018-08-04 19:34:10.000000      N/A     Disabled
1356    492     VGAuthService.  0x7dc0f630      3       85      0       False   2018-08-04 19:26:25.000000      N/A     Disabled
1324    492     dllhost.exe     0x7dc7f630      15      207     0       False   2018-08-04 19:26:42.000000      N/A     Disabled
1428    492     vmtoolsd.exe    0x7dc92920      9       313     0       False   2018-08-04 19:26:27.000000      N/A     Disabled
452     3880    sc.exe  0x7dcb6890      0       -       0       False   2018-08-04 19:33:48.000000      2018-08-04 19:33:48.000000      Disabled
2740    3064    SearchFilterHo  0x7dce7b30      0       -       0       False   2018-08-04 19:33:11.000000      2018-08-04 19:34:22.000000      Disabled
1948    492     svchost.exe     0x7dde7800      6       96      0       False   2018-08-04 19:26:42.000000      N/A     Disabled
1436    492     msdtc.exe       0x7ddf3b30      14      155     0       False   2018-08-04 19:26:43.000000      N/A     Disabled
2028    3880    sc.exe  0x7de01060      0       -       0       False   2018-08-04 19:33:49.000000      2018-08-04 19:34:03.000000      Disabled
808     492     svchost.exe     0x7de2e9e0      22      508     0       False   2018-08-04 19:26:18.000000      N/A     Disabled
844     492     svchost.exe     0x7de31b30      17      396     0       False   2018-08-04 19:26:18.000000      N/A     Disabled
868     492     svchost.exe     0x7de4db30      45      1114    0       False   2018-08-04 19:26:18.000000      N/A     Disabled
960     808     audiodg.exe     0x7de753a0      7       151     0       False   2018-08-04 19:26:19.000000      N/A     Disabled
1012    492     svchost.exe     0x7de97060      12      554     0       False   2018-08-04 19:26:20.000000      N/A     Disabled
620     492     svchost.exe     0x7ded37e0      19      415     0       False   2018-08-04 19:26:21.000000      N/A     Disabled
1120    492     spoolsv.exe     0x7df5ab30      14      346     0       False   2018-08-04 19:26:22.000000      N/A     Disabled
1164    492     svchost.exe     0x7df718a0      18      312     0       False   2018-08-04 19:26:23.000000      N/A     Disabled
3924    4076    chrome.exe      0x7e000a90      16      228     1       False   2018-08-04 19:29:51.000000      N/A     Disabled
3504    3880    sc.exe  0x7e072b30      0       -       0       False   2018-08-04 19:33:48.000000      2018-08-04 19:33:48.000000      Disabled
3496    492     Lavasoft.WCAss  0x7e0d1060      14      473     0       False   2018-08-04 19:33:49.000000      N/A     Disabled
432     380     winlogon.exe    0x7e0f4060      3       113     1       False   2018-08-04 19:26:11.000000      N/A     Disabled
492     396     services.exe    0x7e1377c0      11      242     0       False   2018-08-04 19:26:12.000000      N/A     Disabled
500     396     lsass.exe       0x7e13f060      7       610     0       False   2018-08-04 19:26:12.000000      N/A     Disabled
508     396     lsm.exe 0x7e1461a0      10      148     0       False   2018-08-04 19:26:12.000000      N/A     Disabled
668     492     vmacthlp.exe    0x7e1bdb30      3       56      0       False   2018-08-04 19:26:16.000000      N/A     Disabled
712     492     svchost.exe     0x7e1ebb30      8       301     0       False   2018-08-04 19:26:17.000000      N/A     Disabled
3856    3880    WebCompanion.e  0x7e4268b0      15      386     0       True    2018-08-04 19:34:05.000000      N/A     Disabled
3648    4076    chrome.exe      0x7e435240      16      207     1       False   2018-08-04 19:33:38.000000      N/A     Disabled
2420    348     conhost.exe     0x7e4643d0      0       30      0       False   2018-08-04 19:34:22.000000      2018-08-04 19:34:22.000000      Disabled
164     492     svchost.exe     0x7e4af9f0      12      147     0       False   2018-08-04 19:28:42.000000      N/A     Disabled
3124    492     mscorsvw.exe    0x7e4c2700      7       77      0       False   2018-08-04 19:28:43.000000      N/A     Disabled
3196    492     svchost.exe     0x7e4e4b30      14      352     0       False   2018-08-04 19:28:44.000000      N/A     Disabled
3788    3916    ipconfig.exe    0x7e5bfb30      0       -       0       False   2018-08-04 19:34:22.000000      2018-08-04 19:34:22.000000      Disabled
2748    4076    chrome.exe      0x7e5f98f0      15      181     1       False   2018-08-04 19:31:15.000000      N/A     Disabled
3720    3820    vmware-tray.ex  0x7e6c5b30      8       147     1       True    2018-08-04 19:33:02.000000      N/A     Disabled
4076    2728    chrome.exe      0x7e6e3870      44      1160    1       False   2018-08-04 19:29:30.000000      N/A     Disabled
4084    4076    chrome.exe      0x7e6eab30      8       86      1       False   2018-08-04 19:29:30.000000      N/A     Disabled
1808    4076    chrome.exe      0x7e6f7b30      13      229     1       False   2018-08-04 19:29:32.000000      N/A     Disabled
576     4076    chrome.exe      0x7e702b30      2       58      1       False   2018-08-04 19:29:31.000000      N/A     Disabled
3916    1428    cmd.exe 0x7e772b30      0       -       0       False   2018-08-04 19:34:22.000000      2018-08-04 19:34:22.000000      Disabled
1796    4076    chrome.exe      0x7e7ef1f0      15      170     1       False   2018-08-04 19:33:41.000000      N/A     Disabled
3428    3064    SearchProtocol  0x7e7fe210      0       -       0       False   2018-08-04 19:33:11.000000      2018-08-04 19:34:22.000000      Disabled
396     336     wininit.exe     0x7e8ed060      3       78      0       False   2018-08-04 19:26:11.000000      N/A     Disabled
348     336     csrss.exe       0x7eac8380      9       563     0       False   2018-08-04 19:26:10.000000      N/A     Disabled
724     492     PresentationFo  0x7f28c2d0      6       148     0       False   2018-08-04 19:27:52.000000      N/A     Disabled
388     380     csrss.exe       0x7f2d3b30      11      460     1       False   2018-08-04 19:26:11.000000      N/A     Disabled
260     4       smss.exe        0x7f67e4d0      2       30      N/A     False   2018-08-04 19:26:03.000000      N/A     Disabled
1800    604     WmiPrvSE.exe    0x7fb24b30      9       222     0       False   2018-08-04 19:26:39.000000      N/A     Disabled
604     492     svchost.exe     0x7fc3c890      11      376     0       False   2018-08-04 19:26:16.000000      N/A     Disabled
4       0       System  0x7fe83740      95      411     N/A     False   2018-08-04 19:26:03.000000      N/A     Disabled
```


# windows.psscan.PsScan 分析

## 1. 執行指令

```bash
.\vol.exe -f .\OtterCTF.vmem windows.psscan.PsScan
```

---

## 2. Plugin 功能說明

`windows.psscan.PsScan` 是 Volatility 3 中用來掃描記憶體中 Process 物件的 Plugin。

它和 `pslist` 不一樣：

| Plugin   | 說明                                           |
| -------- | -------------------------------------------- |
| `pslist` | 從 Windows Active Process List 列出目前正在系統清單中的行程 |
| `psscan` | 直接掃描記憶體中的 Process 物件，可找出已結束或可能被隱藏的行程         |

因此，`psscan` 常用來發現：

* 已結束但仍殘留在記憶體中的 Process
* 沒有出現在 `pslist` 的隱藏行程
* Rootkit 可能隱藏的 Process
* 短時間執行後結束的可疑程式

---

## 3. PsScan 欄位簡單說明

| 欄位            | 說明                                |
| ------------- | --------------------------------- |
| PID           | Process ID，行程編號                   |
| PPID          | Parent Process ID，父行程編號           |
| ImageFileName | 行程名稱                              |
| Offset(V)     | 該 Process 物件在記憶體中的位址              |
| Threads       | Thread 數量                         |
| Handles       | Handle 數量                         |
| SessionId     | 所屬登入 Session                      |
| Wow64         | 是否為 32-bit 程式在 64-bit Windows 上執行 |
| CreateTime    | 行程建立時間                            |
| ExitTime      | 行程結束時間，若為 `N/A` 代表擷取時仍在執行         |

---

## 4. 本次執行結果重點

本次 `psscan` 成功掃描出多個 Process，結果與前面的 `pslist` 大多一致。

這代表目前沒有明顯看到大量被隱藏的行程。

不過，`psscan` 額外顯示了一些已結束或短時間執行的 Process，這些在鑑識分析中非常重要。

---

## 5. 與 pslist 的比較重點

`psscan` 的價值在於可以和 `pslist` 交叉比對。

如果某個 Process 出現在 `psscan`，但沒有出現在 `pslist`，可能代表：

1. Process 已經結束，但記憶體中仍有殘留。
2. Process 被惡意程式或 Rootkit 隱藏。
3. Process 曾經短暫執行過。
4. Windows Active Process List 中已經沒有該行程，但 EPROCESS 結構仍可被掃描到。

本次結果中，大部分 Process 在 `pslist` 中也能看到，因此沒有明顯 Process hiding 的跡象。

但是有一些短時間執行並結束的 Process 需要特別注意。

---

## 6. 已結束或短時間執行的行程

本次 `psscan` 中出現多個有 `ExitTime` 的 Process：

|  PID | PPID | Process        | CreateTime | ExitTime | 注意原因                  |
| ---: | ---: | -------------- | ---------- | -------- | --------------------- |
| 2844 | 2728 | WebCompanion.e | 19:27:07   | 19:33:33 | WebCompanion 相關，已結束   |
| 3208 | 3880 | sc.exe         | 19:33:47   | 19:33:48 | 短時間執行，可能操作 Service    |
|  452 | 3880 | sc.exe         | 19:33:48   | 19:33:48 | 短時間執行，可能操作 Service    |
| 3504 | 3880 | sc.exe         | 19:33:48   | 19:33:48 | 短時間執行，可能操作 Service    |
| 2028 | 3880 | sc.exe         | 19:33:49   | 19:34:03 | 短時間執行，可能操作 Service    |
| 2740 | 3064 | SearchFilterHo | 19:33:11   | 19:34:22 | Windows Search 相關，已結束 |
| 3428 | 3064 | SearchProtocol | 19:33:11   | 19:34:22 | Windows Search 相關，已結束 |
| 3916 | 1428 | cmd.exe        | 19:34:22   | 19:34:22 | 命令列短暫執行               |
| 3788 | 3916 | ipconfig.exe   | 19:34:22   | 19:34:22 | 由 cmd.exe 啟動，短暫執行     |
| 2420 |  348 | conhost.exe    | 19:34:22   | 19:34:22 | 與 cmd.exe 同時間出現       |

這些行程雖然可能已經結束，但仍然被 `psscan` 掃描到，代表它們在記憶體中留下了痕跡。

---

## 7. 重要可疑行程分析

### 7.1 Rick And Morty

```text
PID: 3820
PPID: 2728
Process: Rick And Morty
Wow64: True
CreateTime: 2018-08-04 19:32:55
ExitTime: N/A
```

`Rick And Morty` 是本次結果中非常重要的可疑行程。

可疑原因：

1. 不是 Windows 預設系統行程。
2. 行程名稱不像正式軟體名稱。
3. 由 `explorer.exe` 啟動，代表可能是使用者手動執行。
4. `Wow64=True`，代表它是 32-bit 程式。
5. 在 `pslist` 與 `psscan` 中都存在，代表擷取記憶體時仍在執行。

此行程應列為優先分析目標。

建議後續指令：

```bash
.\vol.exe -f .\OtterCTF.vmem windows.cmdline.CmdLine --pid 3820
.\vol.exe -f .\OtterCTF.vmem windows.dlllist.DllList --pid 3820
.\vol.exe -f .\OtterCTF.vmem windows.malfind.Malfind --pid 3820
```

---

### 7.2 LunarMS.exe

```text
PID: 708
PPID: 2728
Process: LunarMS.exe
Wow64: True
CreateTime: 2018-08-04 19:27:39
ExitTime: N/A
```

`LunarMS.exe` 也是本次需要注意的行程。

可疑原因：

1. 不是 Windows 預設系統行程。
2. 由 `explorer.exe` 啟動。
3. 是 32-bit 程式。
4. 在 `pslist` 和 `psscan` 中都存在，代表擷取時仍在執行。

雖然它可能是遊戲或一般應用程式，但在記憶體鑑識中仍需要確認它的路徑、參數、DLL 與是否有程式碼注入。

建議後續指令：

```bash
.\vol.exe -f .\OtterCTF.vmem windows.cmdline.CmdLine --pid 708
.\vol.exe -f .\OtterCTF.vmem windows.dlllist.DllList --pid 708
.\vol.exe -f .\OtterCTF.vmem windows.malfind.Malfind --pid 708
```

---

### 7.3 BitTorrent.exe 與 bittorrentie.e

```text
PID: 2836
Process: BitTorrent.exe
PPID: 2728

PID: 2308
Process: bittorrentie.e
PPID: 2836

PID: 2624
Process: bittorrentie.e
PPID: 2836
```

`BitTorrent.exe` 是 P2P 下載軟體，子行程為 `bittorrentie.e`。

它本身不一定是惡意程式，但在鑑識分析中需要注意，因為 P2P 軟體常與未知檔案下載有關。

需要進一步確認：

* 是否下載過可疑檔案
* 是否有異常網路連線
* 是否與後續可疑行程有關

建議後續指令：

```bash
.\vol.exe -f .\OtterCTF.vmem windows.cmdline.CmdLine --pid 2836
.\vol.exe -f .\OtterCTF.vmem windows.netscan.NetScan
```

---

### 7.4 WebCompanionIn 與 sc.exe

```text
PID: 3880
Process: WebCompanionIn
CreateTime: 2018-08-04 19:33:07

PID: 3208
Process: sc.exe
PPID: 3880
ExitTime: 2018-08-04 19:33:48

PID: 452
Process: sc.exe
PPID: 3880
ExitTime: 2018-08-04 19:33:48

PID: 3504
Process: sc.exe
PPID: 3880
ExitTime: 2018-08-04 19:33:48

PID: 2028
Process: sc.exe
PPID: 3880
ExitTime: 2018-08-04 19:34:03
```

這是本次 `psscan` 分析中非常重要的線索。

`sc.exe` 是 Windows 服務控制工具，可以用來：

* 建立服務
* 啟動服務
* 停止服務
* 刪除服務
* 修改服務設定

本次多個 `sc.exe` 都是由 `WebCompanionIn` 啟動，而且都在短時間內結束。

這代表 `WebCompanionIn` 可能曾經操作 Windows Service。

是否為正常安裝行為或可疑服務操作，需要透過 `cmdline` 與 `svcscan` 確認。

建議後續指令：

```bash
.\vol.exe -f .\OtterCTF.vmem windows.cmdline.CmdLine
.\vol.exe -f .\OtterCTF.vmem windows.svcscan.SvcScan
```

---

### 7.5 cmd.exe 與 ipconfig.exe

```text
PID: 3916
Process: cmd.exe
PPID: 1428
CreateTime: 2018-08-04 19:34:22
ExitTime: 2018-08-04 19:34:22

PID: 3788
Process: ipconfig.exe
PPID: 3916
CreateTime: 2018-08-04 19:34:22
ExitTime: 2018-08-04 19:34:22
```

`psscan` 額外清楚顯示：`ipconfig.exe` 是由 `cmd.exe` 啟動。

這代表在記憶體擷取時間附近，有人或某個程式執行了類似網路設定查詢的命令。

`ipconfig.exe` 通常用於查看本機 IP、DNS、Gateway 等網路資訊。

這個行為不一定惡意，但在 CTF 或事件調查中非常重要，因為它可能代表：

1. 使用者正在查看網路設定。
2. 惡意程式正在偵察系統網路環境。
3. 攻擊者正在確認主機 IP 與網路狀態。
4. VMware Tools 或其他程式觸發了命令列操作。

此線索需要透過 `cmdline` 確認完整命令。

---

## 8. 時間線整理

| 時間                  | 事件                                 |
| ------------------- | ---------------------------------- |
| 19:27:07            | BitTorrent.exe 與 WebCompanion.e 啟動 |
| 19:27:39            | LunarMS.exe 啟動                     |
| 19:32:55            | Rick And Morty 啟動                  |
| 19:33:07            | WebCompanionIn 啟動                  |
| 19:33:47 - 19:34:03 | 多個 `sc.exe` 被 WebCompanionIn 啟動    |
| 19:34:05            | WebCompanion.e 再次啟動                |
| 19:34:10            | notepad.exe 啟動                     |
| 19:34:22            | cmd.exe 啟動                         |
| 19:34:22            | ipconfig.exe 由 cmd.exe 啟動          |
| 19:34:22            | conhost.exe 出現                     |
| 19:34:22            | 記憶體擷取時間附近                          |

可疑活動主要集中在：

```text
2018-08-04 19:32:55 - 19:34:22
```

---

## 9. psscan 與 pslist 交叉分析

本次 `psscan` 與前面的 `pslist` 結果大致一致。

這代表：

1. 沒有明顯發現被隱藏的 Process。
2. 主要可疑行程在 `pslist` 中也能看到。
3. `psscan` 額外強化了已結束 Process 的線索。
4. 短時間執行的 `sc.exe`、`cmd.exe`、`ipconfig.exe` 是後續重點。

其中最重要的補充是：

```text
ipconfig.exe 是由 cmd.exe 啟動
```

這在 `pslist` 中不一定明顯，但在 `psscan` 中可以看到。

---

## 10. 本次 psscan 鑑識重點

本次 `psscan` 的重要發現如下：

1. `Rick And Morty` 仍然存在於記憶體中，是高優先可疑行程。
2. `LunarMS.exe` 仍在執行，也需要進一步確認。
3. `BitTorrent.exe` 與其子行程存在，可能與下載活動有關。
4. `WebCompanionIn` 啟動多個 `sc.exe`，可能涉及服務操作。
5. `cmd.exe` 啟動了 `ipconfig.exe`，代表有網路資訊查詢行為。
6. 多個短時間執行的 Process 在記憶體中留下痕跡。
7. 未明顯發現只存在於 `psscan` 而不存在於 `pslist` 的隱藏惡意行程。

---

## 11. 後續建議分析指令

建議下一步先執行 `cmdline`，確認可疑 Process 的完整命令：

```bash
.\vol.exe -f .\OtterCTF.vmem windows.cmdline.CmdLine
```

針對可疑 PID：

```bash
.\vol.exe -f .\OtterCTF.vmem windows.cmdline.CmdLine --pid 3820
.\vol.exe -f .\OtterCTF.vmem windows.cmdline.CmdLine --pid 708
.\vol.exe -f .\OtterCTF.vmem windows.cmdline.CmdLine --pid 3880
.\vol.exe -f .\OtterCTF.vmem windows.cmdline.CmdLine --pid 3916
.\vol.exe -f .\OtterCTF.vmem windows.cmdline.CmdLine --pid 3788
```

建議分析網路連線：

```bash
.\vol.exe -f .\OtterCTF.vmem windows.netscan.NetScan
```

建議分析服務：

```bash
.\vol.exe -f .\OtterCTF.vmem windows.svcscan.SvcScan
```

建議針對可疑行程做 DLL 與注入分析：

```bash
.\vol.exe -f .\OtterCTF.vmem windows.dlllist.DllList --pid 3820
.\vol.exe -f .\OtterCTF.vmem windows.malfind.Malfind --pid 3820

.\vol.exe -f .\OtterCTF.vmem windows.dlllist.DllList --pid 708
.\vol.exe -f .\OtterCTF.vmem windows.malfind.Malfind --pid 708
```

---

## 12. 報告用結論

本次使用 Volatility 3 的 `windows.psscan.PsScan` Plugin 對 `OtterCTF.vmem` 進行 Process 掃描分析。

分析結果顯示，`psscan` 掃描出的行程大多與前一步 `pslist` 結果一致，因此目前沒有明顯發現大量被隱藏的 Process。不過，`psscan` 額外保留了多個已結束或短時間執行的 Process 線索，例如多個 `sc.exe`、`cmd.exe`、`ipconfig.exe`、`SearchFilterHost` 與 `SearchProtocolHost`。

在可疑行程方面，`Rick And Morty`、`LunarMS.exe`、`BitTorrent.exe`、`WebCompanionIn` 與多個 `sc.exe` 仍是主要關注目標。其中 `WebCompanionIn` 啟動多個 `sc.exe`，可能代表其曾經操作 Windows Service。除此之外，`cmd.exe` 在記憶體擷取時間附近啟動 `ipconfig.exe`，代表當時可能存在網路環境查詢行為。

綜合判斷，本次 `psscan` 沒有明顯發現隱藏行程，但確認了多個短時間執行的可疑活動痕跡。後續應透過 `cmdline`、`netscan`、`svcscan`、`dlllist` 與 `malfind` 進一步交叉分析。

---

## 13. 簡短結論

`windows.psscan.PsScan` 成功掃描記憶體中的 Process 物件。

本次結果與 `pslist` 大多一致，沒有明顯 Process hiding 跡象。

但 `psscan` 額外確認了幾個重要線索：

```text
WebCompanionIn → sc.exe
cmd.exe → ipconfig.exe
Rick And Morty
LunarMS.exe
BitTorrent.exe
```

其中 `WebCompanionIn` 啟動多個 `sc.exe`，可能涉及服務操作；`cmd.exe` 啟動 `ipconfig.exe`，可能代表網路環境查詢。

後續建議優先執行：

```bash
.\vol.exe -f .\OtterCTF.vmem windows.cmdline.CmdLine
.\vol.exe -f .\OtterCTF.vmem windows.netscan.NetScan
.\vol.exe -f .\OtterCTF.vmem windows.svcscan.SvcScan
.\vol.exe -f .\OtterCTF.vmem windows.malfind.Malfind
```
