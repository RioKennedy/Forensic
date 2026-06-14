# 測試內容

- vol.exe -f .\OtterCTF.vmem windows.ldrmodules.LdrModules --pid  3820
```
D:\Forensic\G140A006\VolatilityWorkbench>.\vol.exe -f .\OtterCTF.vmem windows.ldrmodules.LdrModules --pid 3820
Volatility 3 Framework 2.5.0
Progress:  100.00               PDB scanning finished
Pid     Process Base    InLoad  InInit  InMem   MappedPath

3820    Rick And Morty  0x400000        True    False   True    \Torrents\Rick And Morty season 1 download.exe
3820    Rick And Morty  0x240000        False   False   False   \Windows\SysWOW64\en-US\user32.dll.mui
3820    Rick And Morty  0x530000        False   False   False   \Windows\SysWOW64\en-US\propsys.dll.mui
3820    Rick And Morty  0x75210000      True    True    True    \Windows\System32\wow64.dll
3820    Rick And Morty  0x6c2d0000      False   False   False   \Windows\SysWOW64\mpr.dll
3820    Rick And Morty  0x2f80000       False   False   False   \Windows\SysWOW64\en-US\urlmon.dll.mui
3820    Rick And Morty  0x2fa0000       False   False   False   \Windows\SysWOW64\en-US\setupapi.dll.mui
3820    Rick And Morty  0x68770000      False   False   False   \Windows\SysWOW64\riched20.dll
3820    Rick And Morty  0x68870000      False   False   False   \Program Files (x86)\Common Files\microsoft shared\ink\tiptsf.dll
3820    Rick And Morty  0x68950000      False   False   False   \Windows\SysWOW64\shdocvw.dll
3820    Rick And Morty  0x73da0000      False   False   False   \Windows\SysWOW64\riched32.dll
3820    Rick And Morty  0x72ce0000      False   False   False   \Windows\SysWOW64\apphelp.dll
3820    Rick And Morty  0x6c350000      False   False   False   \Windows\AppPatch\AcLayers.dll
3820    Rick And Morty  0x6c2f0000      False   False   False   \Windows\SysWOW64\winspool.drv
3820    Rick And Morty  0x72080000      False   False   False   \Windows\SysWOW64\propsys.dll
3820    Rick And Morty  0x73c90000      False   False   False   \Windows\SysWOW64\ntmarta.dll
3820    Rick And Morty  0x73c70000      False   False   False   \Windows\SysWOW64\dwmapi.dll
3820    Rick And Morty  0x73ce0000      False   False   False   \Windows\SysWOW64\userenv.dll
3820    Rick And Morty  0x75000000      False   False   False   \Windows\winsxs\x86_microsoft.windows.common-controls_6595b64144ccf1df_6.0.7601.17514_none_41e6975e2bd6f2b2\comctl32.dll
3820    Rick And Morty  0x741a0000      False   False   False   \Windows\SysWOW64\profapi.dll
3820    Rick And Morty  0x74120000      False   False   False   \Windows\SysWOW64\uxtheme.dll
3820    Rick And Morty  0x74820000      False   False   False   \Windows\SysWOW64\version.dll
3820    Rick And Morty  0x751a0000      True    True    True    \Windows\System32\wow64cpu.dll
3820    Rick And Morty  0x751b0000      True    True    True    \Windows\System32\wow64win.dll
3820    Rick And Morty  0x76160000      False   False   False   \Windows\SysWOW64\msvcrt.dll
3820    Rick And Morty  0x75ad0000      False   False   False   \Windows\SysWOW64\usp10.dll
3820    Rick And Morty  0x756c0000      False   False   False   \Windows\SysWOW64\oleaut32.dll
3820    Rick And Morty  0x754b0000      False   False   False   \Windows\SysWOW64\rpcrt4.dll
3820    Rick And Morty  0x75430000      False   False   False   \Windows\SysWOW64\sspicli.dll
3820    Rick And Morty  0x75420000      False   False   False   \Windows\SysWOW64\cryptbase.dll
3820    Rick And Morty  0x75490000      False   False   False   \Windows\SysWOW64\devobj.dll
3820    Rick And Morty  0x755e0000      False   False   False   \Windows\SysWOW64\advapi32.dll
3820    Rick And Morty  0x75680000      False   False   False   \Windows\SysWOW64\cfgmgr32.dll
3820    Rick And Morty  0x757d0000      False   False   False   \Windows\SysWOW64\lpk.dll
3820    Rick And Morty  0x75750000      False   False   False   \Windows\SysWOW64\Wldap32.dll
3820    Rick And Morty  0x757e0000      False   False   False   \Windows\SysWOW64\wininet.dll
3820    Rick And Morty  0x759b0000      False   False   False   \Windows\SysWOW64\crypt32.dll
3820    Rick And Morty  0x75d30000      False   False   False   \Windows\SysWOW64\KernelBase.dll
3820    Rick And Morty  0x75b70000      False   False   False   \Windows\SysWOW64\comdlg32.dll
3820    Rick And Morty  0x75bf0000      False   False   False   \Windows\SysWOW64\urlmon.dll
3820    Rick And Morty  0x75de0000      False   False   False   \Windows\SysWOW64\sechost.dll
3820    Rick And Morty  0x75d80000      False   False   False   \Windows\SysWOW64\imm32.dll
3820    Rick And Morty  0x76000000      False   False   False   \Windows\SysWOW64\ole32.dll
3820    Rick And Morty  0x75e00000      False   False   False   \Windows\SysWOW64\iertutil.dll
3820    Rick And Morty  0x772f0000      False   False   False   \Windows\SysWOW64\kernel32.dll
3820    Rick And Morty  0x76f00000      False   False   False   \Windows\SysWOW64\user32.dll
3820    Rick And Morty  0x76e70000      False   False   False   \Windows\SysWOW64\gdi32.dll
3820    Rick And Morty  0x76220000      False   False   False   \Windows\SysWOW64\shell32.dll
3820    Rick And Morty  0x77200000      False   False   False   \Windows\SysWOW64\shlwapi.dll
3820    Rick And Morty  0x77060000      False   False   False   \Windows\SysWOW64\setupapi.dll
3820    Rick And Morty  0x77260000      False   False   False   \Windows\SysWOW64\clbcatq.dll
3820    Rick And Morty  0x776f0000      True    True    True    \Windows\System32\ntdll.dll
3820    Rick And Morty  0x77400000      False   False   False   \Windows\SysWOW64\msctf.dll
3820    Rick And Morty  0x778d0000      False   False   False   \Windows\SysWOW64\ntdll.dll
3820    Rick And Morty  0x778a0000      False   False   False   \Windows\SysWOW64\msasn1.dll
```

