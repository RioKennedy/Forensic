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
