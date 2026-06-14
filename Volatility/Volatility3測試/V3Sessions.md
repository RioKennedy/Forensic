# 測試內容
- vol.exe -f .\OtterCTF.vmem windows.sessions.Sessions

```
D:\Forensic\G140A006\VolatilityWorkbench>.\vol.exe -f .\OtterCTF.vmem windows.sessions.Sessions
Volatility 3 Framework 2.5.0
Progress:  100.00               PDB scanning finished
Session ID      Session Type    Process ID      Process User Name       Create Time

N/A     -       4       System  -       2018-08-04 19:26:03.000000
N/A     -       260     smss.exe        -       2018-08-04 19:26:03.000000
0       -       348     csrss.exe       /SYSTEM 2018-08-04 19:26:10.000000
0       -       396     wininit.exe     /SYSTEM 2018-08-04 19:26:11.000000
0       -       492     services.exe    /SYSTEM 2018-08-04 19:26:12.000000
0       -       500     lsass.exe       /SYSTEM 2018-08-04 19:26:12.000000
0       -       508     lsm.exe /SYSTEM 2018-08-04 19:26:12.000000
0       -       604     svchost.exe     WORKGROUP/WIN-LO6FAF3DTFE$      2018-08-04 19:26:16.000000
0       -       668     vmacthlp.exe    WORKGROUP/WIN-LO6FAF3DTFE$      2018-08-04 19:26:16.000000
0       -       712     svchost.exe     WORKGROUP/WIN-LO6FAF3DTFE$      2018-08-04 19:26:17.000000
0       -       808     svchost.exe     NT AUTHORITY/LOCAL SERVICE      2018-08-04 19:26:18.000000
0       -       844     svchost.exe     WORKGROUP/WIN-LO6FAF3DTFE$      2018-08-04 19:26:18.000000
0       -       868     svchost.exe     WORKGROUP/WIN-LO6FAF3DTFE$      2018-08-04 19:26:18.000000
0       -       960     audiodg.exe     -       2018-08-04 19:26:19.000000
0       -       1012    svchost.exe     NT AUTHORITY/LOCAL SERVICE      2018-08-04 19:26:20.000000
0       -       620     svchost.exe     WORKGROUP/WIN-LO6FAF3DTFE$      2018-08-04 19:26:21.000000
0       -       1120    spoolsv.exe     WORKGROUP/WIN-LO6FAF3DTFE$      2018-08-04 19:26:22.000000
0       -       1164    svchost.exe     NT AUTHORITY/LOCAL SERVICE      2018-08-04 19:26:23.000000
0       -       1356    VGAuthService.  WORKGROUP/WIN-LO6FAF3DTFE$      2018-08-04 19:26:25.000000
0       -       1428    vmtoolsd.exe    WORKGROUP/WIN-LO6FAF3DTFE$      2018-08-04 19:26:27.000000
0       -       1800    WmiPrvSE.exe    WORKGROUP/WIN-LO6FAF3DTFE$      2018-08-04 19:26:39.000000
0       -       1948    svchost.exe     NT AUTHORITY/LOCAL SERVICE      2018-08-04 19:26:42.000000
0       -       1324    dllhost.exe     WORKGROUP/WIN-LO6FAF3DTFE$      2018-08-04 19:26:42.000000
0       -       1436    msdtc.exe       WORKGROUP/WIN-LO6FAF3DTFE$      2018-08-04 19:26:43.000000
0       -       2136    WmiPrvSE.exe    WORKGROUP/WIN-LO6FAF3DTFE$      2018-08-04 19:26:51.000000
0       -       2500    sppsvc.exe      WORKGROUP/WIN-LO6FAF3DTFE$      2018-08-04 19:26:58.000000
0       -       3064    SearchIndexer.  WORKGROUP/WIN-LO6FAF3DTFE$      2018-08-04 19:27:14.000000
0       -       724     PresentationFo  NT AUTHORITY/LOCAL SERVICE      2018-08-04 19:27:52.000000
0       -       412     mscorsvw.exe    WORKGROUP/WIN-LO6FAF3DTFE$      2018-08-04 19:28:42.000000
0       -       164     svchost.exe     NT AUTHORITY/LOCAL SERVICE      2018-08-04 19:28:42.000000
0       -       3124    mscorsvw.exe    WORKGROUP/WIN-LO6FAF3DTFE$      2018-08-04 19:28:43.000000
0       -       3196    svchost.exe     WORKGROUP/WIN-LO6FAF3DTFE$      2018-08-04 19:28:44.000000
0       -       3880    WebCompanionIn  WORKGROUP/WIN-LO6FAF3DTFE$      2018-08-04 19:33:07.000000
0       -       3208    sc.exe  -       2018-08-04 19:33:47.000000
0       -       452     sc.exe  -       2018-08-04 19:33:48.000000
0       -       3504    sc.exe  -       2018-08-04 19:33:48.000000
0       -       2028    sc.exe  -       2018-08-04 19:33:49.000000
0       -       3496    Lavasoft.WCAss  WORKGROUP/WIN-LO6FAF3DTFE$      2018-08-04 19:33:49.000000
0       -       3856    WebCompanion.e  WORKGROUP/WIN-LO6FAF3DTFE$      2018-08-04 19:34:05.000000
0       -       3916    cmd.exe -       2018-08-04 19:34:22.000000
0       -       2420    conhost.exe     /SYSTEM 2018-08-04 19:34:22.000000
1       -       388     csrss.exe       /SYSTEM 2018-08-04 19:26:11.000000
1       -       432     winlogon.exe    /SYSTEM 2018-08-04 19:26:11.000000
1       -       2344    taskhost.exe    WIN-LO6FAF3DTFE/Rick    2018-08-04 19:26:57.000000
1       -       2704    dwm.exe WIN-LO6FAF3DTFE/Rick    2018-08-04 19:27:04.000000
1       Console 2728    explorer.exe    WIN-LO6FAF3DTFE/Rick    2018-08-04 19:27:04.000000
1       Console 2804    vmtoolsd.exe    WIN-LO6FAF3DTFE/Rick    2018-08-04 19:27:06.000000
1       Console 2836    BitTorrent.exe  WIN-LO6FAF3DTFE/Rick    2018-08-04 19:27:07.000000
1       -       2844    WebCompanion.e  -       2018-08-04 19:27:07.000000
1       Console 2308    bittorrentie.e  WIN-LO6FAF3DTFE/Rick    2018-08-04 19:27:19.000000
1       Console 2624    bittorrentie.e  WIN-LO6FAF3DTFE/Rick    2018-08-04 19:27:21.000000
1       -       708     LunarMS.exe     WIN-LO6FAF3DTFE/Rick    2018-08-04 19:27:39.000000
1       Console 4076    chrome.exe      WIN-LO6FAF3DTFE/Rick    2018-08-04 19:29:30.000000
1       Console 4084    chrome.exe      WIN-LO6FAF3DTFE/Rick    2018-08-04 19:29:30.000000
1       Console 576     chrome.exe      WIN-LO6FAF3DTFE/Rick    2018-08-04 19:29:31.000000
1       Console 1808    chrome.exe      WIN-LO6FAF3DTFE/Rick    2018-08-04 19:29:32.000000
1       Console 3924    chrome.exe      WIN-LO6FAF3DTFE/Rick    2018-08-04 19:29:51.000000
1       Console 2748    chrome.exe      WIN-LO6FAF3DTFE/Rick    2018-08-04 19:31:15.000000
1       Console 3820    Rick And Morty  WIN-LO6FAF3DTFE/Rick    2018-08-04 19:32:55.000000
1       -       3720    vmware-tray.ex  WIN-LO6FAF3DTFE/Rick    2018-08-04 19:33:02.000000
1       Console 3648    chrome.exe      WIN-LO6FAF3DTFE/Rick    2018-08-04 19:33:38.000000
1       Console 1796    chrome.exe      WIN-LO6FAF3DTFE/Rick    2018-08-04 19:33:41.000000
1       Console 3304    notepad.exe     WIN-LO6FAF3DTFE/Rick    2018-08-04 19:34:10.000000
```


