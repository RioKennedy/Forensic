# 測試內容
- vol.exe -f .\OtterCTF.vmem windows.verinfo.VerInfo | findstr Rick

```
D:\Forensic\G140A006\VolatilityWorkbench>.\vol.exe -f .\OtterCTF.vmem windows.verinfo.VerInfo | findstr Rick
3820ressRick And Morty  0x400000PDB scanRick And Morty season 1 download.exe    -       -       --
3820    Rick And Morty  0x776f0000      ntdll.dll       -       -       -       -
3820    Rick And Morty  0x75210000      wow64.dll       -       -       -       -
3820    Rick And Morty  0x751b0000      wow64win.dll    -       -       -       -
3820    Rick And Morty  0x751a0000      wow64cpu.dll    -       -       -       -

```
