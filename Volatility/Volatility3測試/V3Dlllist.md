# 測試內容
- vol.exe -f .\OtterCTF.vmem windows.dlllist.DllList
  
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
