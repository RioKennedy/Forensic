# 測試內容
- vol.exe -f .\OtterCTF.vmem windows.dlllist.DllList --pid 3820
```
D:\Forensic\G140A006\VolatilityWorkbench>.\vol.exe -f .\OtterCTF.vmem windows.dlllist.DllList --pid 3820
Volatility 3 Framework 2.5.0
Progress:  100.00               PDB scanning finished
PID     Process Base    Size    Name    Path    LoadTime        File output

3820    Rick And Morty  0x400000        0x56000 Rick And Morty season 1 download.exe    C:\Torrents\Rick And Morty season 1 download.exe        N/A     Disabled
3820    Rick And Morty  0x776f0000      0x1a9000        ntdll.dll       C:\Windows\SYSTEM32\ntdll.dll   N/A     Disabled
3820    Rick And Morty  0x75210000      0x3f000 wow64.dll       C:\Windows\SYSTEM32\wow64.dll   2018-08-04 19:32:55.000000      Disabled
3820    Rick And Morty  0x751b0000      0x5c000 wow64win.dll    C:\Windows\SYSTEM32\wow64win.dll        2018-08-04 19:32:55.000000      Disabled
3820    Rick And Morty  0x751a0000      0x8000  wow64cpu.dll    C:\Windows\SYSTEM32\wow64cpu.dll        2018-08-04 19:32:55.000000      Disabled
```

- vol.exe -f .\OtterCTF.vmem windows.dlllist.DllList --pid 3720
```
D:\Forensic\G140A006\VolatilityWorkbench>.\vol.exe -f .\OtterCTF.vmem windows.dlllist.DllList --pid 3720
Volatility 3 Framework 2.5.0
Progress:  100.00               PDB scanning finished
PID     Process Base    Size    Name    Path    LoadTime        File output

3720    vmware-tray.ex  0xec0000        0x6e000 vmware-tray.exe C:\Users\Rick\AppData\Local\Temp\RarSFX0\vmware-tray.exeN/A     Disabled
3720    vmware-tray.ex  0x776f0000      0x1a9000        ntdll.dll       C:\Windows\SYSTEM32\ntdll.dll   N/A     Disabled
3720    vmware-tray.ex  0x75210000      0x3f000 wow64.dll       C:\Windows\SYSTEM32\wow64.dll   2018-08-04 19:33:03.000000      Disabled
3720    vmware-tray.ex  0x751b0000      0x5c000 wow64win.dll    C:\Windows\SYSTEM32\wow64win.dll        2018-08-04 19:33:03.000000      Disabled
3720    vmware-tray.ex  0x751a0000      0x8000  wow64cpu.dll    C:\Windows\SYSTEM32\wow64cpu.dll        2018-08-04 19:33:03.000000      Disabled
```

- vol.exe -f .\OtterCTF.vmem windows.dlllist.DllList --pid 708
```
D:\Forensic\G140A006\VolatilityWorkbench>.\vol.exe -f .\OtterCTF.vmem windows.dlllist.DllList --pid 708
Volatility 3 Framework 2.5.0
Progress:  100.00               PDB scanning finished
PID     Process Base    Size    Name    Path    LoadTime        File output

708     LunarMS.exe     0x400000        0xa95000        LunarMS.exe     C:\Nexon\MapleStory\LunarMS.exe  N/A     Disabled
708     LunarMS.exe     0x776f0000      0x1a9000        ntdll.dll       C:\Windows\SYSTEM32\ntdll.dll    N/A     Disabled
708     LunarMS.exe     0x75210000      0x3f000 wow64.dll       C:\Windows\SYSTEM32\wow64.dll   2018-08-04 19:27:39.000000       Disabled
708     LunarMS.exe     0x751b0000      0x5c000 wow64win.dll    C:\Windows\SYSTEM32\wow64win.dll2018-08-04 19:27:39.000000       Disabled
708     LunarMS.exe     0x751a0000      0x8000  wow64cpu.dll    C:\Windows\SYSTEM32\wow64cpu.dll2018-08-04 19:27:39.000000       Disabled
```

- vol.exe -f .\OtterCTF.vmem windows.dlllist.DllList --pid 3880
```
D:\Forensic\G140A006\VolatilityWorkbench>.\vol.exe -f .\OtterCTF.vmem windows.dlllist.DllList --pid 3880
Volatility 3 Framework 2.5.0
Progress:  100.00               PDB scanning finished
PID     Process Base    Size    Name    Path    LoadTime        File output

3880    WebCompanionIn  0x300000        0x52000 WebCompanionInstaller.exe       C:\Program Files (x86)\Lavasoft\Web Companion\Application\WebCompanionInstaller.exe      N/A     Disabled
3880    WebCompanionIn  0x776f0000      0x1a9000        ntdll.dll       C:\Windows\SYSTEM32\ntdll.dll    N/A     Disabled
3880    WebCompanionIn  0x75210000      0x3f000 wow64.dll       C:\Windows\SYSTEM32\wow64.dll   2018-08-04 19:33:07.000000       Disabled
3880    WebCompanionIn  0x751b0000      0x5c000 wow64win.dll    C:\Windows\SYSTEM32\wow64win.dll2018-08-04 19:33:07.000000       Disabled
3880    WebCompanionIn  0x751a0000      0x8000  wow64cpu.dll    C:\Windows\SYSTEM32\wow64cpu.dll2018-08-04 19:33:07.000000       Disabled
```

- vol.exe -f .\OtterCTF.vmem windows.dlllist.DllList --pid 3856
```
D:\Forensic\G140A006\VolatilityWorkbench>.\vol.exe -f .\OtterCTF.vmem windows.dlllist.DllList --pid 3856
Volatility 3 Framework 2.5.0
Progress:  100.00               PDB scanning finished
PID     Process Base    Size    Name    Path    LoadTime        File output

3856    WebCompanion.e  0xf90000        0x70a000        WebCompanion.exe        C:\Program Files (x86)\Lavasoft\Web Companion\Application\WebCompanion.exe       N/A     Disabled
3856    WebCompanion.e  0x776f0000      0x1a9000        ntdll.dll       C:\Windows\SYSTEM32\ntdll.dll    N/A     Disabled
3856    WebCompanion.e  0x75210000      0x3f000 wow64.dll       C:\Windows\SYSTEM32\wow64.dll   2018-08-04 19:34:05.000000       Disabled
3856    WebCompanion.e  0x751b0000      0x5c000 wow64win.dll    C:\Windows\SYSTEM32\wow64win.dll2018-08-04 19:34:05.000000       Disabled
3856    WebCompanion.e  0x751a0000      0x8000  wow64cpu.dll    C:\Windows\SYSTEM32\wow64cpu.dll2018-08-04 19:34:05.000000       Disabled
```