# windows.sessions.Sessions 分析

## 1. 執行指令

```bash
.\vol.exe -f .\OtterCTF.vmem windows.sessions.Sessions
```

---

## 2. Plugin 功能簡述

`windows.sessions.Sessions` 用來查看 Process 所屬的登入 Session 與使用者帳號。

重點是判斷 Process 是屬於：

* 系統 Session
* 使用者登入 Session
* Console 使用者操作環境

---

## 3. Session ID 說明

| Session ID | 意義            |
| ---------- | ------------- |
| `N/A`      | 系統核心或早期開機行程   |
| `0`        | 系統服務 Session  |
| `1`        | 使用者登入 Session |
| `Console`  | 使用者本機桌面操作環境   |

---

## 4. 系統 Session 分析

Session `0` 主要是系統與服務行程，例如：

|  PID | Process          | User                         |
| ---: | ---------------- | ---------------------------- |
|  492 | `services.exe`   | `/SYSTEM`                    |
|  500 | `lsass.exe`      | `/SYSTEM`                    |
|  604 | `svchost.exe`    | `WORKGROUP/WIN-LO6FAF3DTFE$` |
| 1428 | `vmtoolsd.exe`   | `WORKGROUP/WIN-LO6FAF3DTFE$` |
| 3880 | `WebCompanionIn` | `WORKGROUP/WIN-LO6FAF3DTFE$` |
| 3496 | `Lavasoft.WCAss` | `WORKGROUP/WIN-LO6FAF3DTFE$` |
| 3856 | `WebCompanion.e` | `WORKGROUP/WIN-LO6FAF3DTFE$` |

