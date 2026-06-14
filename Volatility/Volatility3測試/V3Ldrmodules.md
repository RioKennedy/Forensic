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

# windows.ldrmodules.LdrModules 分析

## 1. Plugin 分析目的

`windows.ldrmodules.LdrModules` 主要用來檢查 Process 載入的模組是否存在於 Windows Loader List 中。

分析時重點不是單純看 `True` 或 `False`，而是要觀察：

* 模組路徑是否合理
* 是否有從 Temp 目錄載入模組
* 是否有偽裝成正常程式的路徑
* 是否有大量不尋常的第三方模組
* 模組是否與該 Process 的用途相符

---

## 2. 欄位簡要說明

| 欄位           | 說明                              |
| ------------ | ------------------------------- |
| `InLoad`     | 模組是否在 Load Order List           |
| `InInit`     | 模組是否在 Initialization Order List |
| `InMem`      | 模組是否在 Memory Order List         |
| `MappedPath` | 模組對應路徑                          |

`False False False` 不一定代表惡意，仍需搭配路徑與 Process 行為判斷。

---

## 3. PID 3820 - Rick And Morty 分析

### 3.1 主要發現

```text
Process: Rick And Morty
Path: \Torrents\Rick And Morty season 1 download.exe
```

此 Process 的主程式位於 `\Torrents` 目錄，檔名看起來像影片下載，但實際上是 `.exe` 可執行檔。

### 3.2 模組載入狀況

`Rick And Morty` 載入大量 Windows 32-bit 系統模組，例如：

```text
\Windows\SysWOW64\kernel32.dll
\Windows\SysWOW64\user32.dll
\Windows\SysWOW64\shell32.dll
\Windows\SysWOW64\wininet.dll
\Windows\SysWOW64\urlmon.dll
\Windows\SysWOW64\crypt32.dll
```

其中 `wininet.dll`、`urlmon.dll`、`crypt32.dll` 代表程式可能具備網路、URL 存取或憑證相關功能。

### 3.3 分析判斷

此 Process 的可疑點不在於載入了特殊 DLL，而是在於主程式本身的命名與路徑。

```text
\Torrents\Rick And Morty season 1 download.exe
```

此檔案名稱具有偽裝性，容易讓使用者誤以為是影片檔案，但實際上是執行檔。因此，`Rick And Morty` 是本次 `LdrModules` 分析中最高優先的可疑 Process。

### 3.4 判斷結果

| 項目    | 判斷               |
| ----- | ---------------- |
| 主程式路徑 | 可疑               |
| 檔名    | 偽裝成影片下載          |
| 載入模組  | 多數為 Windows 系統模組 |
| 可疑程度  | 高                |

---

## 4. PID 3720 - vmware-tray.exe 分析

### 4.1 主要發現

```text
Process: vmware-tray.exe
Path: \Users\Rick\AppData\Local\Temp\RarSFX0\vmware-tray.exe
```

此 Process 名稱看似 VMware Tools 相關程式，但執行路徑位於使用者 Temp 目錄。

正常 VMware Tools 程式通常應位於：

```text
C:\Program Files\VMware\VMware Tools\
```

但本次發現的路徑是：

```text
C:\Users\Rick\AppData\Local\Temp\RarSFX0\
```

### 4.2 模組載入狀況

`vmware-tray.exe` 載入多個 .NET Framework 相關模組：

```text
\Windows\Microsoft.NET\Framework\v4.0.30319\clr.dll
\Windows\Microsoft.NET\Framework\v4.0.30319\clrjit.dll
\Windows\Microsoft.NET\Framework\v4.0.30319\mscoreei.dll
\Windows\assembly\NativeImages_v4.0.30319_32\System.Windows.Forms\
\Windows\assembly\NativeImages_v4.0.30319_32\System.Drawing\
```

這代表該程式很可能是 .NET 程式，並且可能具有圖形介面功能。

### 4.3 分析判斷

`vmware-tray.exe` 的名稱具有偽裝性，因為它看起來像 VMware 元件，但實際執行位置並非 VMware 正常安裝目錄。

`RarSFX0` 通常與自解壓縮檔或臨時釋放檔案有關，因此此程式可能是由其他可疑程式釋放出來後執行。

### 4.4 判斷結果

| 項目    | 判斷                  |
| ----- | ------------------- |
| 主程式路徑 | 高度可疑                |
| 檔名    | 偽裝成 VMware 元件       |
| 載入模組  | .NET Framework 相關模組 |
| 可疑程度  | 高                   |