- vol.exe -f .\OtterCTF.vmem windows.ldrmodules.LdrModules --pid  3720
```
D:\Forensic\G140A006\VolatilityWorkbench>.\vol.exe -f .\OtterCTF.vmem windows.ldrmodules.LdrModules --pid 3720
Volatility 3 Framework 2.5.0
Progress:  100.00               PDB scanning finished
Pid     Process Base    InLoad  InInit  InMem   MappedPath

3720    vmware-tray.ex  0xec0000        True    False   True    \Users\Rick\AppData\Local\Temp\RarSFX0\vmware-tray.exe
3720    vmware-tray.ex  0xd90000        False   False   False   \Windows\Microsoft.NET\Framework\v4.0.30319\mscorrc.dll
3720    vmware-tray.ex  0x74a00000      False   False   False   \Windows\Microsoft.NET\Framework\v4.0.30319\mscoreei.dll
3720    vmware-tray.ex  0x66660000      False   False   False   \Windows\assembly\NativeImages_v4.0.30319_32\System.Drawing\dd57bc19f5807c6dbe8f88d4a23277f6\System.Drawing.ni.dll
3720    vmware-tray.ex  0x65330000      False   False   False   \Windows\assembly\NativeImages_v4.0.30319_32\System.Core\713647b987b140a17e3c4ffe4c721f85\System.Core.ni.dll
3720    vmware-tray.ex  0x659f0000      False   False   False   \Windows\assembly\NativeImages_v4.0.30319_32\System.Windows.Forms\17e020ae92d7fab33bcc1c98b25019d0\System.Windows.Forms.ni.dll
3720    vmware-tray.ex  0x69720000      False   False   False   \Windows\SysWOW64\msvcr100_clr0400.dll
3720    vmware-tray.ex  0x68070000      False   False   False   \Windows\Microsoft.NET\Framework\v4.0.30319\clr.dll
3720    vmware-tray.ex  0x670a0000      False   False   False   \Windows\assembly\NativeImages_v4.0.30319_32\mscorlib\246f1a5abb686b9dcdf22d3505b08cea\mscorlib.ni.dll
3720    vmware-tray.ex  0x66800000      False   False   False   \Windows\assembly\NativeImages_v4.0.30319_32\System\964da027ebca3b263a05cadb8eaa20a3\System.ni.dll
3720    vmware-tray.ex  0x68010000      False   False   False   \Windows\Microsoft.NET\Framework\v4.0.30319\clrjit.dll
3720    vmware-tray.ex  0x68860000      False   False   False   \Windows\Microsoft.NET\Framework\v4.0.30319\nlssorting.dll
3720    vmware-tray.ex  0x73fe0000      False   False   False   \Windows\winsxs\x86_microsoft.windows.common-controls_6595b64144ccf1df_5.82.7601.17514_none_ec83dffa859149af\comctl32.dll
3720    vmware-tray.ex  0x73c70000      False   False   False   \Windows\SysWOW64\dwmapi.dll
3720    vmware-tray.ex  0x71990000      False   False   False   \Windows\SysWOW64\WindowsCodecs.dll
3720    vmware-tray.ex  0x73f60000      False   False   False   \Windows\SysWOW64\bcrypt.dll
3720    vmware-tray.ex  0x741a0000      False   False   False   \Windows\SysWOW64\profapi.dll
3720    vmware-tray.ex  0x74100000      False   False   False   \Windows\SysWOW64\cryptsp.dll
3720    vmware-tray.ex  0x740c0000      False   False   False   \Windows\SysWOW64\rsaenh.dll
3720    vmware-tray.ex  0x74120000      False   False   False   \Windows\SysWOW64\uxtheme.dll
3720    vmware-tray.ex  0x74870000      False   False   False   \Windows\winsxs\x86_microsoft.windows.gdiplus_6595b64144ccf1df_1.1.7601.17514_none_72d18a4386696c80\GdiPlus.dll
3720    vmware-tray.ex  0x754b0000      False   False   False   \Windows\SysWOW64\rpcrt4.dll
3720    vmware-tray.ex  0x75210000      True    True    True    \Windows\System32\wow64.dll
3720    vmware-tray.ex  0x751a0000      True    True    True    \Windows\System32\wow64cpu.dll
3720    vmware-tray.ex  0x74f60000      False   False   False   \Windows\SysWOW64\mscoree.dll
3720    vmware-tray.ex  0x75000000      False   False   False   \Windows\winsxs\x86_microsoft.windows.common-controls_6595b64144ccf1df_6.0.7601.17514_none_41e6975e2bd6f2b2\comctl32.dll
3720    vmware-tray.ex  0x751b0000      True    True    True    \Windows\System32\wow64win.dll
3720    vmware-tray.ex  0x75430000      False   False   False   \Windows\SysWOW64\sspicli.dll
3720    vmware-tray.ex  0x75420000      False   False   False   \Windows\SysWOW64\cryptbase.dll
3720    vmware-tray.ex  0x76160000      False   False   False   \Windows\SysWOW64\msvcrt.dll
3720    vmware-tray.ex  0x75d30000      False   False   False   \Windows\SysWOW64\KernelBase.dll
3720    vmware-tray.ex  0x757d0000      False   False   False   \Windows\SysWOW64\lpk.dll
3720    vmware-tray.ex  0x755e0000      False   False   False   \Windows\SysWOW64\advapi32.dll
3720    vmware-tray.ex  0x75ad0000      False   False   False   \Windows\SysWOW64\usp10.dll
3720    vmware-tray.ex  0x75de0000      False   False   False   \Windows\SysWOW64\sechost.dll
3720    vmware-tray.ex  0x75d80000      False   False   False   \Windows\SysWOW64\imm32.dll
3720    vmware-tray.ex  0x76000000      False   False   False   \Windows\SysWOW64\ole32.dll
3720    vmware-tray.ex  0x77200000      False   False   False   \Windows\SysWOW64\shlwapi.dll
3720    vmware-tray.ex  0x76e70000      False   False   False   \Windows\SysWOW64\gdi32.dll
3720    vmware-tray.ex  0x76220000      False   False   False   \Windows\SysWOW64\shell32.dll
3720    vmware-tray.ex  0x76f00000      False   False   False   \Windows\SysWOW64\user32.dll
3720    vmware-tray.ex  0x772f0000      False   False   False   \Windows\SysWOW64\kernel32.dll
3720    vmware-tray.ex  0x77400000      False   False   False   \Windows\SysWOW64\msctf.dll
3720    vmware-tray.ex  0x776f0000      True    True    True    \Windows\System32\ntdll.dll
3720    vmware-tray.ex  0x778d0000      False   False   False   \Windows\SysWOW64\ntdll.dll
```