重點：

```text
WebCompanionIn、Lavasoft.WCAss、WebCompanion.e 都在 Session 0。
```

代表它們偏向服務或系統層級執行環境。

---

## 5. 使用者 Session 分析

Session `1` 是使用者 `Rick` 的登入環境。

|  PID | Process          | User                   | 重點             |
| ---: | ---------------- | ---------------------- | -------------- |
| 2728 | `explorer.exe`   | `WIN-LO6FAF3DTFE/Rick` | 使用者桌面          |
| 2836 | `BitTorrent.exe` | `WIN-LO6FAF3DTFE/Rick` | P2P 下載軟體       |
| 2308 | `bittorrentie.e` | `WIN-LO6FAF3DTFE/Rick` | BitTorrent 子行程 |
| 2624 | `bittorrentie.e` | `WIN-LO6FAF3DTFE/Rick` | BitTorrent 子行程 |
|  708 | `LunarMS.exe`    | `WIN-LO6FAF3DTFE/Rick` | 使用者程式          |
| 4076 | `chrome.exe`     | `WIN-LO6FAF3DTFE/Rick` | 瀏覽器            |
| 3820 | `Rick And Morty` | `WIN-LO6FAF3DTFE/Rick` | 可疑程式           |
| 3720 | `vmware-tray.ex` | `WIN-LO6FAF3DTFE/Rick` | 可疑子行程          |
| 3304 | `notepad.exe`    | `WIN-LO6FAF3DTFE/Rick` | 開啟 Flag 檔案     |

重點：

```text
可疑程式 Rick And Morty 是在 Rick 的使用者 Session 中執行。
```

---

## 6. 重要可疑項目整理

| 關係                        | Session | 判斷                    |
| ------------------------- | ------: | --------------------- |
| `Rick → BitTorrent.exe`   |       1 | 使用者下載活動               |
| `Rick → Rick And Morty`   |       1 | 使用者執行的可疑 EXE          |
| `Rick → vmware-tray.ex`   |       1 | 與可疑程式相關               |
| `Rick → notepad.exe`      |       1 | 開啟 `Flag.txt.WINDOWS` |
| `WebCompanionIn → sc.exe` |       0 | 服務層級操作線索              |
| `vmtoolsd.exe → cmd.exe`  |       0 | 短時間命令列行為              |

