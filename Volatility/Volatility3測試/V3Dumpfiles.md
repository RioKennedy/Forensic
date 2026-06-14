# 測試內容
- vol.exe -f .\OtterCTF.vmem windows.dumpfiles.DumpFiles


```
D:\Forensic\G140A006\VolatilityWorkbench>.\vol.exe -f .\OtterCTF.vmem -o dump windows.dumpfiles.DumpFiles --physaddr 0x7d660500
Volatility 3 Framework 2.5.0
Progress:  100.00               PDB scanning finished
Cache   FileObject      FileName        Result

DataSectionObject       0x7d660500      READ_IT.txt     file.0x7d660500.0xfa801b2def10.DataSectionObject.READ_IT.txt.dat

D:\Forensic\G140A006\VolatilityWorkbench>.\vol.exe -f .\OtterCTF.vmem -o dump windows.dumpfiles.DumpFiles --physaddr 0x7d61b070
Volatility 3 Framework 2.5.0
Progress:  100.00               PDB scanning finished
Cache   FileObject      FileName        Result

DataSectionObject       0x7d61b070      Flag.txt.WINDOWS.lnk    file.0x7d61b070.0xfa801ab60450.DataSectionObject.Flag.txt.WINDOWS.lnk.dat

D:\Forensic\G140A006\VolatilityWorkbench>.\vol.exe -f .\OtterCTF.vmem -o dump windows.dumpfiles.DumpFiles --physaddr 0x7d63dbc0
Volatility 3 Framework 2.5.0
Progress:  100.00               PDB scanning finished
Cache   FileObject      FileName        Result

DataSectionObject       0x7d63dbc0      Rick And Morty season 1 download.exe    file.0x7d63dbc0.0xfa801b5a8d10.DataSectionObject.Rick And Morty season 1 download.exe.dat
ImageSectionObject      0x7d63dbc0      Rick And Morty season 1 download.exe    file.0x7d63dbc0.0xfa801a79c860.ImageSectionObject.Rick And Morty season 1 download.exe.img

D:\Forensic\G140A006\VolatilityWorkbench>.\vol.exe -f .\OtterCTF.vmem -o dump windows.dumpfiles.DumpFiles --physaddr 0x7daad840
Volatility 3 Framework 2.5.0
Progress:  100.00               PDB scanning finished
Cache   FileObject      FileName        Result

DataSectionObject       0x7daad840      vmware-tray.exe file.0x7daad840.0xfa801ab15890.DataSectionObject.vmware-tray.exe.dat
ImageSectionObject      0x7daad840      vmware-tray.exe file.0x7daad840.0xfa801b494c30.ImageSectionObject.vmware-tray.exe.img
```