- vol.exe -f .\OtterCTF.vmem windows.ldrmodules.LdrModules --pid  708
```
D:\Forensic\G140A006\VolatilityWorkbench>.\vol.exe -f .\OtterCTF.vmem windows.ldrmodules.LdrModules --pid 708
Volatility 3 Framework 2.5.0
Progress:  100.00               PDB scanning finished
Pid     Process Base    InLoad  InInit  InMem   MappedPath

708     LunarMS.exe     0x400000        True    False   True    \Nexon\MapleStory\LunarMS.exe
708     LunarMS.exe     0x280000        False   False   False   \Windows\SysWOW64\en-US\setupapi.dll.mui
708     LunarMS.exe     0xee0000        False   False   False   \Nexon\MapleStory\ZLZ.dll
708     LunarMS.exe     0x11c0000       False   False   False   \Windows\SysWOW64\en-US\l3codeca.acm.mui
708     LunarMS.exe     0x2e40000       False   False   False   \Windows\SysWOW64\en-US\msacm32.dll.mui
708     LunarMS.exe     0x3070000       False   False   False   \Windows\SysWOW64\en-US\MMDevAPI.dll.mui
708     LunarMS.exe     0x3ad0000       False   False   False   \Windows\SysWOW64\en-US\wdmaud.drv.mui
708     LunarMS.exe     0x3680000       False   False   False   \Nexon\MapleStory\nmconew.dll
708     LunarMS.exe     0x4210000       False   False   False   \Nexon\MapleStory\l3codeca.acm
708     LunarMS.exe     0x45d0000       False   False   False   \Windows\SysWOW64\en-US\wshtcpip.dll.mui
708     LunarMS.exe     0x10000000      False   False   False   \Nexon\MapleStory\nmcogame.dll
708     LunarMS.exe     0x6c420000      False   False   False   \Windows\SysWOW64\netapi32.dll
708     LunarMS.exe     0x50000000      False   False   False   \Nexon\MapleStory\Canvas.dll
708     LunarMS.exe     0x21100000      False   False   False   \Nexon\MapleStory\mss32.dll
708     LunarMS.exe     0x60000000      False   False   False   \Nexon\MapleStory\ijl15.dll
708     LunarMS.exe     0x50c00000      False   False   False   \Nexon\MapleStory\PCOM.dll
708     LunarMS.exe     0x50400000      False   False   False   \Nexon\MapleStory\Gr2D_DX8.dll
708     LunarMS.exe     0x50800000      False   False   False   \Nexon\MapleStory\NameSpace.dll
708     LunarMS.exe     0x51400000      False   False   False   \Nexon\MapleStory\Shape2D.dll
708     LunarMS.exe     0x51000000      False   False   False   \Nexon\MapleStory\ResMan.dll
708     LunarMS.exe     0x51800000      False   False   False   \Nexon\MapleStory\Sound_DX8.dll
708     LunarMS.exe     0x6bd70000      False   False   False   \Users\Rick\AppData\Local\Temp\nstB3C5.tmp
708     LunarMS.exe     0x6bb70000      False   False   False   \Users\Rick\AppData\Local\Temp\nstB41B.tmp
708     LunarMS.exe     0x6b990000      False   False   False   \Windows\SysWOW64\vm3dum.dll
708     LunarMS.exe     0x6a0c0000      False   False   False   \Windows\SysWOW64\powrprof.dll
708     LunarMS.exe     0x68e90000      False   False   False   \Windows\SysWOW64\netbios.dll
708     LunarMS.exe     0x68ea0000      False   False   False   \Windows\SysWOW64\l3codeca.acm
708     LunarMS.exe     0x6a0f0000      False   False   False   \Windows\SysWOW64\dsound.dll
708     LunarMS.exe     0x6ba50000      False   False   False   \Windows\SysWOW64\d3d8thk.dll
708     LunarMS.exe     0x6ba40000      False   False   False   \Windows\SysWOW64\hid.dll
708     LunarMS.exe     0x6ba60000      False   False   False   \Windows\SysWOW64\d3d8.dll
708     LunarMS.exe     0x6bc70000      False   False   False   \Users\Rick\AppData\Local\Temp\nstB3F8.tmp
708     LunarMS.exe     0x6bbf0000      False   False   False   \Users\Rick\AppData\Local\Temp\nstB409.tmp
708     LunarMS.exe     0x6bbb0000      False   False   False   \Users\Rick\AppData\Local\Temp\nstB40A.tmp
708     LunarMS.exe     0x6bc30000      False   False   False   \Users\Rick\AppData\Local\Temp\nstB3F9.tmp
708     LunarMS.exe     0x6bcf0000      False   False   False   \Users\Rick\AppData\Local\Temp\nstB3E6.tmp
708     LunarMS.exe     0x6bcb0000      False   False   False   \Users\Rick\AppData\Local\Temp\nstB3F7.tmp
708     LunarMS.exe     0x6bd30000      False   False   False   \Users\Rick\AppData\Local\Temp\nstB3D5.tmp
708     LunarMS.exe     0x6c0a0000      False   False   False   \Windows\SysWOW64\samcli.dll
708     LunarMS.exe     0x6be10000      False   False   False   \Windows\SysWOW64\shunimpl.dll
708     LunarMS.exe     0x6bdf0000      False   False   False   \Windows\SysWOW64\icmp.dll
708     LunarMS.exe     0x6bdb0000      False   False   False   \Users\Rick\AppData\Local\Temp\nstB395.tmp
708     LunarMS.exe     0x6be00000      False   False   False   \Windows\SysWOW64\SortServer2003Compat.dll
708     LunarMS.exe     0x6c080000      False   False   False   \Windows\SysWOW64\sfc_os.dll
708     LunarMS.exe     0x6be20000      False   False   False   \Windows\AppPatch\AcXtrnal.dll
708     LunarMS.exe     0x6c090000      False   False   False   \Windows\SysWOW64\sfc.dll
708     LunarMS.exe     0x6c350000      False   False   False   \Windows\AppPatch\AcLayers.dll
708     LunarMS.exe     0x6c2d0000      False   False   False   \Windows\SysWOW64\mpr.dll
708     LunarMS.exe     0x6c0b0000      False   False   False   \Windows\AppPatch\AcGenral.dll
708     LunarMS.exe     0x6c2f0000      False   False   False   \Windows\SysWOW64\winspool.drv
708     LunarMS.exe     0x6c3f0000      False   False   False   \Windows\SysWOW64\srvcli.dll
708     LunarMS.exe     0x6c3e0000      False   False   False   \Windows\SysWOW64\wkscli.dll
708     LunarMS.exe     0x6c410000      False   False   False   \Windows\SysWOW64\netutils.dll
708     LunarMS.exe     0x75d30000      False   False   False   \Windows\SysWOW64\KernelBase.dll
708     LunarMS.exe     0x75210000      True    True    True    \Windows\System32\wow64.dll
708     LunarMS.exe     0x74080000      False   False   False   \Windows\SysWOW64\mswsock.dll
708     LunarMS.exe     0x72ce0000      False   False   False   \Windows\SysWOW64\apphelp.dll
708     LunarMS.exe     0x6e660000      False   False   False   \Windows\SysWOW64\winmm.dll
708     LunarMS.exe     0x6e600000      False   False   False   \Windows\SysWOW64\msacm32.dll
708     LunarMS.exe     0x6d850000      False   False   False   \Windows\SysWOW64\shfolder.dll
708     LunarMS.exe     0x6c440000      False   False   False   \Windows\SysWOW64\dinput8.dll
708     LunarMS.exe     0x6e460000      False   False   False   \Windows\SysWOW64\midimap.dll
708     LunarMS.exe     0x6e620000      False   False   False   \Windows\SysWOW64\msacm32.drv
708     LunarMS.exe     0x6e630000      False   False   False   \Windows\SysWOW64\wdmaud.drv
708     LunarMS.exe     0x72080000      False   False   False   \Windows\SysWOW64\propsys.dll
708     LunarMS.exe     0x71aa0000      False   False   False   \Windows\SysWOW64\ksuser.dll
708     LunarMS.exe     0x71a90000      False   False   False   \Windows\SysWOW64\avrt.dll
708     LunarMS.exe     0x72040000      False   False   False   \Windows\SysWOW64\AudioSes.dll
708     LunarMS.exe     0x72180000      False   False   False   \Windows\SysWOW64\MMDevAPI.dll
708     LunarMS.exe     0x73ce0000      False   False   False   \Windows\SysWOW64\userenv.dll
708     LunarMS.exe     0x73c90000      False   False   False   \Windows\SysWOW64\ntmarta.dll
708     LunarMS.exe     0x73c70000      False   False   False   \Windows\SysWOW64\dwmapi.dll
708     LunarMS.exe     0x73cc0000      False   False   False   \Windows\SysWOW64\dhcpcsvc.dll
708     LunarMS.exe     0x73fd0000      False   False   False   \Windows\SysWOW64\WSHTCPIP.DLL
708     LunarMS.exe     0x74820000      False   False   False   \Windows\SysWOW64\version.dll
708     LunarMS.exe     0x74120000      False   False   False   \Windows\SysWOW64\uxtheme.dll
708     LunarMS.exe     0x741a0000      False   False   False   \Windows\SysWOW64\profapi.dll
708     LunarMS.exe     0x751a0000      True    True    True    \Windows\System32\wow64cpu.dll
708     LunarMS.exe     0x74850000      False   False   False   \Windows\SysWOW64\IPHLPAPI.DLL
708     LunarMS.exe     0x74840000      False   False   False   \Windows\SysWOW64\winnsi.dll
708     LunarMS.exe     0x751b0000      True    True    True    \Windows\System32\wow64win.dll
708     LunarMS.exe     0x757d0000      False   False   False   \Windows\SysWOW64\lpk.dll
708     LunarMS.exe     0x754b0000      False   False   False   \Windows\SysWOW64\rpcrt4.dll
708     LunarMS.exe     0x75430000      False   False   False   \Windows\SysWOW64\sspicli.dll
708     LunarMS.exe     0x75420000      False   False   False   \Windows\SysWOW64\cryptbase.dll
708     LunarMS.exe     0x75490000      False   False   False   \Windows\SysWOW64\devobj.dll
708     LunarMS.exe     0x756c0000      False   False   False   \Windows\SysWOW64\oleaut32.dll
708     LunarMS.exe     0x755e0000      False   False   False   \Windows\SysWOW64\advapi32.dll
708     LunarMS.exe     0x755a0000      False   False   False   \Windows\SysWOW64\ws2_32.dll
708     LunarMS.exe     0x75680000      False   False   False   \Windows\SysWOW64\cfgmgr32.dll
708     LunarMS.exe     0x75750000      False   False   False   \Windows\SysWOW64\Wldap32.dll
708     LunarMS.exe     0x757a0000      False   False   False   \Windows\SysWOW64\wintrust.dll
708     LunarMS.exe     0x75ad0000      False   False   False   \Windows\SysWOW64\usp10.dll
708     LunarMS.exe     0x75970000      False   False   False   \Windows\SysWOW64\nsi.dll
708     LunarMS.exe     0x757e0000      False   False   False   \Windows\SysWOW64\wininet.dll
708     LunarMS.exe     0x759b0000      False   False   False   \Windows\SysWOW64\crypt32.dll
708     LunarMS.exe     0x75bf0000      False   False   False   \Windows\SysWOW64\urlmon.dll
708     LunarMS.exe     0x76f00000      False   False   False   \Windows\SysWOW64\user32.dll
708     LunarMS.exe     0x76160000      False   False   False   \Windows\SysWOW64\msvcrt.dll
708     LunarMS.exe     0x75e00000      False   False   False   \Windows\SysWOW64\iertutil.dll
708     LunarMS.exe     0x75de0000      False   False   False   \Windows\SysWOW64\sechost.dll
708     LunarMS.exe     0x75d80000      False   False   False   \Windows\SysWOW64\imm32.dll
708     LunarMS.exe     0x76000000      False   False   False   \Windows\SysWOW64\ole32.dll
708     LunarMS.exe     0x76e70000      False   False   False   \Windows\SysWOW64\gdi32.dll
708     LunarMS.exe     0x76220000      False   False   False   \Windows\SysWOW64\shell32.dll
708     LunarMS.exe     0x77200000      False   False   False   \Windows\SysWOW64\shlwapi.dll
708     LunarMS.exe     0x77060000      False   False   False   \Windows\SysWOW64\setupapi.dll
708     LunarMS.exe     0x772f0000      False   False   False   \Windows\SysWOW64\kernel32.dll
708     LunarMS.exe     0x77260000      False   False   False   \Windows\SysWOW64\clbcatq.dll
708     LunarMS.exe     0x77400000      False   False   False   \Windows\SysWOW64\msctf.dll
708     LunarMS.exe     0x778d0000      False   False   False   \Windows\SysWOW64\ntdll.dll
708     LunarMS.exe     0x776f0000      True    True    True    \Windows\System32\ntdll.dll
708     LunarMS.exe     0x778a0000      False   False   False   \Windows\SysWOW64\msasn1.dll
```