---

## 7. 時間線重點

| 時間                  | Session | Process          | 重點           |
| ------------------- | ------: | ---------------- | ------------ |
| 19:27:04            |       1 | `explorer.exe`   | Rick 使用者桌面啟動 |
| 19:27:07            |       1 | `BitTorrent.exe` | P2P 下載軟體執行   |
| 19:27:39            |       1 | `LunarMS.exe`    | 使用者程式執行      |
| 19:32:55            |       1 | `Rick And Morty` | 可疑 EXE 執行    |
| 19:33:02            |       1 | `vmware-tray.ex` | 可疑子行程出現      |
| 19:33:07            |       0 | `WebCompanionIn` | 系統/服務環境執行    |
| 19:33:47 - 19:34:03 |       0 | `sc.exe`         | 服務操作線索       |
| 19:34:10            |       1 | `notepad.exe`    | 開啟 Flag 檔案   |
| 19:34:22            |       0 | `cmd.exe`        | 短時間命令列行為     |

---

## 8. 鑑識判斷

本次 `sessions` 結果確認兩個重要方向：

```text
Session 1 = Rick 使用者操作環境
Session 0 = 系統服務環境
```

`Rick And Morty`、`BitTorrent.exe`、`vmware-tray.ex`、`notepad.exe` 都屬於 `Rick` 的 Session 1。

這代表主要可疑活動與使用者 `Rick` 的登入桌面環境有關。

`WebCompanionIn`、`Lavasoft.WCAss`、`sc.exe` 則位於 Session 0，代表 WebCompanion 相關行為偏向服務層級操作。

---

## 9. 後續建議

優先分析 Rick 使用者相關行程：

```bash
.\vol.exe -f .\OtterCTF.vmem windows.dlllist.DllList --pid 3820
.\vol.exe -f .\OtterCTF.vmem windows.malfind.Malfind --pid 3820
.\vol.exe -f .\OtterCTF.vmem windows.dlllist.DllList --pid 3720
.\vol.exe -f .\OtterCTF.vmem windows.malfind.Malfind --pid 3720
```

分析服務操作：

```bash
.\vol.exe -f .\OtterCTF.vmem windows.svcscan.SvcScan
```

分析網路連線：

```bash
.\vol.exe -f .\OtterCTF.vmem windows.netscan.NetScan
```

---

## 10. 報告用結論

本次使用 `windows.sessions.Sessions` 分析 Process 所屬的登入 Session 與使用者帳號。

結果顯示，系統中主要存在兩個重要 Session：Session `0` 為系統服務環境，Session `1` 為使用者 `Rick` 的登入桌面環境。

可疑程式 `Rick And Morty`、`vmware-tray.ex`、`BitTorrent.exe` 與 `notepad.exe` 都屬於 `WIN-LO6FAF3DTFE/Rick` 的 Session `1`，代表主要可疑活動發生在 Rick 使用者操作環境中。

另一方面，`WebCompanionIn`、`Lavasoft.WCAss` 與多個 `sc.exe` 位於 Session `0`，顯示 WebCompanion 相關行為可能涉及系統服務操作。

綜合判斷，本次 `sessions` 結果補強了前面分析：可疑 EXE 與 Flag 檔案線索主要屬於 Rick 使用者環境，而 WebCompanion 相關行為則偏向服務層級活動。

---

## 11. 簡短結論

本次最重要的 Session 關係如下：

```text
Session 1 → Rick → Rick And Morty
Session 1 → Rick → vmware-tray.ex
Session 1 → Rick → notepad.exe → Flag.txt.WINDOWS
Session 0 → WebCompanionIn → sc.exe
```

因此，主要可疑活動可分成兩條線：

```text
Rick 使用者線：Rick And Morty、vmware-tray.ex、Flag.txt.WINDOWS
服務操作線：WebCompanionIn、sc.exe、Lavasoft.WCAss
```
