# 測試內容
- .\vol.exe -f .\OtterCTF.vmem windows.registry.printkey.PrintKey


```
D:\Forensic\G140A006\VolatilityWorkbench>.\vol.exe -f .\OtterCTF.vmem windows.registry.printkey.PrintKey
Volatility 3 Framework 2.5.0
Progress:  100.00               PDB scanning finished
Last Write Time Hive Offset     Type    Key     Name    Data    Volatile

2018-08-04 19:25:54.000000      0xf8a00000f010  Key     [NONAME]        A               False
2018-08-04 19:25:54.000000      0xf8a00000f010  Key     [NONAME]        MACHINE         False
2018-08-04 19:25:54.000000      0xf8a00000f010  Key     [NONAME]        USER            False
2018-08-04 19:25:54.000000      0xf8a000024010  Key     \REGISTRY\MACHINE\SYSTEM        ControlSet001            False
2018-08-04 19:25:54.000000      0xf8a000024010  Key     \REGISTRY\MACHINE\SYSTEM        ControlSet002            False
2018-08-04 19:25:54.000000      0xf8a000024010  Key     \REGISTRY\MACHINE\SYSTEM        MountedDevices           False
2018-08-04 19:25:54.000000      0xf8a000024010  Key     \REGISTRY\MACHINE\SYSTEM        RNG     False
2018-08-04 19:25:54.000000      0xf8a000024010  Key     \REGISTRY\MACHINE\SYSTEM        Select  False
2018-08-04 19:25:54.000000      0xf8a000024010  Key     \REGISTRY\MACHINE\SYSTEM        Setup   False
2018-08-04 19:25:54.000000      0xf8a000024010  Key     \REGISTRY\MACHINE\SYSTEM        SoftwareFalse
2018-08-04 19:25:54.000000      0xf8a000024010  Key     \REGISTRY\MACHINE\SYSTEM        WPA     False
2018-08-04 19:25:54.000000      0xf8a000024010  Key     \REGISTRY\MACHINE\SYSTEM        CurrentControlSet                True
2018-08-04 19:25:54.000000      0xf8a000053320  Key     \REGISTRY\MACHINE\HARDWARE      ACPI    False
2018-08-04 19:25:54.000000      0xf8a000053320  Key     \REGISTRY\MACHINE\HARDWARE      DESCRIPTION              False
2018-08-04 19:25:54.000000      0xf8a000053320  Key     \REGISTRY\MACHINE\HARDWARE      DEVICEMAPFalse
2018-08-04 19:25:54.000000      0xf8a000053320  Key     \REGISTRY\MACHINE\HARDWARE      RESOURCEMAP              True
2018-08-04 19:26:14.000000      0xf8a000109410  Key     \SystemRoot\System32\Config\SECURITY    Policy           False
2018-08-04 19:26:14.000000      0xf8a000109410  Key     \SystemRoot\System32\Config\SECURITY    RXACT            False
2018-08-04 19:26:14.000000      0xf8a000109410  Key     \SystemRoot\System32\Config\SECURITY    SAM              True
2018-08-04 19:26:04.000000      0xf8a00033d410  Key     \Device\HarddiskVolume1\Boot\BCD        Description              False
2018-08-04 19:26:04.000000      0xf8a00033d410  Key     \Device\HarddiskVolume1\Boot\BCD        Objects          False
2018-06-02 09:28:52.000000      0xf8a0005d5010  Key     \SystemRoot\System32\Config\SOFTWARE    ATI Technologies         False
2018-06-02 09:28:52.000000      0xf8a0005d5010  Key     \SystemRoot\System32\Config\SOFTWARE    CBSTEST          False
2018-06-02 09:28:52.000000      0xf8a0005d5010  Key     \SystemRoot\System32\Config\SOFTWARE    Classes          False
2018-06-02 09:28:52.000000      0xf8a0005d5010  Key     \SystemRoot\System32\Config\SOFTWARE    Clients          False
2018-06-02 09:28:52.000000      0xf8a0005d5010  Key     \SystemRoot\System32\Config\SOFTWARE    Intel            False
2018-06-02 09:28:52.000000      0xf8a0005d5010  Key     \SystemRoot\System32\Config\SOFTWARE    Microsoft                False
2018-06-02 09:28:52.000000      0xf8a0005d5010  Key     \SystemRoot\System32\Config\SOFTWARE    ODBC             False
2018-06-02 09:28:52.000000      0xf8a0005d5010  Key     \SystemRoot\System32\Config\SOFTWARE    Policies         False
2018-06-02 09:28:52.000000      0xf8a0005d5010  Key     \SystemRoot\System32\Config\SOFTWARE    RegisteredApplications           False
2018-06-02 09:28:52.000000      0xf8a0005d5010  Key     \SystemRoot\System32\Config\SOFTWARE    Sonic            False
2018-06-02 09:28:52.000000      0xf8a0005d5010  Key     \SystemRoot\System32\Config\SOFTWARE    ThinPrint                False
2018-06-02 09:28:52.000000      0xf8a0005d5010  Key     \SystemRoot\System32\Config\SOFTWARE    VMware, Inc.             False
2018-06-02 09:28:52.000000      0xf8a0005d5010  Key     \SystemRoot\System32\Config\SOFTWARE    Wow6432Node              False
2009-07-14 04:57:10.000000      0xf8a001495010  Key     \SystemRoot\System32\Config\DEFAULT     Control Panel            False
2009-07-14 04:57:10.000000      0xf8a001495010  Key     \SystemRoot\System32\Config\DEFAULT     Environment              False
2009-07-14 04:57:10.000000      0xf8a001495010  Key     \SystemRoot\System32\Config\DEFAULT     EUDC             False
2009-07-14 04:57:10.000000      0xf8a001495010  Key     \SystemRoot\System32\Config\DEFAULT     Keyboard Layout          False
2009-07-14 04:57:10.000000      0xf8a001495010  Key     \SystemRoot\System32\Config\DEFAULT     Printers         False
2009-07-14 04:57:10.000000      0xf8a001495010  Key     \SystemRoot\System32\Config\DEFAULT     Software         False
2009-07-14 04:57:10.000000      0xf8a001495010  Key     \SystemRoot\System32\Config\DEFAULT     SYSTEM           False
2009-07-14 04:45:46.000000      0xf8a0016d4010  Key     \SystemRoot\System32\Config\SAM SAM     False
2009-07-14 04:45:47.000000      0xf8a00175b010  Key     \??\C:\Windows\ServiceProfiles\NetworkService\NTUSER.DAT AppEvents               False
2009-07-14 04:45:47.000000      0xf8a00175b010  Key     \??\C:\Windows\ServiceProfiles\NetworkService\NTUSER.DAT Console         False
2009-07-14 04:45:47.000000      0xf8a00175b010  Key     \??\C:\Windows\ServiceProfiles\NetworkService\NTUSER.DAT Control Panel           False
2009-07-14 04:45:47.000000      0xf8a00175b010  Key     \??\C:\Windows\ServiceProfiles\NetworkService\NTUSER.DAT Environment             False
2009-07-14 04:45:47.000000      0xf8a00175b010  Key     \??\C:\Windows\ServiceProfiles\NetworkService\NTUSER.DAT EUDC            False
2009-07-14 04:45:47.000000      0xf8a00175b010  Key     \??\C:\Windows\ServiceProfiles\NetworkService\NTUSER.DAT Keyboard Layout         False
2009-07-14 04:45:47.000000      0xf8a00175b010  Key     \??\C:\Windows\ServiceProfiles\NetworkService\NTUSER.DAT Network         False
2009-07-14 04:45:47.000000      0xf8a00175b010  Key     \??\C:\Windows\ServiceProfiles\NetworkService\NTUSER.DAT Printers                False
2009-07-14 04:45:47.000000      0xf8a00175b010  Key     \??\C:\Windows\ServiceProfiles\NetworkService\NTUSER.DAT Software                False
2009-07-14 04:45:47.000000      0xf8a00175b010  Key     \??\C:\Windows\ServiceProfiles\NetworkService\NTUSER.DAT System          False
2009-07-14 04:45:48.000000      0xf8a00176e410  Key     \??\C:\Windows\ServiceProfiles\LocalService\NTUSER.DAT   AppEvents               False
2009-07-14 04:45:48.000000      0xf8a00176e410  Key     \??\C:\Windows\ServiceProfiles\LocalService\NTUSER.DAT   Console         False
2009-07-14 04:45:48.000000      0xf8a00176e410  Key     \??\C:\Windows\ServiceProfiles\LocalService\NTUSER.DAT   Control Panel           False
2009-07-14 04:45:48.000000      0xf8a00176e410  Key     \??\C:\Windows\ServiceProfiles\LocalService\NTUSER.DAT   Environment             False
2009-07-14 04:45:48.000000      0xf8a00176e410  Key     \??\C:\Windows\ServiceProfiles\LocalService\NTUSER.DAT   EUDC            False
2009-07-14 04:45:48.000000      0xf8a00176e410  Key     \??\C:\Windows\ServiceProfiles\LocalService\NTUSER.DAT   Keyboard Layout         False
2009-07-14 04:45:48.000000      0xf8a00176e410  Key     \??\C:\Windows\ServiceProfiles\LocalService\NTUSER.DAT   Network         False
2009-07-14 04:45:48.000000      0xf8a00176e410  Key     \??\C:\Windows\ServiceProfiles\LocalService\NTUSER.DAT   Printers                False
2009-07-14 04:45:48.000000      0xf8a00176e410  Key     \??\C:\Windows\ServiceProfiles\LocalService\NTUSER.DAT   Software                False
2009-07-14 04:45:48.000000      0xf8a00176e410  Key     \??\C:\Windows\ServiceProfiles\LocalService\NTUSER.DAT   System          False
2018-08-04 19:26:57.000000      0xf8a002090010  Key     \??\C:\Users\Rick\ntuser.dat    AppEventsFalse
2018-08-04 19:26:57.000000      0xf8a002090010  Key     \??\C:\Users\Rick\ntuser.dat    Console False
2018-08-04 19:26:57.000000      0xf8a002090010  Key     \??\C:\Users\Rick\ntuser.dat    Control Panel            False
2018-08-04 19:26:57.000000      0xf8a002090010  Key     \??\C:\Users\Rick\ntuser.dat    Environment              False
2018-08-04 19:26:57.000000      0xf8a002090010  Key     \??\C:\Users\Rick\ntuser.dat    EUDC    False
2018-08-04 19:26:57.000000      0xf8a002090010  Key     \??\C:\Users\Rick\ntuser.dat    Identities               False
2018-08-04 19:26:57.000000      0xf8a002090010  Key     \??\C:\Users\Rick\ntuser.dat    Keyboard Layout          False
2018-08-04 19:26:57.000000      0xf8a002090010  Key     \??\C:\Users\Rick\ntuser.dat    Network False
2018-08-04 19:26:57.000000      0xf8a002090010  Key     \??\C:\Users\Rick\ntuser.dat    PrintersFalse
2018-08-04 19:26:57.000000      0xf8a002090010  Key     \??\C:\Users\Rick\ntuser.dat    SoftwareFalse
2018-08-04 19:26:57.000000      0xf8a002090010  Key     \??\C:\Users\Rick\ntuser.dat    System  False
2018-08-04 19:26:57.000000      0xf8a002090010  Key     \??\C:\Users\Rick\ntuser.dat    Volatile Environment             True
2018-07-07 10:23:46.000000      0xf8a0020ad410  Key     \??\C:\Users\Rick\AppData\Local\Microsoft\Windows\UsrClass.dat   .btapp          False
2018-07-07 10:23:46.000000      0xf8a0020ad410  Key     \??\C:\Users\Rick\AppData\Local\Microsoft\Windows\UsrClass.dat   .btinstall              False
2018-07-07 10:23:46.000000      0xf8a0020ad410  Key     \??\C:\Users\Rick\AppData\Local\Microsoft\Windows\UsrClass.dat   .btkey          False
2018-07-07 10:23:46.000000      0xf8a0020ad410  Key     \??\C:\Users\Rick\AppData\Local\Microsoft\Windows\UsrClass.dat   .btsearch               False
2018-07-07 10:23:46.000000      0xf8a0020ad410  Key     \??\C:\Users\Rick\AppData\Local\Microsoft\Windows\UsrClass.dat   .btskin         False
2018-07-07 10:23:46.000000      0xf8a0020ad410  Key     \??\C:\Users\Rick\AppData\Local\Microsoft\Windows\UsrClass.dat   .htm            False
2018-07-07 10:23:46.000000      0xf8a0020ad410  Key     \??\C:\Users\Rick\AppData\Local\Microsoft\Windows\UsrClass.dat   .html           False
2018-07-07 10:23:46.000000      0xf8a0020ad410  Key     \??\C:\Users\Rick\AppData\Local\Microsoft\Windows\UsrClass.dat   .shtml          False
2018-07-07 10:23:46.000000      0xf8a0020ad410  Key     \??\C:\Users\Rick\AppData\Local\Microsoft\Windows\UsrClass.dat   .torrent                False
2018-07-07 10:23:46.000000      0xf8a0020ad410  Key     \??\C:\Users\Rick\AppData\Local\Microsoft\Windows\UsrClass.dat   .xht            False
2018-07-07 10:23:46.000000      0xf8a0020ad410  Key     \??\C:\Users\Rick\AppData\Local\Microsoft\Windows\UsrClass.dat   .xhtml          False
2018-07-07 10:23:46.000000      0xf8a0020ad410  Key     \??\C:\Users\Rick\AppData\Local\Microsoft\Windows\UsrClass.dat   Applications            False
2018-07-07 10:23:46.000000      0xf8a0020ad410  Key     \??\C:\Users\Rick\AppData\Local\Microsoft\Windows\UsrClass.dat   BitTorrent              False
2018-07-07 10:23:46.000000      0xf8a0020ad410  Key     \??\C:\Users\Rick\AppData\Local\Microsoft\Windows\UsrClass.dat   FalconBetaAccount               False
2018-07-07 10:23:46.000000      0xf8a0020ad410  Key     \??\C:\Users\Rick\AppData\Local\Microsoft\Windows\UsrClass.dat   ftp             False
2018-07-07 10:23:46.000000      0xf8a0020ad410  Key     \??\C:\Users\Rick\AppData\Local\Microsoft\Windows\UsrClass.dat   http            False
2018-07-07 10:23:46.000000      0xf8a0020ad410  Key     \??\C:\Users\Rick\AppData\Local\Microsoft\Windows\UsrClass.dat   https           False
2018-07-07 10:23:46.000000      0xf8a0020ad410  Key     \??\C:\Users\Rick\AppData\Local\Microsoft\Windows\UsrClass.dat   Local Settings          False
2018-07-07 10:23:46.000000      0xf8a0020ad410  Key     \??\C:\Users\Rick\AppData\Local\Microsoft\Windows\UsrClass.dat   Magnet          False
2018-07-07 10:23:46.000000      0xf8a0020ad410  Key     \??\C:\Users\Rick\AppData\Local\Microsoft\Windows\UsrClass.dat   MIME            False
2018-07-07 10:23:46.000000      0xf8a0020ad410  Key     \??\C:\Users\Rick\AppData\Local\Microsoft\Windows\UsrClass.dat   Software                False
2018-07-07 10:23:46.000000      0xf8a0020ad410  Key     \??\C:\Users\Rick\AppData\Local\Microsoft\Windows\UsrClass.dat   VirtualStore            False
2018-08-04 19:33:07.000000      0xf8a00377d2d0  Key     \??\C:\System Volume Information\Syscache.hve    DefaultObjectStore              False
```