- vol.exe -f .\OtterCTF.vmem windows.ldrmodules.LdrModules --pid  3880
```
D:\Forensic\G140A006\VolatilityWorkbench>.\vol.exe -f .\OtterCTF.vmem windows.ldrmodules.LdrModules --pid 3880
Volatility 3 Framework 2.5.0
Progress:  100.00               PDB scanning finished
Pid     Process Base    InLoad  InInit  InMem   MappedPath

3880    WebCompanionIn  0x64020000      False   False   False   \Windows\Microsoft.NET\Framework\v2.0.50727\mscorsec.dll
3880    WebCompanionIn  0x300000        True    False   True    \Program Files (x86)\Lavasoft\Web Companion\Application\WebCompanionInstaller.exe
3880    WebCompanionIn  0x3c0000        False   False   False   \Windows\SysWOW64\en-US\winhttp.dll.mui
3880    WebCompanionIn  0x390000        False   False   False   \Windows\SysWOW64\en-US\crypt32.dll.mui
3880    WebCompanionIn  0xc60000        False   False   False   \Windows\Microsoft.NET\Framework\v2.0.50727\WMINet_Utils.dll
3880    WebCompanionIn  0x30f0000       False   False   False   \Windows\SysWOW64\en-US\setupapi.dll.mui
3880    WebCompanionIn  0x3ac0000       False   False   False   \Windows\SysWOW64\en-US\KernelBase.dll.mui
3880    WebCompanionIn  0x3950000       False   False   False   \Program Files (x86)\Lavasoft\Web Companion\Application\ICSharpCode.SharpZipLib.dll
3880    WebCompanionIn  0x3bf0000       False   False   False   \Windows\SysWOW64\en-US\shell32.dll.mui
3880    WebCompanionIn  0x75210000      True    True    True    \Windows\System32\wow64.dll
3880    WebCompanionIn  0x72200000      False   False   False   \Windows\assembly\NativeImages_v2.0.50727_32\WindowsBase\cf293040f3a93afa1ea782487acae816\WindowsBase.ni.dll
3880    WebCompanionIn  0x6aee0000      False   False   False   \Windows\SysWOW64\winhttp.dll
3880    WebCompanionIn  0x69f30000      False   False   False   \Windows\SysWOW64\wbemcomn.dll
3880    WebCompanionIn  0x68ae0000      False   False   False   \Windows\assembly\NativeImages_v2.0.50727_32\System.WorkflowServ#\f0f10d0591d11a36ee2aa8ee2fbdb2bf\System.WorkflowServices.ni.dll
3880    WebCompanionIn  0x689d0000      False   False   False   \Windows\assembly\NativeImages_v2.0.50727_32\System.IdentityModel\b4c60dd01be760ee0452df2c040de8fc\System.IdentityModel.ni.dll
3880    WebCompanionIn  0x69e80000      False   False   False   \Windows\SysWOW64\wbem\fastprox.dll
3880    WebCompanionIn  0x69e60000      False   False   False   \Windows\SysWOW64\ntdsapi.dll
3880    WebCompanionIn  0x69f20000      False   False   False   \Windows\SysWOW64\wbem\wbemsvc.dll
3880    WebCompanionIn  0x6a190000      False   False   False   \Windows\assembly\NativeImages_v2.0.50727_32\System.Web\da5da08245467818759aa44c4eb948e1\System.Web.ni.dll
3880    WebCompanionIn  0x69f90000      False   False   False   \Windows\SysWOW64\wbem\wmiutils.dll
3880    WebCompanionIn  0x69fb0000      False   False   False   \Windows\assembly\NativeImages_v2.0.50727_32\System.Management\6f3b99ed0b791ff4d8aa52f2f0cd0bcf\System.Management.ni.dll
3880    WebCompanionIn  0x6ace0000      False   False   False   \Windows\assembly\NativeImages_v2.0.50727_32\System.ServiceModel#\4782a5d2bc7d86895faf404a3470aacb\System.ServiceModel.Web.ni.dll
3880    WebCompanionIn  0x6ae90000      False   False   False   \Windows\SysWOW64\webio.dll
3880    WebCompanionIn  0x6e6a0000      False   False   False   \Windows\assembly\NativeImages_v2.0.50727_32\System.Xml\461d3b6b3f43e6fbe6c897d5936e17e4\System.Xml.ni.dll
3880    WebCompanionIn  0x6c4d0000      False   False   False   \Windows\assembly\NativeImages_v2.0.50727_32\System.Runtime.Seri#\4a984a9ad59d14063bc6ae64a0c8f62a\System.Runtime.Serialization.ni.dll
3880    WebCompanionIn  0x6b250000      False   False   False   \Windows\assembly\NativeImages_v2.0.50727_32\SMDiagnostics\8218dc4808b77f3585fb048c61597af1\SMDiagnostics.ni.dll
3880    WebCompanionIn  0x6b240000      False   False   False   \Windows\SysWOW64\pcwum.dll
3880    WebCompanionIn  0x6b110000      False   False   False   \Windows\SysWOW64\wbem\wbemprox.dll
3880    WebCompanionIn  0x6b9f0000      False   False   False   \Windows\SysWOW64\httpapi.dll
3880    WebCompanionIn  0x6d850000      False   False   False   \Windows\SysWOW64\shfolder.dll
3880    WebCompanionIn  0x6c720000      False   False   False   \Windows\assembly\NativeImages_v2.0.50727_32\System.ServiceModel\e2642bff810609f64343e53dddb6b59c\System.ServiceModel.ni.dll
3880    WebCompanionIn  0x6e5c0000      False   False   False   \Windows\assembly\NativeImages_v2.0.50727_32\System.ServiceProce#\20008c75bb41e2febf84d4d4aea5b4e8\System.ServiceProcess.ni.dll
3880    WebCompanionIn  0x6f5a0000      False   False   False   \Windows\assembly\NativeImages_v2.0.50727_32\PresentationFramewo#\bfaf8f86e69928fb2f67987c0203f603\PresentationFramework.ni.dll
3880    WebCompanionIn  0x6ebe0000      False   False   False   \Windows\assembly\NativeImages_v2.0.50727_32\System.Configuration\bc09ad2d49d8535371845cd7532f9271\System.Configuration.ni.dll
3880    WebCompanionIn  0x6eda0000      False   False   False   \Windows\assembly\NativeImages_v2.0.50727_32\System.Core\fbc05b5b05dc6366b02b8e2f77d080f1\System.Core.ni.dll
3880    WebCompanionIn  0x71b70000      False   False   False   \Windows\Microsoft.NET\Framework\v2.0.50727\mscorjit.dll
3880    WebCompanionIn  0x70360000      False   False   False   \Windows\assembly\NativeImages_v2.0.50727_32\PresentationCore\2ad23de8284d4594aa658dfb5e667d97\PresentationCore.ni.dll
3880    WebCompanionIn  0x71c00000      False   False   False   \Windows\Microsoft.NET\Framework\v3.0\WPF\wpfgfx_v0300.dll
3880    WebCompanionIn  0x72080000      False   False   False   \Windows\SysWOW64\propsys.dll
3880    WebCompanionIn  0x73fe0000      False   False   False   \Windows\winsxs\x86_microsoft.windows.common-controls_6595b64144ccf1df_5.82.7601.17514_none_ec83dffa859149af\comctl32.dll
3880    WebCompanionIn  0x73ce0000      False   False   False   \Windows\SysWOW64\userenv.dll
3880    WebCompanionIn  0x72f30000      False   False   False   \Windows\SysWOW64\gpapi.dll
3880    WebCompanionIn  0x72d60000      False   False   False   \Windows\SysWOW64\rtutils.dll
3880    WebCompanionIn  0x72540000      False   False   False   \Windows\assembly\NativeImages_v2.0.50727_32\System\9e0a3b9b9f457233a335d7fba8f95419\System.ni.dll
3880    WebCompanionIn  0x72ce0000      False   False   False   \Windows\SysWOW64\apphelp.dll
3880    WebCompanionIn  0x72d90000      False   False   False   \Windows\SysWOW64\rasapi32.dll
3880    WebCompanionIn  0x72d70000      False   False   False   \Windows\SysWOW64\rasman.dll
3880    WebCompanionIn  0x72ef0000      False   False   False   \Windows\SysWOW64\cryptnet.dll
3880    WebCompanionIn  0x73c20000      False   False   False   \Windows\SysWOW64\SensApi.dll
3880    WebCompanionIn  0x72fd0000      False   False   False   \Windows\assembly\NativeImages_v2.0.50727_32\mscorlib\62a0b3e4b40ec0e8c5cfaa0c8848e64a\mscorlib.ni.dll
3880    WebCompanionIn  0x73c10000      False   False   False   \Windows\SysWOW64\RpcRtRemote.dll
3880    WebCompanionIn  0x73cc0000      False   False   False   \Windows\SysWOW64\dhcpcsvc.dll
3880    WebCompanionIn  0x73f00000      False   False   False   \Windows\SysWOW64\ncrypt.dll
3880    WebCompanionIn  0x73d50000      False   False   False   \Program Files (x86)\Lavasoft\Web Companion\Application\ICSharpCode.SharpZipLib.dll
3880    WebCompanionIn  0x73d00000      False   False   False   \Windows\SysWOW64\bcryptprimitives.dll
3880    WebCompanionIn  0x73ef0000      False   False   False   \Windows\SysWOW64\credssp.dll
3880    WebCompanionIn  0x73f60000      False   False   False   \Windows\SysWOW64\bcrypt.dll
3880    WebCompanionIn  0x73f50000      False   False   False   \Windows\SysWOW64\dhcpcsvc6.dll
3880    WebCompanionIn  0x73f40000      False   False   False   \Windows\SysWOW64\rasadhlp.dll
3880    WebCompanionIn  0x73fd0000      False   False   False   \Windows\SysWOW64\WSHTCPIP.DLL
3880    WebCompanionIn  0x73f90000      False   False   False   \Windows\SysWOW64\FWPUCLNT.DLL
3880    WebCompanionIn  0x741b0000      False   False   False   \Windows\winsxs\x86_microsoft.vc80.crt_1fc8b3b9a1e18e3b_8.0.50727.4940_none_d08cc06a442b34fc\msvcr80.dll
3880    WebCompanionIn  0x74100000      False   False   False   \Windows\SysWOW64\cryptsp.dll
3880    WebCompanionIn  0x74080000      False   False   False   \Windows\SysWOW64\mswsock.dll
3880    WebCompanionIn  0x74070000      False   False   False   \Windows\SysWOW64\wship6.dll
3880    WebCompanionIn  0x740c0000      False   False   False   \Windows\SysWOW64\rsaenh.dll
3880    WebCompanionIn  0x741a0000      False   False   False   \Windows\SysWOW64\profapi.dll
3880    WebCompanionIn  0x74f60000      False   False   False   \Windows\SysWOW64\mscoree.dll
3880    WebCompanionIn  0x74850000      False   False   False   \Windows\SysWOW64\IPHLPAPI.DLL
3880    WebCompanionIn  0x74820000      False   False   False   \Windows\SysWOW64\version.dll
3880    WebCompanionIn  0x74260000      False   False   False   \Windows\Microsoft.NET\Framework\v2.0.50727\mscorwks.dll
3880    WebCompanionIn  0x74840000      False   False   False   \Windows\SysWOW64\winnsi.dll
3880    WebCompanionIn  0x74a00000      False   False   False   \Windows\Microsoft.NET\Framework\v4.0.30319\mscoreei.dll
3880    WebCompanionIn  0x751a0000      True    True    True    \Windows\System32\wow64cpu.dll
3880    WebCompanionIn  0x74fb0000      False   False   False   \Windows\SysWOW64\dnsapi.dll
3880    WebCompanionIn  0x75000000      False   False   False   \Windows\winsxs\x86_microsoft.windows.common-controls_6595b64144ccf1df_6.0.7601.17514_none_41e6975e2bd6f2b2\comctl32.dll
3880    WebCompanionIn  0x751b0000      True    True    True    \Windows\System32\wow64win.dll
3880    WebCompanionIn  0x77200000      False   False   False   \Windows\SysWOW64\shlwapi.dll
3880    WebCompanionIn  0x75750000      False   False   False   \Windows\SysWOW64\Wldap32.dll
3880    WebCompanionIn  0x754b0000      False   False   False   \Windows\SysWOW64\rpcrt4.dll
3880    WebCompanionIn  0x75430000      False   False   False   \Windows\SysWOW64\sspicli.dll
3880    WebCompanionIn  0x75420000      False   False   False   \Windows\SysWOW64\cryptbase.dll
3880    WebCompanionIn  0x75250000      False   False   False   \Windows\SysWOW64\mssprxy.dll
3880    WebCompanionIn  0x75490000      False   False   False   \Windows\SysWOW64\devobj.dll
3880    WebCompanionIn  0x755e0000      False   False   False   \Windows\SysWOW64\advapi32.dll
3880    WebCompanionIn  0x755a0000      False   False   False   \Windows\SysWOW64\ws2_32.dll
3880    WebCompanionIn  0x75680000      False   False   False   \Windows\SysWOW64\cfgmgr32.dll
3880    WebCompanionIn  0x756c0000      False   False   False   \Windows\SysWOW64\oleaut32.dll
3880    WebCompanionIn  0x75d30000      False   False   False   \Windows\SysWOW64\KernelBase.dll
3880    WebCompanionIn  0x75980000      False   False   False   \Windows\SysWOW64\imagehlp.dll
3880    WebCompanionIn  0x757d0000      False   False   False   \Windows\SysWOW64\lpk.dll
3880    WebCompanionIn  0x757a0000      False   False   False   \Windows\SysWOW64\wintrust.dll
3880    WebCompanionIn  0x75970000      False   False   False   \Windows\SysWOW64\nsi.dll
3880    WebCompanionIn  0x759b0000      False   False   False   \Windows\SysWOW64\crypt32.dll
3880    WebCompanionIn  0x75ad0000      False   False   False   \Windows\SysWOW64\usp10.dll
3880    WebCompanionIn  0x76160000      False   False   False   \Windows\SysWOW64\msvcrt.dll
3880    WebCompanionIn  0x75de0000      False   False   False   \Windows\SysWOW64\sechost.dll
3880    WebCompanionIn  0x75d80000      False   False   False   \Windows\SysWOW64\imm32.dll
3880    WebCompanionIn  0x76000000      False   False   False   \Windows\SysWOW64\ole32.dll
3880    WebCompanionIn  0x76e70000      False   False   False   \Windows\SysWOW64\gdi32.dll
3880    WebCompanionIn  0x76220000      False   False   False   \Windows\SysWOW64\shell32.dll
3880    WebCompanionIn  0x76f00000      False   False   False   \Windows\SysWOW64\user32.dll
3880    WebCompanionIn  0x77060000      False   False   False   \Windows\SysWOW64\setupapi.dll
3880    WebCompanionIn  0x778d0000      False   False   False   \Windows\SysWOW64\ntdll.dll
3880    WebCompanionIn  0x772f0000      False   False   False   \Windows\SysWOW64\kernel32.dll
3880    WebCompanionIn  0x77260000      False   False   False   \Windows\SysWOW64\clbcatq.dll
3880    WebCompanionIn  0x77400000      False   False   False   \Windows\SysWOW64\msctf.dll
3880    WebCompanionIn  0x776f0000      True    True    True    \Windows\System32\ntdll.dll
3880    WebCompanionIn  0x778a0000      False   False   False   \Windows\SysWOW64\msasn1.dll
```

