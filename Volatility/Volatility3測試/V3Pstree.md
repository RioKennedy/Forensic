# 測試內容
- vol.exe -f .\OtterCTF.vmem windows.pstree.PsTree

```
D:\Forensic\G140A006\VolatilityWorkbench>.\vol.exe -f .\OtterCTF.vmem windows.pstree.PsTree
Volatility 3 Framework 2.5.0
Progress:  100.00               PDB scanning finished
PID     PPID    ImageFileName   Offset(V)       Threads Handles SessionId       Wow64   CreateTime      ExitTime

4       0       System  0xfa8018d44740  95      411     N/A     False   2018-08-04 19:26:03.000000      N/A
* 260   4       smss.exe        0xfa801947e4d0  2       30      N/A     False   2018-08-04 19:26:03.000000      N/A
348     336     csrss.exe       0xfa801a0c8380  9       563     0       False   2018-08-04 19:26:10.000000      N/A
* 2420  348     conhost.exe     0xfa801a6643d0  0       30      0       False   2018-08-04 19:34:22.000000      2018-08-04 19:34:22.000000
388     380     csrss.exe       0xfa80198d3b30  11      460     1       False   2018-08-04 19:26:11.000000      N/A
396     336     wininit.exe     0xfa801a2ed060  3       78      0       False   2018-08-04 19:26:11.000000      N/A
* 508   396     lsm.exe 0xfa801ab461a0  10      148     0       False   2018-08-04 19:26:12.000000      N/A
* 492   396     services.exe    0xfa801ab377c0  11      242     0       False   2018-08-04 19:26:12.000000      N/A
** 1164 492     svchost.exe     0xfa801ad718a0  18      312     0       False   2018-08-04 19:26:23.000000      N/A
** 1428 492     vmtoolsd.exe    0xfa801ae92920  9       313     0       False   2018-08-04 19:26:27.000000      N/A
*** 3916        1428    cmd.exe 0xfa801a572b30  0       -       0       False   2018-08-04 19:34:22.000000      2018-08-04 19:34:22.000000
** 1948 492     svchost.exe     0xfa801afe7800  6       96      0       False   2018-08-04 19:26:42.000000      N/A
** 1436 492     msdtc.exe       0xfa801aff3b30  14      155     0       False   2018-08-04 19:26:43.000000      N/A
** 668  492     vmacthlp.exe    0xfa801abbdb30  3       56      0       False   2018-08-04 19:26:16.000000      N/A
** 412  492     mscorsvw.exe    0xfa801b603610  7       86      0       True    2018-08-04 19:28:42.000000      N/A
** 164  492     svchost.exe     0xfa801a6af9f0  12      147     0       False   2018-08-04 19:28:42.000000      N/A
** 808  492     svchost.exe     0xfa801ac2e9e0  22      508     0       False   2018-08-04 19:26:18.000000      N/A
*** 960 808     audiodg.exe     0xfa801ac753a0  7       151     0       False   2018-08-04 19:26:19.000000      N/A
** 2344 492     taskhost.exe    0xfa801b1e9b30  8       193     1       False   2018-08-04 19:26:57.000000      N/A
** 3496 492     Lavasoft.WCAss  0xfa801aad1060  14      473     0       False   2018-08-04 19:33:49.000000      N/A
** 1324 492     dllhost.exe     0xfa801ae7f630  15      207     0       False   2018-08-04 19:26:42.000000      N/A
** 3124 492     mscorsvw.exe    0xfa801a6c2700  7       77      0       False   2018-08-04 19:28:43.000000      N/A
** 2500 492     sppsvc.exe      0xfa801b232060  4       149     0       False   2018-08-04 19:26:58.000000      N/A
** 712  492     svchost.exe     0xfa801abebb30  8       301     0       False   2018-08-04 19:26:17.000000      N/A
** 844  492     svchost.exe     0xfa801ac31b30  17      396     0       False   2018-08-04 19:26:18.000000      N/A
*** 2704        844     dwm.exe 0xfa801b1fab30  4       97      1       False   2018-08-04 19:27:04.000000      N/A
** 1356 492     VGAuthService.  0xfa801ae0f630  3       85      0       False   2018-08-04 19:26:25.000000      N/A
** 724  492     PresentationFo  0xfa801988c2d0  6       148     0       False   2018-08-04 19:27:52.000000      N/A
** 604  492     svchost.exe     0xfa8018e3c890  11      376     0       False   2018-08-04 19:26:16.000000      N/A
*** 1800        604     WmiPrvSE.exe    0xfa8019124b30  9       222     0       False   2018-08-04 19:26:39.000000     N/A
*** 2136        604     WmiPrvSE.exe    0xfa801b112060  12      324     0       False   2018-08-04 19:26:51.000000     N/A
** 1120 492     spoolsv.exe     0xfa801ad5ab30  14      346     0       False   2018-08-04 19:26:22.000000      N/A
** 868  492     svchost.exe     0xfa801ac4db30  45      1114    0       False   2018-08-04 19:26:18.000000      N/A
** 620  492     svchost.exe     0xfa801acd37e0  19      415     0       False   2018-08-04 19:26:21.000000      N/A
** 1012 492     svchost.exe     0xfa801ac97060  12      554     0       False   2018-08-04 19:26:20.000000      N/A
** 3064 492     SearchIndexer.  0xfa801b3aab30  11      610     0       False   2018-08-04 19:27:14.000000      N/A
** 3196 492     svchost.exe     0xfa801a6e4b30  14      352     0       False   2018-08-04 19:28:44.000000      N/A
* 500   396     lsass.exe       0xfa801ab3f060  7       610     0       False   2018-08-04 19:26:12.000000      N/A
432     380     winlogon.exe    0xfa801aaf4060  3       113     1       False   2018-08-04 19:26:11.000000      N/A
2728    2696    explorer.exe    0xfa801b27e060  33      854     1       False   2018-08-04 19:27:04.000000      N/A
* 708   2728    LunarMS.exe     0xfa801b5cb740  18      346     1       True    2018-08-04 19:27:39.000000      N/A
* 4076  2728    chrome.exe      0xfa801a4e3870  44      1160    1       False   2018-08-04 19:29:30.000000      N/A
** 576  4076    chrome.exe      0xfa801a502b30  2       58      1       False   2018-08-04 19:29:31.000000      N/A
** 3648 4076    chrome.exe      0xfa801a635240  16      207     1       False   2018-08-04 19:33:38.000000      N/A
** 1796 4076    chrome.exe      0xfa801a5ef1f0  15      170     1       False   2018-08-04 19:33:41.000000      N/A
** 1808 4076    chrome.exe      0xfa801a4f7b30  13      229     1       False   2018-08-04 19:29:32.000000      N/A
** 4084 4076    chrome.exe      0xfa801a4eab30  8       86      1       False   2018-08-04 19:29:30.000000      N/A
** 3924 4076    chrome.exe      0xfa801aa00a90  16      228     1       False   2018-08-04 19:29:51.000000      N/A
** 2748 4076    chrome.exe      0xfa801a7f98f0  15      181     1       False   2018-08-04 19:31:15.000000      N/A
* 3820  2728    Rick And Morty  0xfa801b486b30  4       185     1       True    2018-08-04 19:32:55.000000      N/A
** 3720 3820    vmware-tray.ex  0xfa801a4c5b30  8       147     1       True    2018-08-04 19:33:02.000000      N/A
* 2804  2728    vmtoolsd.exe    0xfa801b1cdb30  6       190     1       False   2018-08-04 19:27:06.000000      N/A
* 2836  2728    BitTorrent.exe  0xfa801b290b30  24      471     1       True    2018-08-04 19:27:07.000000      N/A
** 2624 2836    bittorrentie.e  0xfa801b4c9b30  13      316     1       True    2018-08-04 19:27:21.000000      N/A
** 2308 2836    bittorrentie.e  0xfa801b4a7b30  15      337     1       True    2018-08-04 19:27:19.000000      N/A
* 2844  2728    WebCompanion.e  0xfa801b2f02e0  0       -       1       False   2018-08-04 19:27:07.000000      2018-08-04 19:33:33.000000
3880    1484    WebCompanionIn  0xfa801b18f060  15      522     0       True    2018-08-04 19:33:07.000000      N/A
* 452   3880    sc.exe  0xfa801aeb6890  0       -       0       False   2018-08-04 19:33:48.000000      2018-08-04 19:33:48.000000
* 3208  3880    sc.exe  0xfa801b08f060  0       -       0       False   2018-08-04 19:33:47.000000      2018-08-04 19:33:48.000000
* 2028  3880    sc.exe  0xfa801ac01060  0       -       0       False   2018-08-04 19:33:49.000000      2018-08-04 19:34:03.000000
* 3856  3880    WebCompanion.e  0xfa801a6268b0  15      386     0       True    2018-08-04 19:34:05.000000      N/A
* 3504  3880    sc.exe  0xfa801aa72b30  0       -       0       False   2018-08-04 19:33:48.000000      2018-08-04 19:33:48.000000
3304    3132    notepad.exe     0xfa801b1fd960  2       79      1       False   2018-08-04 19:34:10.000000      N/A
```

