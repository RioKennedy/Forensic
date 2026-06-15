# 測試內容
- vol.exe -f .\OtterCTF.vmem windows.registry.hivelist.HiveList

```
D:\Forensic\G140A006\VolatilityWorkbench>.\vol.exe -f .\OtterCTF.vmem windows.registry.hivelist.HiveList
Volatility 3 Framework 2.5.0
Progress:  100.00               PDB scanning finished
Offset  FileFullPath    File output

0xf8a00000f010          Disabled
0xf8a000024010  \REGISTRY\MACHINE\SYSTEM        Disabled
0xf8a000053320  \REGISTRY\MACHINE\HARDWARE      Disabled
0xf8a000109410  \SystemRoot\System32\Config\SECURITY    Disabled
0xf8a00033d410  \Device\HarddiskVolume1\Boot\BCD        Disabled
0xf8a0005d5010  \SystemRoot\System32\Config\SOFTWARE    Disabled
0xf8a001495010  \SystemRoot\System32\Config\DEFAULT     Disabled
0xf8a0016d4010  \SystemRoot\System32\Config\SAM Disabled
0xf8a00175b010  \??\C:\Windows\ServiceProfiles\NetworkService\NTUSER.DAT        Disabled
0xf8a00176e410  \??\C:\Windows\ServiceProfiles\LocalService\NTUSER.DAT  Disabled
0xf8a002090010  \??\C:\Users\Rick\ntuser.dat    Disabled
0xf8a0020ad410  \??\C:\Users\Rick\AppData\Local\Microsoft\Windows\UsrClass.dat  Disabled
0xf8a00377d2d0  \??\C:\System Volume Information\Syscache.hve   Disabled
```