---

## 5. PID 708 - LunarMS.exe 分析

### 5.1 主要發現

```text
Process: LunarMS.exe
Path: \Nexon\MapleStory\LunarMS.exe
```

此 Process 位於 MapleStory 相關目錄，從主程式路徑來看，較像遊戲程式。

### 5.2 遊戲相關模組

`LunarMS.exe` 載入多個遊戲相關模組，例如：

```text
\Nexon\MapleStory\ZLZ.dll
\Nexon\MapleStory\nmconew.dll
\Nexon\MapleStory\nmcogame.dll
\Nexon\MapleStory\Canvas.dll
\Nexon\MapleStory\PCOM.dll
\Nexon\MapleStory\Gr2D_DX8.dll
\Nexon\MapleStory\Sound_DX8.dll
```

這些模組與遊戲執行環境相符。

### 5.3 Temp 模組

但此 Process 同時載入多個使用者 Temp 目錄下的 `.tmp` 模組：

```text
\Users\Rick\AppData\Local\Temp\nstB3C5.tmp
\Users\Rick\AppData\Local\Temp\nstB41B.tmp
\Users\Rick\AppData\Local\Temp\nstB3F8.tmp
\Users\Rick\AppData\Local\Temp\nstB409.tmp
\Users\Rick\AppData\Local\Temp\nstB40A.tmp
\Users\Rick\AppData\Local\Temp\nstB3F9.tmp
\Users\Rick\AppData\Local\Temp\nstB3E6.tmp
\Users\Rick\AppData\Local\Temp\nstB3F7.tmp
\Users\Rick\AppData\Local\Temp\nstB3D5.tmp
\Users\Rick\AppData\Local\Temp\nstB395.tmp
```

### 5.4 分析判斷

`LunarMS.exe` 本身不像 `Rick And Morty` 那樣直接可疑，但載入多個 Temp `.tmp` 模組需要注意。

這些 `.tmp` 模組可能是遊戲保護、安裝暫存、外掛、補丁或臨時載入模組。但在鑑識分析中，從 Temp 載入模組仍然需要進一步確認，因為惡意程式也常使用 Temp 目錄放置或載入模組。

### 5.5 判斷結果

| 項目             | 判斷              |
| -------------- | --------------- |
| 主程式路徑          | 較合理             |
| 遊戲 DLL         | 與 MapleStory 相符 |
| Temp `.tmp` 模組 | 需要注意            |
| 可疑程度           | 中               |

---

## 6. PID 3880 - WebCompanionInstaller.exe 分析

### 6.1 主要發現

```text
Process: WebCompanionInstaller.exe
Path: \Program Files (x86)\Lavasoft\Web Companion\Application\WebCompanionInstaller.exe
```

此 Process 為 WebCompanion 安裝或更新程式。

### 6.2 模組載入特徵

`WebCompanionInstaller.exe` 載入多種類型模組：

```text
.NET Framework 模組
WMI 相關模組
Web / HTTP 相關模組
壓縮函式庫
ServiceProcess 相關模組
```

較重要的模組包括：

```text
\Windows\SysWOW64\wbem\wbemprox.dll
\Windows\SysWOW64\wbem\wbemsvc.dll
\Windows\SysWOW64\wbem\fastprox.dll
\Windows\SysWOW64\winhttp.dll
\Windows\SysWOW64\httpapi.dll
\Program Files (x86)\Lavasoft\Web Companion\Application\ICSharpCode.SharpZipLib.dll
\Windows\assembly\NativeImages_v2.0.50727_32\System.ServiceProcess\
```

### 6.3 分析判斷

這些模組符合安裝程式或更新程式常見行為，例如：

```text
查詢系統資訊
連線下載資料
解壓縮安裝檔案
操作或建立服務
```

其中 `ICSharpCode.SharpZipLib.dll` 顯示它可能有解壓縮功能；WMI 與 ServiceProcess 模組則表示它可能查詢系統狀態或操作服務。

### 6.4 判斷結果

| 項目    | 判斷                   |
| ----- | -------------------- |
| 主程式路徑 | WebCompanion 安裝目錄    |
| 行為特徵  | 安裝 / 更新 / 解壓縮 / 服務操作 |
| 可疑程度  | 中                    |
| 主要風險  | PUP 或服務操作行為          |

---

## 7. PID 3856 - WebCompanion.exe 分析