# windows.pstree.PsTree 分析

## 1. 執行指令

```bash
.\vol.exe -f .\OtterCTF.vmem windows.pstree.PsTree
```

---

## 2. Plugin 功能說明

`windows.pstree.PsTree` 是 Volatility 3 中用來顯示 Process 父子關係的 Plugin。

它會用樹狀結構顯示每個 Process 是由哪個父行程啟動的。

在記憶體鑑識中，`pstree` 很重要，因為它可以幫助判斷：

* 行程父子關係是否正常
* 可疑程式是由誰啟動
* 是否有異常的命令列或服務操作
* 是否有短時間執行後結束的可疑 Process

---

## 3. PsTree 星號說明

`pstree` 結果前面的 `*` 代表層級關係。

例如：

```text
2728 explorer.exe
* 708 LunarMS.exe
* 3820 Rick And Morty
```

代表 `LunarMS.exe` 和 `Rick And Morty` 都是由 `explorer.exe` 啟動。

星號越多，代表層級越深：

| 顯示方式  | 意義                |
| ----- | ----------------- |
| 無星號   | 最上層或獨立顯示的 Process |
| `*`   | 子行程               |
| `**`  | 孫行程               |
| `***` | 更下一層行程            |

---

## 4. 正常系統行程關係

本次結果中，Windows 系統核心行程關係大致正常。