- vol.exe -f .\OtterCTF.vmem windows.ldrmodules.LdrModules --pid  3856
```
D:\Forensic\G140A006\VolatilityWorkbench>.\vol.exe -f .\OtterCTF.vmem windows.ldrmodules.LdrModules --pid 3856
Volatility 3 Framework 2.5.0
Progress:  100.00               PDB scanning finished
Pid     Process Base    InLoad  InInit  InMem   MappedPath

3856    WebCompanion.e  0x741a0000      False   False   False   \Windows\SysWOW64\profapi.dll
3856    WebCompanion.e  0xf90000        True    False   True    \Program Files (x86)\Lavasoft\Web Companion\Application\WebCompanion.exe
3856    WebCompanion.e  0x3a0000        False   False   False   \Windows\SysWOW64\en-US\crypt32.dll.mui
3856    WebCompanion.e  0x4c0000        False   False   False   \Windows\SysWOW64\en-US\winhttp.dll.mui
3856    WebCompanion.e  0x750000        False   False   False   \Program Files (x86)\Lavasoft\Web Companion\Application\Lavasoft.AppCore.dll
3856    WebCompanion.e  0xb30000        False   False   False   \Program Files (x86)\Lavasoft\Web Companion\Application\Lavasoft.Utils.dll
3856    WebCompanion.e  0xba0000        False   False   False   \Program Files (x86)\Lavasoft\Web Companion\Application\log4net.dll
3856    WebCompanion.e  0xe70000        False   False   False   \Program Files (x86)\Lavasoft\Web Companion\Application\Lavasoft.SearchProtect.Business.dll
3856    WebCompanion.e  0x64020000      False   False   False   \Windows\Microsoft.NET\Framework\v2.0.50727\mscorsec.dll
3856    WebCompanion.e  0x4030000       False   False   False   \Windows\SysWOW64\en-US\KernelBase.dll.mui
3856    WebCompanion.e  0x4170000       False   False   False   \Program Files (x86)\Lavasoft\Web Companion\Application\Newtonsoft.Json.dll
3856    WebCompanion.e  0x5e3a0000      False   False   False   \Windows\Microsoft.NET\Framework\v2.0.50727\diasymreader.dll
3856    WebCompanion.e  0x72f30000      False   False   False   \Windows\SysWOW64\gpapi.dll
3856    WebCompanion.e  0x6f5a0000      False   False   False   \Windows\assembly\NativeImages_v2.0.50727_32\PresentationFramewo#\bfaf8f86e69928fb2f67987c0203f603\PresentationFramework.ni.dll
3856    WebCompanion.e  0x6e2d0000      False   False   False   \Windows\assembly\NativeImages_v2.0.50727_32\System.Drawing\dbfe8642a8ed7b2b103ad28e0c96418a\System.Drawing.ni.dll
3856    WebCompanion.e  0x6aee0000      False   False   False   \Windows\SysWOW64\winhttp.dll
3856    WebCompanion.e  0x6ae90000      False   False   False   \Windows\SysWOW64\webio.dll
3856    WebCompanion.e  0x64750000      False   False   False   \Windows\assembly\NativeImages_v2.0.50727_32\System.Windows.Forms\3afcd5168c7a6cb02eab99d7fd71e102\System.Windows.Forms.ni.dll
3856    WebCompanion.e  0x6d850000      False   False   False   \Windows\SysWOW64\shfolder.dll
3856    WebCompanion.e  0x6c720000      False   False   False   \Windows\assembly\NativeImages_v2.0.50727_32\System.ServiceModel\e2642bff810609f64343e53dddb6b59c\System.ServiceModel.ni.dll
3856    WebCompanion.e  0x6e6a0000      False   False   False   \Windows\assembly\NativeImages_v2.0.50727_32\System.Xml\461d3b6b3f43e6fbe6c897d5936e17e4\System.Xml.ni.dll
3856    WebCompanion.e  0x6e560000      False   False   False   \Program Files (x86)\Lavasoft\Web Companion\Application\Lavasoft.SearchProtect.Business.dll
3856    WebCompanion.e  0x6e4f0000      False   False   False   \Program Files (x86)\Lavasoft\Web Companion\Application\Newtonsoft.Json.dll
3856    WebCompanion.e  0x6ebe0000      False   False   False   \Windows\assembly\NativeImages_v2.0.50727_32\System.Configuration\bc09ad2d49d8535371845cd7532f9271\System.Configuration.ni.dll
3856    WebCompanion.e  0x6eda0000      False   False   False   \Windows\assembly\NativeImages_v2.0.50727_32\System.Core\fbc05b5b05dc6366b02b8e2f77d080f1\System.Core.ni.dll
3856    WebCompanion.e  0x72200000      False   False   False   \Windows\assembly\NativeImages_v2.0.50727_32\WindowsBase\cf293040f3a93afa1ea782487acae816\WindowsBase.ni.dll
3856    WebCompanion.e  0x71b70000      False   False   False   \Windows\Microsoft.NET\Framework\v2.0.50727\mscorjit.dll
3856    WebCompanion.e  0x70360000      False   False   False   \Windows\assembly\NativeImages_v2.0.50727_32\PresentationCore\2ad23de8284d4594aa658dfb5e667d97\PresentationCore.ni.dll
3856    WebCompanion.e  0x71b10000      False   False   False   \Program Files (x86)\Lavasoft\Web Companion\Application\Lavasoft.Utils.dll
3856    WebCompanion.e  0x71c00000      False   False   False   \Windows\Microsoft.NET\Framework\v3.0\WPF\wpfgfx_v0300.dll
3856    WebCompanion.e  0x72d70000      False   False   False   \Windows\SysWOW64\rasman.dll
3856    WebCompanion.e  0x72d30000      False   False   False   \Program Files (x86)\Lavasoft\Web Companion\Application\Lavasoft.AppCore.dll
3856    WebCompanion.e  0x72540000      False   False   False   \Windows\assembly\NativeImages_v2.0.50727_32\System\9e0a3b9b9f457233a335d7fba8f95419\System.ni.dll
3856    WebCompanion.e  0x72d60000      False   False   False   \Windows\SysWOW64\rtutils.dll
3856    WebCompanion.e  0x72d90000      False   False   False   \Windows\SysWOW64\rasapi32.dll
3856    WebCompanion.e  0x72ef0000      False   False   False   \Windows\SysWOW64\cryptnet.dll
3856    WebCompanion.e  0x73f00000      False   False   False   \Windows\SysWOW64\ncrypt.dll
3856    WebCompanion.e  0x73ce0000      False   False   False   \Windows\SysWOW64\userenv.dll
3856    WebCompanion.e  0x73c20000      False   False   False   \Windows\SysWOW64\SensApi.dll
3856    WebCompanion.e  0x72fd0000      False   False   False   \Windows\assembly\NativeImages_v2.0.50727_32\mscorlib\62a0b3e4b40ec0e8c5cfaa0c8848e64a\mscorlib.ni.dll
3856    WebCompanion.e  0x73c10000      False   False   False   \Windows\SysWOW64\RpcRtRemote.dll
3856    WebCompanion.e  0x73cc0000      False   False   False   \Windows\SysWOW64\dhcpcsvc.dll
3856    WebCompanion.e  0x73dc0000      False   False   False   \Program Files (x86)\Lavasoft\Web Companion\Application\log4net.dll
3856    WebCompanion.e  0x73d00000      False   False   False   \Windows\SysWOW64\bcryptprimitives.dll
3856    WebCompanion.e  0x73ef0000      False   False   False   \Windows\SysWOW64\credssp.dll
3856    WebCompanion.e  0x73fe0000      False   False   False   \Windows\winsxs\x86_microsoft.windows.common-controls_6595b64144ccf1df_5.82.7601.17514_none_ec83dffa859149af\comctl32.dll
3856    WebCompanion.e  0x73f60000      False   False   False   \Windows\SysWOW64\bcrypt.dll
3856    WebCompanion.e  0x73f50000      False   False   False   \Windows\SysWOW64\dhcpcsvc6.dll
3856    WebCompanion.e  0x73f40000      False   False   False   \Windows\SysWOW64\rasadhlp.dll
3856    WebCompanion.e  0x73fd0000      False   False   False   \Windows\SysWOW64\WSHTCPIP.DLL
3856    WebCompanion.e  0x73f90000      False   False   False   \Windows\SysWOW64\FWPUCLNT.DLL
3856    WebCompanion.e  0x740c0000      False   False   False   \Windows\SysWOW64\rsaenh.dll
3856    WebCompanion.e  0x74080000      False   False   False   \Windows\SysWOW64\mswsock.dll
3856    WebCompanion.e  0x74070000      False   False   False   \Windows\SysWOW64\wship6.dll
3856    WebCompanion.e  0x74100000      False   False   False   \Windows\SysWOW64\cryptsp.dll
3856    WebCompanion.e  0x75d30000      False   False   False   \Windows\SysWOW64\KernelBase.dll
3856    WebCompanion.e  0x75210000      True    True    True    \Windows\System32\wow64.dll
3856    WebCompanion.e  0x74a00000      False   False   False   \Windows\Microsoft.NET\Framework\v4.0.30319\mscoreei.dll
3856    WebCompanion.e  0x74260000      False   False   False   \Windows\Microsoft.NET\Framework\v2.0.50727\mscorwks.dll
3856    WebCompanion.e  0x741b0000      False   False   False   \Windows\winsxs\x86_microsoft.vc80.crt_1fc8b3b9a1e18e3b_8.0.50727.4940_none_d08cc06a442b34fc\msvcr80.dll
3856    WebCompanion.e  0x74840000      False   False   False   \Windows\SysWOW64\winnsi.dll
3856    WebCompanion.e  0x74820000      False   False   False   \Windows\SysWOW64\version.dll
3856    WebCompanion.e  0x74850000      False   False   False   \Windows\SysWOW64\IPHLPAPI.DLL
3856    WebCompanion.e  0x751a0000      True    True    True    \Windows\System32\wow64cpu.dll
3856    WebCompanion.e  0x74f60000      False   False   False   \Windows\SysWOW64\mscoree.dll
3856    WebCompanion.e  0x74fb0000      False   False   False   \Windows\SysWOW64\dnsapi.dll
3856    WebCompanion.e  0x751b0000      True    True    True    \Windows\System32\wow64win.dll
3856    WebCompanion.e  0x75750000      False   False   False   \Windows\SysWOW64\Wldap32.dll
3856    WebCompanion.e  0x754b0000      False   False   False   \Windows\SysWOW64\rpcrt4.dll
3856    WebCompanion.e  0x75430000      False   False   False   \Windows\SysWOW64\sspicli.dll
3856    WebCompanion.e  0x75420000      False   False   False   \Windows\SysWOW64\cryptbase.dll
3856    WebCompanion.e  0x755e0000      False   False   False   \Windows\SysWOW64\advapi32.dll
3856    WebCompanion.e  0x755a0000      False   False   False   \Windows\SysWOW64\ws2_32.dll
3856    WebCompanion.e  0x75680000      False   False   False   \Windows\SysWOW64\cfgmgr32.dll
3856    WebCompanion.e  0x756c0000      False   False   False   \Windows\SysWOW64\oleaut32.dll
3856    WebCompanion.e  0x75980000      False   False   False   \Windows\SysWOW64\imagehlp.dll
3856    WebCompanion.e  0x757d0000      False   False   False   \Windows\SysWOW64\lpk.dll
3856    WebCompanion.e  0x757a0000      False   False   False   \Windows\SysWOW64\wintrust.dll
3856    WebCompanion.e  0x75970000      False   False   False   \Windows\SysWOW64\nsi.dll
3856    WebCompanion.e  0x759b0000      False   False   False   \Windows\SysWOW64\crypt32.dll
3856    WebCompanion.e  0x75ad0000      False   False   False   \Windows\SysWOW64\usp10.dll
3856    WebCompanion.e  0x778d0000      False   False   False   \Windows\SysWOW64\ntdll.dll
3856    WebCompanion.e  0x77200000      False   False   False   \Windows\SysWOW64\shlwapi.dll
3856    WebCompanion.e  0x76160000      False   False   False   \Windows\SysWOW64\msvcrt.dll
3856    WebCompanion.e  0x75de0000      False   False   False   \Windows\SysWOW64\sechost.dll
3856    WebCompanion.e  0x75d80000      False   False   False   \Windows\SysWOW64\imm32.dll
3856    WebCompanion.e  0x76000000      False   False   False   \Windows\SysWOW64\ole32.dll
3856    WebCompanion.e  0x76e70000      False   False   False   \Windows\SysWOW64\gdi32.dll
3856    WebCompanion.e  0x76220000      False   False   False   \Windows\SysWOW64\shell32.dll
3856    WebCompanion.e  0x76f00000      False   False   False   \Windows\SysWOW64\user32.dll
3856    WebCompanion.e  0x772f0000      False   False   False   \Windows\SysWOW64\kernel32.dll
3856    WebCompanion.e  0x77400000      False   False   False   \Windows\SysWOW64\msctf.dll
3856    WebCompanion.e  0x776f0000      True    True    True    \Windows\System32\ntdll.dll
3856    WebCompanion.e  0x778a0000      False   False   False   \Windows\SysWOW64\msasn1.dll
```