### 7.1 主要發現

```text
Process: WebCompanion.exe
Path: \Program Files (x86)\Lavasoft\Web Companion\Application\WebCompanion.exe
```

此 Process 是 WebCompanion 主程式。

### 7.2 Lavasoft 相關模組

`WebCompanion.exe` 載入多個 Lavasoft 模組：

```text
Lavasoft.AppCore.dll
Lavasoft.Utils.dll
Lavasoft.SearchProtect.Business.dll
log4net.dll
Newtonsoft.Json.dll
```

其中比較需要注意的是：

```text
Lavasoft.SearchProtect.Business.dll
```

此模組名稱顯示它可能與搜尋保護、瀏覽器設定保護或 SearchProtect 類功能有關。

### 7.3 分析判斷

`WebCompanion.exe` 的路徑與 WebCompanion 安裝目錄相符，因此不屬於路徑偽裝型可疑程式。

但它載入 SearchProtect 相關模組，且與 WebCompanionInstaller、Lavasoft.WCAssistant、服務操作線索有關，因此可列為 PUP 類或輔助分析目標。

### 7.4 判斷結果

| 項目               | 判斷                |
| ---------------- | ----------------- |
| 主程式路徑            | 合理                |
| Lavasoft 模組      | 與 WebCompanion 相符 |
| SearchProtect 模組 | 需要注意              |
| 可疑程度             | 中低                |

---

## 8. 綜合分析

本次 `LdrModules` 分析中，最重要的發現是兩條線索。

第一條是主要可疑執行鏈：

```text
Rick And Morty → vmware-tray.exe
```

其可疑路徑為：

```text
\Torrents\Rick And Morty season 1 download.exe
\Users\Rick\AppData\Local\Temp\RarSFX0\vmware-tray.exe
```

`Rick And Morty` 偽裝成影片下載檔，但實際是 EXE；`vmware-tray.exe` 則偽裝成 VMware 元件，卻從 Temp 自解壓目錄執行。兩者可疑程度最高。

第二條是輔助可疑線索：

```text
LunarMS.exe → Temp\nst*.tmp
```

`LunarMS.exe` 本身像遊戲程式，但載入多個 Temp `.tmp` 模組，仍需要進一步確認。

WebCompanion 相關行程則較像安裝、更新與服務操作行為。其可疑程度低於 `Rick And Morty` 執行鏈，但仍應注意其 PUP 與 SearchProtect 特徵。

---

## 9. 可疑程度排序

| 排名 |  PID | Process                     | 可疑程度 | 原因                              |
| -: | ---: | --------------------------- | ---- | ------------------------------- |
|  1 | 3820 | `Rick And Morty`            | 高    | 偽裝成影片下載的 EXE                    |
|  2 | 3720 | `vmware-tray.exe`           | 高    | 從 Temp `RarSFX0` 執行，偽裝 VMware   |
|  3 |  708 | `LunarMS.exe`               | 中    | 載入多個 Temp `.tmp` 模組             |
|  4 | 3880 | `WebCompanionInstaller.exe` | 中    | 安裝、更新、WMI、服務操作                  |
|  5 | 3856 | `WebCompanion.exe`          | 中低   | WebCompanion / SearchProtect 相關 |

---

## 10. 結論

`LdrModules` 結果顯示，最主要的可疑目標為 `PID 3820 Rick And Morty` 與 `PID 3720 vmware-tray.exe`。

`Rick And Morty` 的主程式位於：

```text
\Torrents\Rick And Morty season 1 download.exe
```

此檔案名稱具有偽裝性，實際上是可執行檔，且與 torrent 下載目錄有關。

`vmware-tray.exe` 位於：

```text
\Users\Rick\AppData\Local\Temp\RarSFX0\vmware-tray.exe
```

此路徑不屬於正常 VMware Tools 安裝目錄，且位於使用者 Temp 自解壓目錄，因此高度可疑。

另外，`LunarMS.exe` 載入多個：

```text
\Users\Rick\AppData\Local\Temp\nst*.tmp
```

雖然可能與遊戲或安裝暫存有關，但仍需要進一步確認。

整體而言，本次 `LdrModules` 分析支持以下判斷：

```text
Rick And Morty season 1 download.exe 是主要可疑程式。
vmware-tray.exe 是其可疑子程式。
LunarMS.exe 需要補充檢查 Temp 模組。
WebCompanion 相關行程偏向 PUP / 安裝更新 / 服務操作。
```