```text
System
* smss.exe

wininit.exe
* services.exe
* lsass.exe
* lsm.exe
```

這些是 Windows 開機後常見的正常行程。

| Process        | 說明                    |
| -------------- | --------------------- |
| `System`       | Windows 系統核心行程        |
| `smss.exe`     | Session Manager       |
| `wininit.exe`  | Windows 初始化行程         |
| `services.exe` | Windows 服務管理程式        |
| `lsass.exe`    | 帳號驗證與安全性相關            |
| `lsm.exe`      | Local Session Manager |

目前這些系統行程的父子關係沒有明顯異常。

---

## 5. services.exe 底下的服務行程

`services.exe` 是 Windows 服務管理程式，許多系統服務都會由它啟動。

本次可看到多個服務行程：

```text
services.exe
** svchost.exe
** vmtoolsd.exe
** vmacthlp.exe
** spoolsv.exe
** SearchIndexer
** Lavasoft.WCAss
```

其中大部分是正常服務，例如 `svchost.exe`、`spoolsv.exe`、`SearchIndexer`。

但是 `Lavasoft.WCAss` 需要注意，因為它與 WebCompanion 相關，可能屬於 PUP，也就是潛在不需要程式。

---

## 6. VMware 相關行程

本次結果中可以看到 VMware 相關行程：

```text
vmtoolsd.exe
vmacthlp.exe
VGAuthService
vmware-tray.exe
```

這代表此記憶體映像檔來自 VMware 虛擬機器環境。

這也與 `OtterCTF.vmem` 的 `.vmem` 格式相符。

---

## 7. explorer.exe 底下的使用者行程

本次 `explorer.exe` 底下出現多個使用者啟動的程式：

```text
explorer.exe
* LunarMS.exe
* chrome.exe
* Rick And Morty
* vmtoolsd.exe
* BitTorrent.exe
* WebCompanion.e
```

`explorer.exe` 是 Windows 桌面行程。
如果某個程式是由 `explorer.exe` 啟動，通常代表它可能是使用者從桌面、資料夾或捷徑執行。

其中需要注意的行程有：

| Process          |  PID | 原因                  |
| ---------------- | ---: | ------------------- |
| `LunarMS.exe`    |  708 | 非 Windows 預設行程      |
| `Rick And Morty` | 3820 | 名稱可疑，非系統行程          |
| `BitTorrent.exe` | 2836 | P2P 下載軟體            |
| `WebCompanion.e` | 2844 | WebCompanion 相關，已結束 |

---

## 8. 重要可疑父子關係

| 關係 | 重點 |
|---|---|
| explorer.exe → LunarMS.exe | 非系統行程，需確認路徑與參數 |
| explorer.exe → Rick And Morty | 名稱可疑，優先分析 |
| explorer.exe → BitTorrent.exe | P2P 軟體，需搭配 netscan 查看連線 |
| WebCompanionIn → sc.exe | 可能操作 Windows Service |
| vmtoolsd.exe → cmd.exe | 短時間執行，需確認命令內容 |

---

## 9. 本次 PsTree 鑑識重點

本次 `pstree` 主要發現：

1. Windows 系統行程父子關係大致正常。
2. 此記憶體映像檔來自 VMware 虛擬機器環境。
3. `LunarMS.exe` 由 `explorer.exe` 啟動，需進一步分析。
4. `Rick And Morty` 由 `explorer.exe` 啟動，名稱可疑，是高優先分析目標。
5. `BitTorrent.exe` 由 `explorer.exe` 啟動，可能與下載活動有關。
6. `WebCompanionIn` 啟動多個 `sc.exe`，可能涉及服務操作。
7. `vmtoolsd.exe` 啟動短暫的 `cmd.exe`，需透過 `cmdline` 確認內容。
