# 測試內容
- vol.exe -f .\OtterCTF.vmem windows.vadinfo.VadInfo --pid 3820


```
D:\Forensic\G140A006\VolatilityWorkbench>.\vol.exe -f .\OtterCTF.vmem windows.vadinfo.VadInfo --pid 3820
Volatility 3 Framework 2.5.0
Progress:  100.00               PDB scanning finished
PID     Process Offset  Start VPN       End VPN Tag     Protection      CommitCharge    PrivateMemory    Parent  File    File output

3820    Rick And Morty  0xfffffa801a7b7010      0x22d0000       0x230ffff       VadS    PAGE_READWRITE   36      1       0xfa801b486f78  N/A     Disabled
3820    Rick And Morty  0xfffffa8018d71f70      0x400000        0x455fff        Vadm    PAGE_EXECUTE_WRITECOPY   35      0       0xfa801a7b7010  \Torrents\Rick And Morty season 1 download.exe  Disabled
3820    Rick And Morty  0xfffffa801abb0550      0x250000        0x251fff        Vad     PAGE_READONLY    0       0       0xfa8018d71f70  N/A     Disabled
3820    Rick And Morty  0xfffffa801a627e80      0x190000        0x193fff        Vad     PAGE_READONLY    0       0       0xfa801abb0550  N/A     Disabled
3820    Rick And Morty  0xfffffa801b46a6a0      0x40000 0x40fff Vad     PAGE_EXECUTE_WRITECOPY  00       0xfa801a627e80  \Windows\System32\apisetschema.dll      Disabled
3820    Rick And Morty  0xfffffa801aa92f70      0x20000 0x20fff Vadm    PAGE_READWRITE  1       10xfa801b46a6a0  N/A     Disabled
3820    Rick And Morty  0xfffffa801b46c5c0      0x10000 0x1ffff Vad     PAGE_READWRITE  0       00xfa801aa92f70  N/A     Disabled
3820    Rick And Morty  0xfffffa801aa9e010      0x30000 0x30fff Vadm    PAGE_READWRITE  1       10xfa801aa92f70  N/A     Disabled
3820    Rick And Morty  0xfffffa801aadd420      0x50000 0x8ffff VadS    PAGE_READWRITE  11      10xfa801b46a6a0  N/A     Disabled
3820    Rick And Morty  0xfffffa801a7b4be0      0x90000 0x18ffff        VadS    PAGE_READWRITE  51       1       0xfa801aadd420  N/A     Disabled
3820    Rick And Morty  0xfffffa801a577ac0      0x1d0000        0x236fff        Vad     PAGE_READONLY    0       0       0xfa801a627e80  \Windows\System32\locale.nls    Disabled
3820    Rick And Morty  0xfffffa801a53f850      0x1b0000        0x1b0fff        VadS    PAGE_READWRITE   1       1       0xfa801a577ac0  N/A     Disabled
3820    Rick And Morty  0xfffffa801b491b40      0x1a0000        0x1a2fff        Vad     PAGE_READONLY    0       0       0xfa801a53f850  N/A     Disabled
3820    Rick And Morty  0xfffffa801a586190      0x1c0000        0x1c0fff        VadS    PAGE_READWRITE   1       1       0xfa801a53f850  N/A     Disabled
3820    Rick And Morty  0xfffffa801aa97730      0x240000        0x244fff        Vad     PAGE_WRITECOPY   5       0       0xfa801a577ac0  \Windows\SysWOW64\en-US\user32.dll.mui  Disabled
3820    Rick And Morty  0xfffffa801a7a9b10      0x2d0000        0x2dffff        VadS    PAGE_NOACCESS    1       1       0xfa801abb0550  N/A     Disabled
3820    Rick And Morty  0xfffffa801a7f42c0      0x2a0000        0x2affff        VadS    PAGE_READWRITE   3       1       0xfa801a7a9b10  N/A     Disabled
3820    Rick And Morty  0xfffffa801a51e1e0      0x270000        0x27ffff        VadS    PAGE_READWRITE   11      1       0xfa801a7f42c0  N/A     Disabled
3820    Rick And Morty  0xfffffa801a5251e0      0x260000        0x260fff        Vad     PAGE_READONLY    0       0       0xfa801a51e1e0  N/A     Disabled
3820    Rick And Morty  0xfffffa801a785170      0x280000        0x29ffff        VadS    PAGE_READWRITE   1       1       0xfa801a51e1e0  N/A     Disabled
3820    Rick And Morty  0xfffffa801a56fd40      0x2c0000        0x2c6fff        Vad     PAGE_READONLY    0       0       0xfa801a7f42c0  \Windows\Registration\R000000000006.clb Disabled
3820    Rick And Morty  0xfffffa801b0b2880      0x2b0000        0x2b0fff        Vad     PAGE_READONLY    0       0       0xfa801a56fd40  N/A     Disabled
3820    Rick And Morty  0xfffffa801b418510      0x320000        0x320fff        Vad     PAGE_READWRITE   0       0       0xfa801a7a9b10  N/A     Disabled
3820    Rick And Morty  0xfffffa801a556790      0x2f0000        0x2fffff        VadS    PAGE_READWRITE   1       1       0xfa801b418510  N/A     Disabled
3820    Rick And Morty  0xfffffa801aadb1a0      0x2e0000        0x2e1fff        Vad     PAGE_READONLY    0       0       0xfa801a556790  N/A     Disabled
3820    Rick And Morty  0xfffffa801a5baa60      0x300000        0x300fff        Vad     PAGE_READWRITE   0       0       0xfa801a556790  N/A     Disabled
3820    Rick And Morty  0xfffffa801a79c6b0      0x310000        0x313fff        Vad     PAGE_READONLY    0       0       0xfa801a5baa60  \ProgramData\Microsoft\Windows\Caches\cversions.2.db    Disabled
3820    Rick And Morty  0xfffffa801a528680      0x3b0000        0x3cbfff        Vad     PAGE_READONLY    0       0       0xfa801b418510  \Users\Rick\AppData\Local\Microsoft\Windows\Caches\{AFBF9F1A-8EE8-4C77-AF34-C647E37CA0D9}.1.ver0x0000000000000005.db     Disabled
3820    Rick And Morty  0xfffffa801a562a30      0x330000        0x3affff        VadS    PAGE_READWRITE   6       1       0xfa801a528680  N/A     Disabled
3820    Rick And Morty  0xfffffa801a56f0c0      0x3d0000        0x3fffff        Vad     PAGE_READONLY    0       0       0xfa801a528680  \ProgramData\Microsoft\Windows\Caches\{6AF0698E-D558-4F6E-9B3C-3716689AF493}.2.ver0x000000000000000a.db  Disabled
3820    Rick And Morty  0xfffffa801a53d240      0x540000        0x54ffff        VadS    PAGE_READWRITE   11      1       0xfa8018d71f70  N/A     Disabled
3820    Rick And Morty  0xfffffa801a7caeb0      0x4e0000        0x4e3fff        Vad     PAGE_READONLY    0       0       0xfa801a53d240  \ProgramData\Microsoft\Windows\Caches\cversions.2.db    Disabled
3820    Rick And Morty  0xfffffa801a541880      0x460000        0x4dffff        VadS    PAGE_READWRITE   1       1       0xfa801a7caeb0  N/A     Disabled
3820    Rick And Morty  0xfffffa801a593fc0      0x4f0000        0x52ffff        VadS    PAGE_READWRITE   27      1       0xfa801a7caeb0  N/A     Disabled
3820    Rick And Morty  0xfffffa801afcca20      0x530000        0x53dfff        Vad     PAGE_WRITECOPY   14      0       0xfa801a593fc0  \Windows\SysWOW64\en-US\propsys.dll.mui Disabled
3820    Rick And Morty  0xfffffa801b00d0b0      0x9e0000        0x1ddffff       Vad     PAGE_READONLY    0       0       0xfa801a53d240  N/A     Disabled
3820    Rick And Morty  0xfffffa801a585ac0      0x6c0000        0x847fff        Vad     PAGE_READONLY    0       0       0xfa801b00d0b0  N/A     Disabled
3820    Rick And Morty  0xfffffa801acefb90      0x5c0000        0x6bffff        Vadm    PAGE_READWRITE   161     1       0xfa801a585ac0  N/A     Disabled
3820    Rick And Morty  0xfffffa801a7e82c0      0x550000        0x5b5fff        Vad     PAGE_READONLY    0       0       0xfa801acefb90  \ProgramData\Microsoft\Windows\Caches\{DDF571F2-BE98-426D-8288-1A9A39C3FDA2}.2.ver0x0000000000000002.db  Disabled
3820    Rick And Morty  0xfffffa801a7f2660      0x850000        0x9d0fff        Vadm    PAGE_READONLY    0       0       0xfa801a585ac0  N/A     Disabled
3820    Rick And Morty  0xfffffa801ad8b610      0x1ec0000       0x218efff       Vad     PAGE_READONLY    0       0       0xfa801b00d0b0  \Windows\Globalization\Sorting\SortDefault.nls  Disabled
3820    Rick And Morty  0xfffffa80194326b0      0x1de0000       0x1ebefff       Vad     PAGE_READONLY    0       0       0xfa801ad8b610  N/A     Disabled
3820    Rick And Morty  0xfffffa801b3b30a0      0x2190000       0x228ffff       VadS    PAGE_READWRITE   18      1       0xfa801ad8b610  N/A     Disabled
3820    Rick And Morty  0xfffffa801a7bc240      0x75210000      0x7524efff      Vad     PAGE_EXECUTE_WRITECOPY   3       0       0xfa801a7b7010  \Windows\System32\wow64.dll     Disabled
3820    Rick And Morty  0xfffffa801a7aff80      0x6c2d0000      0x6c2e1fff      Vad     PAGE_EXECUTE_WRITECOPY   2       0       0xfa801a7bc240  \Windows\SysWOW64\mpr.dll       Disabled
3820    Rick And Morty  0xfffffa801a7f6700      0x30f0000       0x312ffff       VadS    PAGE_READWRITE   7       1       0xfa801a7aff80  N/A     Disabled
3820    Rick And Morty  0xfffffa801a79b950      0x2e80000       0x2f7ffff       VadS    PAGE_READWRITE   3       1       0xfa801a7f6700  N/A     Disabled
3820    Rick And Morty  0xfffffa801b1eeec0      0x2c40000       0x2d3ffff       VadS    PAGE_READWRITE   23      1       0xfa801a79b950  N/A     Disabled
3820    Rick And Morty  0xfffffa801a528b90      0x2310000       0x2c3ffff       Vad     PAGE_READONLY    0       0       0xfa801b1eeec0  \Windows\Fonts\StaticCache.dat  Disabled
3820    Rick And Morty  0xfffffa801a56ae00      0x2e40000       0x2e7ffff       VadS    PAGE_READWRITE   7       1       0xfa801b1eeec0  N/A     Disabled
3820    Rick And Morty  0xfffffa801aadd6b0      0x2fb0000       0x2feffff       VadS    PAGE_READWRITE   7       1       0xfa801a79b950  N/A     Disabled
3820    Rick And Morty  0xfffffa801a52d2a0      0x2f90000       0x2f90fff       Vad     PAGE_READWRITE   0       0       0xfa801aadd6b0  N/A     Disabled
3820    Rick And Morty  0xfffffa801aa3e280      0x2f80000       0x2f87fff       Vad     PAGE_WRITECOPY   8       0       0xfa801a52d2a0  \Windows\SysWOW64\en-US\urlmon.dll.mui  Disabled
3820    Rick And Morty  0xfffffa801a545630      0x2fa0000       0x2facfff       Vad     PAGE_WRITECOPY   13      0       0xfa801a52d2a0  \Windows\SysWOW64\en-US\setupapi.dll.mui        Disabled
3820    Rick And Morty  0xfffffa801b0cd270      0x2ff0000       0x30effff       VadS    PAGE_READWRITE   3       1       0xfa801aadd6b0  N/A     Disabled
3820    Rick And Morty  0xfffffa801b1e8d70      0x68770000      0x687e5fff      Vadm    PAGE_EXECUTE_WRITECOPY   2       0       0xfa801a7f6700  \Windows\SysWOW64\riched20.dll  Disabled
3820    Rick And Morty  0xfffffa801aad6f40      0x3130000       0x322ffff       VadS    PAGE_READWRITE   3       1       0xfa801b1e8d70  N/A     Disabled
3820    Rick And Morty  0xfffffa801aa3b470      0x68870000      0x688c7fff      Vad     PAGE_EXECUTE_WRITECOPY   3       0       0xfa801b1e8d70  \Program Files (x86)\Common Files\microsoft shared\ink\tiptsf.dll        Disabled
3820    Rick And Morty  0xfffffa801b227810      0x68950000      0x6897dfff      Vad     PAGE_EXECUTE_WRITECOPY   2       0       0xfa801aa3b470  \Windows\SysWOW64\shdocvw.dll   Disabled
3820    Rick And Morty  0xfffffa801a089260      0x73da0000      0x73da5fff      Vad     PAGE_EXECUTE_WRITECOPY   2       0       0xfa801a7aff80  \Windows\SysWOW64\riched32.dll  Disabled
3820    Rick And Morty  0xfffffa801afcd760      0x72ce0000      0x72d2bfff      Vad     PAGE_EXECUTE_WRITECOPY   4       0       0xfa801a089260  \Windows\SysWOW64\apphelp.dll   Disabled
3820    Rick And Morty  0xfffffa8019442120      0x6c350000      0x6c3dcfff      Vad     PAGE_EXECUTE_WRITECOPY   11      0       0xfa801afcd760  \Windows\AppPatch\AcLayers.dll  Disabled
3820    Rick And Morty  0xfffffa801a7b5b40      0x6c2f0000      0x6c340fff      Vad     PAGE_EXECUTE_WRITECOPY   2       0       0xfa8019442120  \Windows\SysWOW64\winspool.drv  Disabled
3820    Rick And Morty  0xfffffa801a56e9c0      0x72080000      0x72174fff      Vad     PAGE_EXECUTE_WRITECOPY   3       0       0xfa8019442120  \Windows\SysWOW64\propsys.dll   Disabled
3820    Rick And Morty  0xfffffa80194ba830      0x73c90000      0x73cb0fff      Vad     PAGE_EXECUTE_WRITECOPY   3       0       0xfa801afcd760  \Windows\SysWOW64\ntmarta.dll   Disabled
3820    Rick And Morty  0xfffffa801a627c40      0x73c70000      0x73c82fff      Vad     PAGE_EXECUTE_WRITECOPY   3       0       0xfa80194ba830  \Windows\SysWOW64\dwmapi.dll    Disabled
3820    Rick And Morty  0xfffffa801a58e9e0      0x73ce0000      0x73cf6fff      Vad     PAGE_EXECUTE_WRITECOPY   2       0       0xfa80194ba830  \Windows\SysWOW64\userenv.dll   Disabled
3820    Rick And Morty  0xfffffa801a5ca480      0x75000000      0x7519dfff      Vad     PAGE_EXECUTE_WRITECOPY   4       0       0xfa801a089260  \Windows\winsxs\x86_microsoft.windows.common-controls_6595b64144ccf1df_6.0.7601.17514_none_41e6975e2bd6f2b2\comctl32.dll Disabled
3820    Rick And Morty  0xfffffa801a7fb920      0x741a0000      0x741aafff      Vad     PAGE_EXECUTE_WRITECOPY   2       0       0xfa801a5ca480  \Windows\SysWOW64\profapi.dll   Disabled
3820    Rick And Morty  0xfffffa801a5b1890      0x74120000      0x7419ffff      Vad     PAGE_EXECUTE_WRITECOPY   3       0       0xfa801a7fb920  \Windows\SysWOW64\uxtheme.dll   Disabled
3820    Rick And Morty  0xfffffa801a56e930      0x74820000      0x74828fff      Vad     PAGE_EXECUTE_WRITECOPY   2       0       0xfa801a7fb920  \Windows\SysWOW64\version.dll   Disabled
3820    Rick And Morty  0xfffffa801b1f6260      0x751a0000      0x751a7fff      Vad     PAGE_EXECUTE_WRITECOPY   2       0       0xfa801a5ca480  \Windows\System32\wow64cpu.dll  Disabled
3820    Rick And Morty  0xfffffa801b483280      0x751b0000      0x7520bfff      Vad     PAGE_EXECUTE_WRITECOPY   6       0       0xfa801b1f6260  \Windows\System32\wow64win.dll  Disabled
3820    Rick And Morty  0xfffffa801a6b7960      0x76160000      0x7620bfff      Vad     PAGE_EXECUTE_WRITECOPY   8       0       0xfa801a7bc240  \Windows\SysWOW64\msvcrt.dll    Disabled
3820    Rick And Morty  0xfffffa801ab0b490      0x75ad0000      0x75b6cfff      Vad     PAGE_EXECUTE_WRITECOPY   3       0       0xfa801a6b7960  \Windows\SysWOW64\usp10.dll     Disabled
3820    Rick And Morty  0xfffffa801a646330      0x756c0000      0x7574efff      Vad     PAGE_EXECUTE_WRITECOPY   3       0       0xfa801ab0b490  \Windows\SysWOW64\oleaut32.dll  Disabled
3820    Rick And Morty  0xfffffa801b0cd9e0      0x754b0000      0x7559ffff      Vad     PAGE_EXECUTE_WRITECOPY   2       0       0xfa801a646330  \Windows\SysWOW64\rpcrt4.dll    Disabled
3820    Rick And Morty  0xfffffa801a528710      0x75430000      0x7548ffff      Vad     PAGE_EXECUTE_WRITECOPY   2       0       0xfa801b0cd9e0  \Windows\SysWOW64\sspicli.dll   Disabled
3820    Rick And Morty  0xfffffa801a53df80      0x75420000      0x7542bfff      Vad     PAGE_EXECUTE_WRITECOPY   2       0       0xfa801a528710  \Windows\SysWOW64\cryptbase.dll Disabled
3820    Rick And Morty  0xfffffa801b490e30      0x75490000      0x754a1fff      Vad     PAGE_EXECUTE_WRITECOPY   2       0       0xfa801a528710  \Windows\SysWOW64\devobj.dll    Disabled
3820    Rick And Morty  0xfffffa801a56c0f0      0x755e0000      0x7567ffff      Vad     PAGE_EXECUTE_WRITECOPY   5       0       0xfa801b0cd9e0  \Windows\SysWOW64\advapi32.dll  Disabled
3820    Rick And Morty  0xfffffa801a7f9f80      0x75680000      0x756a6fff      Vad     PAGE_EXECUTE_WRITECOPY   2       0       0xfa801a56c0f0  \Windows\SysWOW64\cfgmgr32.dll  Disabled
3820    Rick And Morty  0xfffffa801b5952d0      0x757d0000      0x757d9fff      Vad     PAGE_EXECUTE_WRITECOPY   2       0       0xfa801a646330  \Windows\SysWOW64\lpk.dll       Disabled
3820    Rick And Morty  0xfffffa801a52a0e0      0x75750000      0x75794fff      Vad     PAGE_EXECUTE_WRITECOPY   2       0       0xfa801b5952d0  \Windows\SysWOW64\Wldap32.dll   Disabled
3820    Rick And Morty  0xfffffa801a5283b0      0x757e0000      0x758d4fff      Vad     PAGE_EXECUTE_WRITECOPY   8       0       0xfa801b5952d0  \Windows\SysWOW64\wininet.dll   Disabled
3820    Rick And Morty  0xfffffa801986ad60      0x759b0000      0x75accfff      Vad     PAGE_EXECUTE_WRITECOPY   3       0       0xfa801a5283b0  \Windows\SysWOW64\crypt32.dll   Disabled
3820    Rick And Morty  0xfffffa801b47da20      0x75d30000      0x75d75fff      Vad     PAGE_EXECUTE_WRITECOPY   3       0       0xfa801ab0b490  \Windows\SysWOW64\KernelBase.dll        Disabled
3820    Rick And Morty  0xfffffa801b64f890      0x75b70000      0x75beafff      Vad     PAGE_EXECUTE_WRITECOPY   5       0       0xfa801b47da20  \Windows\SysWOW64\comdlg32.dll  Disabled
3820    Rick And Morty  0xfffffa801a585be0      0x75bf0000      0x75d25fff      Vad     PAGE_EXECUTE_WRITECOPY   12      0       0xfa801b64f890  \Windows\SysWOW64\urlmon.dll    Disabled
3820    Rick And Morty  0xfffffa801aac2250      0x75de0000      0x75df8fff      Vad     PAGE_EXECUTE_WRITECOPY   4       0       0xfa801b47da20  \Windows\SysWOW64\sechost.dll   Disabled
3820    Rick And Morty  0xfffffa801a54f010      0x75d80000      0x75ddffff      Vad     PAGE_EXECUTE_WRITECOPY   2       0       0xfa801aac2250  \Windows\SysWOW64\imm32.dll     Disabled
3820    Rick And Morty  0xfffffa801a561210      0x76000000      0x7615bfff      Vad     PAGE_EXECUTE_WRITECOPY   5       0       0xfa801aac2250  \Windows\SysWOW64\ole32.dll     Disabled
3820    Rick And Morty  0xfffffa801a55cb50      0x75e00000      0x75ffafff      Vad     PAGE_EXECUTE_WRITECOPY   6       0       0xfa801a561210  \Windows\SysWOW64\iertutil.dll  Disabled
3820    Rick And Morty  0xfffffa801a7d4970      0x7efb0000      0x7efd2fff      Vad     PAGE_READONLY    0       0       0xfa801a6b7960  N/A     Disabled
3820    Rick And Morty  0xfffffa801b000010      0x772f0000      0x773fffff      Vad     PAGE_EXECUTE_WRITECOPY   3       0       0xfa801a7d4970  \Windows\SysWOW64\kernel32.dll  Disabled
3820    Rick And Morty  0xfffffa801a40d4d0      0x76f00000      0x76ffffff      Vadm    PAGE_EXECUTE_WRITECOPY   2       0       0xfa801b000010  \Windows\SysWOW64\user32.dll    Disabled
3820    Rick And Morty  0xfffffa801a569f80      0x76e70000      0x76efffff      Vad     PAGE_EXECUTE_WRITECOPY   2       0       0xfa801a40d4d0  \Windows\SysWOW64\gdi32.dll     Disabled
3820    Rick And Morty  0xfffffa801a71e750      0x76220000      0x76e69fff      Vad     PAGE_EXECUTE_WRITECOPY   9       0       0xfa801a569f80  \Windows\SysWOW64\shell32.dll   Disabled
3820    Rick And Morty  0xfffffa801afe6660      0x77200000      0x77256fff      Vad     PAGE_EXECUTE_WRITECOPY   2       0       0xfa801a40d4d0  \Windows\SysWOW64\shlwapi.dll   Disabled
3820    Rick And Morty  0xfffffa801a54d6a0      0x77060000      0x771fcfff      Vad     PAGE_EXECUTE_WRITECOPY   6       0       0xfa801afe6660  \Windows\SysWOW64\setupapi.dll  Disabled
3820    Rick And Morty  0xfffffa801ab3dbf0      0x77260000      0x772e2fff      Vad     PAGE_EXECUTE_WRITECOPY   5       0       0xfa801afe6660  \Windows\SysWOW64\clbcatq.dll   Disabled
3820    Rick And Morty  0xfffffa801b0b5ce0      0x776f0000      0x77898fff      Vad     PAGE_EXECUTE_WRITECOPY   12      0       0xfa801b000010  \Windows\System32\ntdll.dll     Disabled
3820    Rick And Morty  0xfffffa801a7b9870      0x774d0000      0x775c9fff      VadS    PAGE_EXECUTE_READWRITE   0       1       0xfa801b0b5ce0  N/A     Disabled
3820    Rick And Morty  0xfffffa801a57b940      0x77400000      0x774cbfff      Vad     PAGE_EXECUTE_WRITECOPY   3       0       0xfa801a7b9870  \Windows\SysWOW64\msctf.dll     Disabled
3820    Rick And Morty  0xfffffa801a547330      0x775d0000      0x776eefff      VadS    PAGE_EXECUTE_READWRITE   0       1       0xfa801a7b9870  N/A     Disabled
3820    Rick And Morty  0xfffffa801a50b470      0x778d0000      0x77a4ffff      Vad     PAGE_EXECUTE_WRITECOPY   9       0       0xfa801b0b5ce0  \Windows\SysWOW64\ntdll.dll     Disabled
3820    Rick And Morty  0xfffffa801a7d9200      0x778a0000      0x778abfff      Vad     PAGE_EXECUTE_WRITECOPY   2       0       0xfa801a50b470  \Windows\SysWOW64\msasn1.dll    Disabled
3820    Rick And Morty  0xfffffa801b485ee0      0x7efad000      0x7efaffff      Vadl    PAGE_READWRITE   3       1       0xfa801a50b470  N/A     Disabled
3820    Rick And Morty  0xfffffa801a7a5f70      0x7efaa000      0x7efacfff      Vadl    PAGE_READWRITE   3       1       0xfa801b485ee0  N/A     Disabled
3820    Rick And Morty  0xfffffa801aac5e00      0x7f0e0000      0x7ffdffff      VadS    PAGE_READONLY    0       1       0xfa801a7d4970  N/A     Disabled
3820    Rick And Morty  0xfffffa801a772910      0x7efde000      0x7efdefff      Vadl    PAGE_READWRITE   1       1       0xfa801aac5e00  N/A     Disabled
3820    Rick And Morty  0xfffffa801b5c3c00      0x7efdb000      0x7efddfff      Vadl    PAGE_READWRITE   3       1       0xfa801a772910  N/A     Disabled
3820    Rick And Morty  0xfffffa801b1e8a80      0x7efd5000      0x7efd7fff      Vadl    PAGE_READWRITE   3       1       0xfa801b5c3c00  N/A     Disabled
3820    Rick And Morty  0xfffffa801b0e2510      0x7efdf000      0x7efdffff      Vadl    PAGE_READWRITE   1       1       0xfa801a772910  \Windows\System32\user32.dll    Disabled
3820    Rick And Morty  0xfffffa801a7cae20      0x7efe0000      0x7f0dffff      Vad     PAGE_READONLY    0       0       0xfa801b0e2510  N/A     Disabled
3820    Rick And Morty  0xfffffa801b1e8940      0x7ffe0000      0x7ffeffff      Vadl    PAGE_READONLY    2251799813685247        1       0xfa801aac5e00  N/A     Disabled
3820    Rick And Morty  0xfffffa801b1e89e0      0x7fff0000      0x7fffffeffff   Vadl    PAGE_READONLY    2251799813685247        1       0xfa801b1e8940  N/A     Disabled
```


# 測試內容
- vol.exe -f .\OtterCTF.vmem windows.vadinfo.VadInfo --pid 3720


```
D:\Forensic\G140A006\VolatilityWorkbench>.\vol.exe -f .\OtterCTF.vmem windows.vadinfo.VadInfo --pid 3720
Volatility 3 Framework 2.5.0
Progress:  100.00               PDB scanning finished
PID     Process Offset  Start VPN       End VPN Tag     Protection      CommitCharge    PrivateMemory    Parent  File    File output

3720    vmware-tray.ex  0xfffffa801aaaab00      0xec0000        0xf2dfff        Vad     PAGE_EXECUTE_WRITECOPY   2       0       0xfa801a4c5f78  \Users\Rick\AppData\Local\Temp\RarSFX0\vmware-tray.exe   Disabled
3720    vmware-tray.ex  0xfffffa801afec060      0x330000        0x3affff        VadS    PAGE_READWRITE   6       1       0xfa801aaaab00  N/A     Disabled
3720    vmware-tray.ex  0xfffffa801ac9c8a0      0x110000        0x14ffff        VadS    PAGE_READWRITE   9       1       0xfa801afec060  N/A     Disabled
3720    vmware-tray.ex  0xfffffa801b4f2bd0      0x60000 0x60fff Vad     PAGE_READONLY   0       00xfa801ac9c8a0  N/A     Disabled
3720    vmware-tray.ex  0xfffffa801afe6770      0x40000 0x40fff Vad     PAGE_EXECUTE_WRITECOPY  00       0xfa801b4f2bd0  \Windows\System32\apisetschema.dll      Disabled
3720    vmware-tray.ex  0xfffffa801ad15c00      0x20000 0x20fff Vadm    PAGE_READWRITE  1       10xfa801afe6770  N/A     Disabled
3720    vmware-tray.ex  0xfffffa801a5c43e0      0x10000 0x1ffff Vad     PAGE_READWRITE  0       00xfa801ad15c00  N/A     Disabled
3720    vmware-tray.ex  0xfffffa801b536bb0      0x30000 0x30fff Vadm    PAGE_READWRITE  1       10xfa801ad15c00  N/A     Disabled
3720    vmware-tray.ex  0xfffffa801aa635e0      0x50000 0x53fff Vad     PAGE_READONLY   0       00xfa801afe6770  N/A     Disabled
3720    vmware-tray.ex  0xfffffa801a591530      0x80000 0xe6fff Vad     PAGE_READONLY   0       00xfa801b4f2bd0  \Windows\System32\locale.nls    Disabled
3720    vmware-tray.ex  0xfffffa801a7b94c0      0x70000 0x70fff VadS    PAGE_READWRITE  1       10xfa801a591530  N/A     Disabled
3720    vmware-tray.ex  0xfffffa801a6cf9a0      0xf0000 0xf0fff Vad     PAGE_READWRITE  0       00xfa801a591530  N/A     Disabled
3720    vmware-tray.ex  0xfffffa801a597110      0x100000        0x10ffff        Vad     PAGE_READWRITE   0       0       0xfa801a6cf9a0  N/A     Disabled
3720    vmware-tray.ex  0xfffffa801a46c1f0      0x1b0000        0x1b0fff        VadS    PAGE_READWRITE   1       1       0xfa801ac9c8a0  N/A     Disabled
3720    vmware-tray.ex  0xfffffa801a4dc180      0x170000        0x17ffff        VadS    PAGE_NOACCESS    11      1       0xfa801a46c1f0  N/A     Disabled
3720    vmware-tray.ex  0xfffffa801ac660f0      0x160000        0x16ffff        VadS    PAGE_NOACCESS    3       1       0xfa801a4dc180  N/A     Disabled
3720    vmware-tray.ex  0xfffffa801b0c4430      0x150000        0x15ffff        VadS    PAGE_NOACCESS    2       1       0xfa801ac660f0  N/A     Disabled
3720    vmware-tray.ex  0xfffffa801b0e92a0      0x190000        0x19ffff        VadS    PAGE_READWRITE   4       1       0xfa801a4dc180  N/A     Disabled
3720    vmware-tray.ex  0xfffffa801aaab340      0x180000        0x18ffff        VadS    PAGE_NOACCESS    5       1       0xfa801b0e92a0  N/A     Disabled
3720    vmware-tray.ex  0xfffffa801a42a240      0x1a0000        0x1affff        VadS    PAGE_NOACCESS    5       1       0xfa801b0e92a0  N/A     Disabled
3720    vmware-tray.ex  0xfffffa801b2fa4b0      0x1f0000        0x2effff        Vadm    PAGE_READWRITE   255     1       0xfa801a46c1f0  N/A     Disabled
3720    vmware-tray.ex  0xfffffa801a7d5510      0x1d0000        0x1dffff        VadS    PAGE_READWRITE   16      1       0xfa801b2fa4b0  N/A     Disabled
3720    vmware-tray.ex  0xfffffa801a46c3a0      0x1c0000        0x1c0fff        VadS    PAGE_READWRITE   1       1       0xfa801a7d5510  N/A     Disabled
3720    vmware-tray.ex  0xfffffa801a57db80      0x1e0000        0x1effff        VadS    PAGE_NOACCESS    3       1       0xfa801a7d5510  N/A     Disabled
3720    vmware-tray.ex  0xfffffa801aabb9d0      0x300000        0x301fff        Vad     PAGE_READONLY    0       0       0xfa801b2fa4b0  N/A     Disabled
3720    vmware-tray.ex  0xfffffa801afe1070      0x2f0000        0x2fffff        VadS    PAGE_NOACCESS    4       1       0xfa801aabb9d0  N/A     Disabled
3720    vmware-tray.ex  0xfffffa801af7deb0      0x320000        0x321fff        Vad     PAGE_READONLY    0       0       0xfa801aabb9d0  N/A     Disabled
3720    vmware-tray.ex  0xfffffa801af75240      0x310000        0x31ffff        VadS    PAGE_READWRITE   16      1       0xfa801af7deb0  N/A     Disabled
3720    vmware-tray.ex  0xfffffa801ad6a0f0      0x670000        0x6affff        VadS    PAGE_EXECUTE_READWRITE   1       1       0xfa801afec060  N/A     Disabled
3720    vmware-tray.ex  0xfffffa801a4baef0      0x510000        0x54ffff        VadS    PAGE_EXECUTE_READWRITE   23      1       0xfa801ad6a0f0  N/A     Disabled
3720    vmware-tray.ex  0xfffffa801b5a00f0      0x3f0000        0x4effff        Vadm    PAGE_READWRITE   251     1       0xfa801a4baef0  N/A     Disabled
3720    vmware-tray.ex  0xfffffa801a785280      0x3d0000        0x3dffff        VadS    PAGE_READWRITE   3       1       0xfa801b5a00f0  N/A     Disabled
3720    vmware-tray.ex  0xfffffa801b3a9c20      0x3b0000        0x3cffff        VadS    PAGE_READWRITE   1       1       0xfa801a785280  N/A     Disabled
3720    vmware-tray.ex  0xfffffa801ace0680      0x3e0000        0x3e0fff        Vadm    PAGE_READWRITE   1       1       0xfa801a785280  N/A     Disabled
3720    vmware-tray.ex  0xfffffa801aa06f80      0x4f0000        0x4f0fff        Vad     PAGE_READWRITE   0       0       0xfa801b5a00f0  N/A     Disabled
3720    vmware-tray.ex  0xfffffa801a53d650      0x500000        0x500fff        Vadm    PAGE_READWRITE   1       1       0xfa801aa06f80  N/A     Disabled
3720    vmware-tray.ex  0xfffffa801a42a090      0x590000        0x59ffff        VadS    PAGE_READWRITE   4       1       0xfa801a4baef0  N/A     Disabled
3720    vmware-tray.ex  0xfffffa801af3d200      0x550000        0x56dfff        Vadm    PAGE_READWRITE   30      1       0xfa801a42a090  N/A     Disabled
3720    vmware-tray.ex  0xfffffa801a5e6340      0x5d0000        0x5dffff        VadS    PAGE_READWRITE   4       1       0xfa801a42a090  N/A     Disabled
3720    vmware-tray.ex  0xfffffa801a73d920      0x600000        0x63ffff        VadS    PAGE_READWRITE   7       1       0xfa801a5e6340  N/A     Disabled
3720    vmware-tray.ex  0xfffffa801a4b5ae0      0xc00000        0xc3ffff        VadS    PAGE_EXECUTE_READWRITE   1       1       0xfa801ad6a0f0  N/A     Disabled
3720    vmware-tray.ex  0xfffffa801b0533e0      0xa10000        0xa4ffff        VadS    PAGE_EXECUTE_READWRITE   1       1       0xfa801a4b5ae0  N/A     Disabled
3720    vmware-tray.ex  0xfffffa801b1f2fc0      0x840000        0x84ffff        VadS    PAGE_READWRITE   4       1       0xfa801b0533e0  N/A     Disabled
3720    vmware-tray.ex  0xfffffa801b52b8a0      0x6b0000        0x837fff        Vad     PAGE_READONLY    0       0       0xfa801b1f2fc0  N/A     Disabled
3720    vmware-tray.ex  0xfffffa8018e01010      0x850000        0x9d0fff        Vadm    PAGE_READONLY    0       0       0xfa801b1f2fc0  N/A     Disabled
3720    vmware-tray.ex  0xfffffa801adaf990      0xb10000        0xb4ffff        VadS    PAGE_READWRITE   26      1       0xfa801b0533e0  N/A     Disabled
3720    vmware-tray.ex  0xfffffa801b30ac00      0xa50000        0xaeffff        VadS    PAGE_READWRITE   160     1       0xfa801adaf990  N/A     Disabled
3720    vmware-tray.ex  0xfffffa801aad6be0      0xb70000        0xbaffff        VadS    PAGE_READWRITE   7       1       0xfa801adaf990  N/A     Disabled
3720    vmware-tray.ex  0xfffffa801a416df0      0xe10000        0xe4ffff        VadS    PAGE_READWRITE   7       1       0xfa801a4b5ae0  N/A     Disabled
3720    vmware-tray.ex  0xfffffa801a4b5d50      0xc90000        0xd8ffff        VadS    PAGE_READWRITE   255     1       0xfa801a416df0  N/A     Disabled
3720    vmware-tray.ex  0xfffffa801b4636d0      0xc50000        0xc8ffff        VadS    PAGE_READWRITE   7       1       0xfa801a4b5d50  N/A     Disabled
3720    vmware-tray.ex  0xfffffa801a56ff80      0xd90000        0xdeafff        Vad     PAGE_READONLY    0       0       0xfa801a4b5d50  \Windows\Microsoft.NET\Framework\v4.0.30319\mscorrc.dll Disabled
3720    vmware-tray.ex  0xfffffa801919e8d0      0xe60000        0xe9ffff        VadS    PAGE_READWRITE   7       1       0xfa801a416df0  N/A     Disabled
3720    vmware-tray.ex  0xfffffa801a6afee0      0x74a00000      0x74a65fff      Vad     PAGE_EXECUTE_WRITECOPY   5       0       0xfa801aaaab00  \Windows\Microsoft.NET\Framework\v4.0.30319\mscoreei.dll Disabled
3720    vmware-tray.ex  0xfffffa801a46a260      0x66660000      0x667f5fff      Vad     PAGE_EXECUTE_WRITECOPY   61      0       0xfa801a6afee0  \Windows\assembly\NativeImages_v4.0.30319_32\System.Drawing\dd57bc19f5807c6dbe8f88d4a23277f6\System.Drawing.ni.dll       Disabled
3720    vmware-tray.ex  0xfffffa801a6b8670      0x4f20000       0x4f95fff       VadS    PAGE_READWRITE   118     1       0xfa801a46a260  N/A     Disabled
3720    vmware-tray.ex  0xfffffa801b0b5120      0x4960000       0x4a5ffff       VadS    PAGE_READWRITE   3       1       0xfa801a6b8670  N/A     Disabled
3720    vmware-tray.ex  0xfffffa801a416f00      0x4480000       0x457ffff       VadS    PAGE_READWRITE   255     1       0xfa801b0b5120  N/A     Disabled
3720    vmware-tray.ex  0xfffffa801a73aae0      0x2330000       0x432ffff       Vadm    PAGE_READWRITE   515     1       0xfa801a416f00  N/A     Disabled
3720    vmware-tray.ex  0xfffffa801b558510      0xf30000        0x232ffff       Vad     PAGE_READONLY    0       0       0xfa801a73aae0  N/A     Disabled
3720    vmware-tray.ex  0xfffffa801b1f7200      0x4330000       0x440efff       Vad     PAGE_READONLY    0       0       0xfa801a73aae0  N/A     Disabled
3720    vmware-tray.ex  0xfffffa801b3dfa00      0x4410000       0x444ffff       VadS    PAGE_READWRITE   7       1       0xfa801b1f7200  N/A     Disabled
3720    vmware-tray.ex  0xfffffa801a406010      0x4580000       0x484efff       Vad     PAGE_READONLY    0       0       0xfa801a416f00  \Windows\Globalization\Sorting\SortDefault.nls  Disabled
3720    vmware-tray.ex  0xfffffa801a7dc210      0x4850000       0x494ffff       VadS    PAGE_READWRITE   248     1       0xfa801a406010  N/A     Disabled
3720    vmware-tray.ex  0xfffffa801a627630      0x4e90000       0x4e9ffff       VadS    PAGE_READWRITE   16      1       0xfa801b0b5120  N/A     Disabled
3720    vmware-tray.ex  0xfffffa801a56aa20      0x4a60000       0x4d31fff       Vad     PAGE_READONLY    0       0       0xfa801a627630  \Windows\Microsoft.NET\Framework\v4.0.30319\sortdefault.nlp      Disabled
3720    vmware-tray.ex  0xfffffa801ad8dca0      0x4d70000       0x4e6ffff       VadS    PAGE_READWRITE   3       1       0xfa801a56aa20  N/A     Disabled
3720    vmware-tray.ex  0xfffffa801ab4f830      0x4ea0000       0x4f1ffff       VadS    PAGE_READWRITE   1       1       0xfa801a627630  N/A     Disabled
3720    vmware-tray.ex  0xfffffa801b5cb4b0      0x54d0000       0x5dfffff       Vad     PAGE_READONLY    0       0       0xfa801a6b8670  \Windows\Fonts\StaticCache.dat  Disabled
3720    vmware-tray.ex  0xfffffa801a6c58a0      0x50e0000       0x511ffff       VadS    PAGE_READWRITE   28      1       0xfa801b5cb4b0  N/A     Disabled
3720    vmware-tray.ex  0xfffffa801a5863c0      0x4fa0000       0x509ffff       VadS    PAGE_READWRITE   10      1       0xfa801a6c58a0  N/A     Disabled
3720    vmware-tray.ex  0xfffffa801b1aa380      0x52d0000       0x54cffff       VadS    PAGE_READWRITE   85      1       0xfa801a6c58a0  N/A     Disabled
3720    vmware-tray.ex  0xfffffa801aa64fc0      0x5240000       0x527ffff       VadS    PAGE_READWRITE   7       1       0xfa801b1aa380  N/A     Disabled
3720    vmware-tray.ex  0xfffffa801aa64f70      0x7bd0000       0x7ccffff       VadS    PAGE_READWRITE   3       1       0xfa801b5cb4b0  N/A     Disabled
3720    vmware-tray.ex  0xfffffa801b438bd0      0x7970000       0x7a6ffff       VadS    PAGE_READWRITE   3       1       0xfa801aa64f70  N/A     Disabled
3720    vmware-tray.ex  0xfffffa801a656590      0x5e00000       0x789ffff       VadS    PAGE_READWRITE   6816    1       0xfa801b438bd0  N/A     Disabled
3720    vmware-tray.ex  0xfffffa801a6351a0      0x7a80000       0x7b7ffff       VadS    PAGE_READWRITE   3       1       0xfa801b438bd0  N/A     Disabled
3720    vmware-tray.ex  0xfffffa801aea1ae0      0x65330000      0x659e5fff      Vad     PAGE_EXECUTE_WRITECOPY   416     0       0xfa801aa64f70  \Windows\assembly\NativeImages_v4.0.30319_32\System.Core\713647b987b140a17e3c4ffe4c721f85\System.Core.ni.dll     Disabled
3720    vmware-tray.ex  0xfffffa801a585430      0x659f0000      0x6665afff      Vad     PAGE_EXECUTE_WRITECOPY   432     0       0xfa801aea1ae0  \Windows\assembly\NativeImages_v4.0.30319_32\System.Windows.Forms\17e020ae92d7fab33bcc1c98b25019d0\System.Windows.Forms.ni.dll   Disabled
3720    vmware-tray.ex  0xfffffa801a2f5240      0x69720000      0x697ddfff      Vad     PAGE_EXECUTE_WRITECOPY   7       0       0xfa801a46a260  \Windows\SysWOW64\msvcr100_clr0400.dll  Disabled
3720    vmware-tray.ex  0xfffffa801b19e380      0x68070000      0x686defff      Vad     PAGE_EXECUTE_WRITECOPY   66      0       0xfa801a2f5240  \Windows\Microsoft.NET\Framework\v4.0.30319\clr.dll      Disabled
3720    vmware-tray.ex  0xfffffa801a528c20      0x670a0000      0x67e62fff      Vad     PAGE_EXECUTE_WRITECOPY   524     0       0xfa801b19e380  \Windows\assembly\NativeImages_v4.0.30319_32\mscorlib\246f1a5abb686b9dcdf22d3505b08cea\mscorlib.ni.dll   Disabled
3720    vmware-tray.ex  0xfffffa801b19eb60      0x66800000      0x67097fff      Vad     PAGE_EXECUTE_WRITECOPY   304     0       0xfa801a528c20  \Windows\assembly\NativeImages_v4.0.30319_32\System\964da027ebca3b263a05cadb8eaa20a3\System.ni.dll       Disabled
3720    vmware-tray.ex  0xfffffa801a733390      0x68010000      0x6806ffff      Vad     PAGE_EXECUTE_WRITECOPY   2       0       0xfa801a528c20  \Windows\Microsoft.NET\Framework\v4.0.30319\clrjit.dll   Disabled
3720    vmware-tray.ex  0xfffffa801aaa4ef0      0x68860000      0x6886ffff      Vad     PAGE_EXECUTE_WRITECOPY   2       0       0xfa801b19e380  \Windows\Microsoft.NET\Framework\v4.0.30319\nlssorting.dll       Disabled
3720    vmware-tray.ex  0xfffffa801a0b5390      0x73fe0000      0x74063fff      Vad     PAGE_EXECUTE_WRITECOPY   4       0       0xfa801a2f5240  \Windows\winsxs\x86_microsoft.windows.common-controls_6595b64144ccf1df_5.82.7601.17514_none_ec83dffa859149af\comctl32.dll        Disabled
3720    vmware-tray.ex  0xfffffa801aefd4b0      0x73c70000      0x73c82fff      Vad     PAGE_EXECUTE_WRITECOPY   3       0       0xfa801a0b5390  \Windows\SysWOW64\dwmapi.dll    Disabled
3720    vmware-tray.ex  0xfffffa801b5886b0      0x71990000      0x71a8afff      Vad     PAGE_EXECUTE_WRITECOPY   5       0       0xfa801aefd4b0  \Windows\SysWOW64\WindowsCodecs.dll     Disabled
3720    vmware-tray.ex  0xfffffa801a627460      0x73f60000      0x73f76fff      Vad     PAGE_EXECUTE_WRITECOPY   2       0       0xfa801aefd4b0  \Windows\SysWOW64\bcrypt.dll    Disabled
3720    vmware-tray.ex  0xfffffa801ae3aac0      0x741a0000      0x741aafff      Vad     PAGE_EXECUTE_WRITECOPY   2       0       0xfa801a0b5390  \Windows\SysWOW64\profapi.dll   Disabled
3720    vmware-tray.ex  0xfffffa801b0ae0e0      0x74100000      0x74115fff      Vad     PAGE_EXECUTE_WRITECOPY   2       0       0xfa801ae3aac0  \Windows\SysWOW64\cryptsp.dll   Disabled
3720    vmware-tray.ex  0xfffffa801ad0fb00      0x740c0000      0x740fafff      Vad     PAGE_EXECUTE_WRITECOPY   4       0       0xfa801b0ae0e0  \Windows\SysWOW64\rsaenh.dll    Disabled
3720    vmware-tray.ex  0xfffffa801a561180      0x74120000      0x7419ffff      Vad     PAGE_EXECUTE_WRITECOPY   3       0       0xfa801b0ae0e0  \Windows\SysWOW64\uxtheme.dll   Disabled
3720    vmware-tray.ex  0xfffffa801ae95ce0      0x74870000      0x749fffff      Vad     PAGE_EXECUTE_WRITECOPY   10      0       0xfa801ae3aac0  \Windows\winsxs\x86_microsoft.windows.gdiplus_6595b64144ccf1df_1.1.7601.17514_none_72d18a4386696c80\GdiPlus.dll  Disabled
3720    vmware-tray.ex  0xfffffa801a6448b0      0x774d0000      0x775c9fff      VadS    PAGE_EXECUTE_READWRITE   0       1       0xfa801a6afee0  N/A     Disabled
3720    vmware-tray.ex  0xfffffa801a7df6f0      0x754b0000      0x7559ffff      Vad     PAGE_EXECUTE_WRITECOPY   2       0       0xfa801a6448b0  \Windows\SysWOW64\rpcrt4.dll    Disabled
3720    vmware-tray.ex  0xfffffa801b050840      0x75210000      0x7524efff      Vad     PAGE_EXECUTE_WRITECOPY   3       0       0xfa801a7df6f0  \Windows\System32\wow64.dll     Disabled
3720    vmware-tray.ex  0xfffffa801b485c60      0x751a0000      0x751a7fff      Vad     PAGE_EXECUTE_WRITECOPY   2       0       0xfa801b050840  \Windows\System32\wow64cpu.dll  Disabled
3720    vmware-tray.ex  0xfffffa801ae4aca0      0x74f60000      0x74fa9fff      Vad     PAGE_EXECUTE_WRITECOPY   5       0       0xfa801b485c60  \Windows\SysWOW64\mscoree.dll   Disabled
3720    vmware-tray.ex  0xfffffa801b48c100      0x75000000      0x7519dfff      Vad     PAGE_EXECUTE_WRITECOPY   4       0       0xfa801ae4aca0  \Windows\winsxs\x86_microsoft.windows.common-controls_6595b64144ccf1df_6.0.7601.17514_none_41e6975e2bd6f2b2\comctl32.dll Disabled
3720    vmware-tray.ex  0xfffffa801b4857b0      0x751b0000      0x7520bfff      Vad     PAGE_EXECUTE_WRITECOPY   6       0       0xfa801b485c60  \Windows\System32\wow64win.dll  Disabled
3720    vmware-tray.ex  0xfffffa801a520a00      0x75430000      0x7548ffff      Vad     PAGE_EXECUTE_WRITECOPY   2       0       0xfa801b050840  \Windows\SysWOW64\sspicli.dll   Disabled
3720    vmware-tray.ex  0xfffffa801ab21700      0x75420000      0x7542bfff      Vad     PAGE_EXECUTE_WRITECOPY   2       0       0xfa801a520a00  \Windows\SysWOW64\cryptbase.dll Disabled
3720    vmware-tray.ex  0xfffffa801a79b8c0      0x76160000      0x7620bfff      Vad     PAGE_EXECUTE_WRITECOPY   8       0       0xfa801a7df6f0  \Windows\SysWOW64\msvcrt.dll    Disabled
3720    vmware-tray.ex  0xfffffa801a7fba60      0x75d30000      0x75d75fff      Vad     PAGE_EXECUTE_WRITECOPY   3       0       0xfa801a79b8c0  \Windows\SysWOW64\KernelBase.dll        Disabled
3720    vmware-tray.ex  0xfffffa801b19b4b0      0x757d0000      0x757d9fff      Vad     PAGE_EXECUTE_WRITECOPY   2       0       0xfa801a7fba60  \Windows\SysWOW64\lpk.dll       Disabled
3720    vmware-tray.ex  0xfffffa801b439370      0x755e0000      0x7567ffff      Vad     PAGE_EXECUTE_WRITECOPY   5       0       0xfa801b19b4b0  \Windows\SysWOW64\advapi32.dll  Disabled
3720    vmware-tray.ex  0xfffffa801b42e280      0x75ad0000      0x75b6cfff      Vad     PAGE_EXECUTE_WRITECOPY   3       0       0xfa801b19b4b0  \Windows\SysWOW64\usp10.dll     Disabled
3720    vmware-tray.ex  0xfffffa801ac9e150      0x75de0000      0x75df8fff      Vad     PAGE_EXECUTE_WRITECOPY   4       0       0xfa801a7fba60  \Windows\SysWOW64\sechost.dll   Disabled
3720    vmware-tray.ex  0xfffffa801af4a870      0x75d80000      0x75ddffff      Vad     PAGE_EXECUTE_WRITECOPY   2       0       0xfa801ac9e150  \Windows\SysWOW64\imm32.dll     Disabled
3720    vmware-tray.ex  0xfffffa8019fbbc90      0x76000000      0x7615bfff      Vad     PAGE_EXECUTE_WRITECOPY   5       0       0xfa801ac9e150  \Windows\SysWOW64\ole32.dll     Disabled
3720    vmware-tray.ex  0xfffffa801ad6bc60      0x77200000      0x77256fff      Vad     PAGE_EXECUTE_WRITECOPY   2       0       0xfa801a79b8c0  \Windows\SysWOW64\shlwapi.dll   Disabled
3720    vmware-tray.ex  0xfffffa801b502a00      0x76e70000      0x76efffff      Vad     PAGE_EXECUTE_WRITECOPY   2       0       0xfa801ad6bc60  \Windows\SysWOW64\gdi32.dll     Disabled
3720    vmware-tray.ex  0xfffffa801b1f5580      0x76220000      0x76e69fff      Vad     PAGE_EXECUTE_WRITECOPY   9       0       0xfa801b502a00  \Windows\SysWOW64\shell32.dll   Disabled
3720    vmware-tray.ex  0xfffffa801a614590      0x76f00000      0x76ffffff      Vadm    PAGE_EXECUTE_WRITECOPY   2       0       0xfa801b502a00  \Windows\SysWOW64\user32.dll    Disabled
3720    vmware-tray.ex  0xfffffa80195bf8a0      0x772f0000      0x773fffff      Vad     PAGE_EXECUTE_WRITECOPY   3       0       0xfa801ad6bc60  \Windows\SysWOW64\kernel32.dll  Disabled
3720    vmware-tray.ex  0xfffffa801b3d7a80      0x77400000      0x774cbfff      Vad     PAGE_EXECUTE_WRITECOPY   3       0       0xfa80195bf8a0  \Windows\SysWOW64\msctf.dll     Disabled
3720    vmware-tray.ex  0xfffffa801b5685b0      0x80000000      0x8000ffff      VadS    PAGE_NOACCESS    0       1       0xfa801a6448b0  N/A     Disabled
3720    vmware-tray.ex  0xfffffa801a7963b0      0x7f0e0000      0x7ffdffff      VadS    PAGE_READONLY    0       1       0xfa801b5685b0  N/A     Disabled
3720    vmware-tray.ex  0xfffffa801a0a5510      0x776f0000      0x77898fff      Vad     PAGE_EXECUTE_WRITECOPY   12      0       0xfa801a7963b0  \Windows\System32\ntdll.dll     Disabled
3720    vmware-tray.ex  0xfffffa801a7e7530      0x775d0000      0x776eefff      VadS    PAGE_EXECUTE_READWRITE   0       1       0xfa801a0a5510  N/A     Disabled
3720    vmware-tray.ex  0xfffffa80197aabf0      0x778d0000      0x77a4ffff      Vad     PAGE_EXECUTE_WRITECOPY   9       0       0xfa801a0a5510  \Windows\SysWOW64\ntdll.dll     Disabled
3720    vmware-tray.ex  0xfffffa801a5699a0      0x7efe0000      0x7f0dffff      Vad     PAGE_READONLY    0       0       0xfa80197aabf0  N/A     Disabled
3720    vmware-tray.ex  0xfffffa801b59d580      0x7fff0000      0x7fffffff      VadS    PAGE_NOACCESS    0       1       0xfa801a7963b0  N/A     Disabled
3720    vmware-tray.ex  0xfffffa801b0aa520      0x7ffe0000      0x7ffeffff      Vadl    PAGE_READONLY    2251799813685247        1       0xfa801b59d580  N/A     Disabled
3720    vmware-tray.ex  0xfffffa801a627bb0      0xfffb0000      0xfffd2fff      Vad     PAGE_READONLY    0       0       0xfa801b5685b0  N/A     Disabled
3720    vmware-tray.ex  0xfffffa801b3c10b0      0xfffaa000      0xfffacfff      Vadl    PAGE_READWRITE   3       1       0xfa801a627bb0  N/A     Disabled
3720    vmware-tray.ex  0xfffffa801a6726f0      0xfffa4000      0xfffa6fff      Vadl    PAGE_READWRITE   3       1       0xfa801b3c10b0  N/A     Disabled
3720    vmware-tray.ex  0xfffffa801a4f07c0      0xfffa1000      0xfffa3fff      Vadl    PAGE_READWRITE   3       1       0xfa801a6726f0  N/A     Disabled
3720    vmware-tray.ex  0xfffffa801aac3740      0xfffa7000      0xfffa9fff      Vadl    PAGE_READWRITE   3       1       0xfa801a6726f0  N/A     Disabled
3720    vmware-tray.ex  0xfffffa801a6a42a0      0xfffad000      0xfffaffff      Vadl    PAGE_READWRITE   3       1       0xfa801b3c10b0  N/A     Disabled
3720    vmware-tray.ex  0xfffffa801aee8780      0xfffde000      0xfffdefff      Vadl    PAGE_READWRITE   1       1       0xfa801a627bb0  N/A     Disabled
3720    vmware-tray.ex  0xfffffa801b3e02e0      0xfffd8000      0xfffdafff      Vadl    PAGE_READWRITE   3       1       0xfa801aee8780  N/A     Disabled
3720    vmware-tray.ex  0xfffffa801a7ded20      0xfffd5000      0xfffd7fff      Vadl    PAGE_READWRITE   3       1       0xfa801b3e02e0  N/A     Disabled
3720    vmware-tray.ex  0xfffffa801afe5500      0xfffdb000      0xfffddfff      Vadl    PAGE_READWRITE   3       1       0xfa801b3e02e0  N/A     Disabled
3720    vmware-tray.ex  0xfffffa801a5be2d0      0xfffdf000      0xfffdffff      Vadl    PAGE_READWRITE   1       1       0xfa801aee8780  N/A     Disabled
3720    vmware-tray.ex  0xfffffa801b227a20      0xfffe0000      0x7fffffeffff   Vadl    PAGE_READONLY    2251799813685247        1       0xfa801a5be2d0  N/A     Disabled

```


# windows.vadinfo.VadInfo 分析

## 1. Plugin 功能說明

`windows.vadinfo.VadInfo` 用來列出指定 Process 的 VAD（Virtual Address Descriptor）資訊。

VAD 是 Windows 用來管理行程虛擬記憶體區塊的資料結構，透過 VAD 可以觀察行程載入了哪些檔案、DLL、記憶體區段，以及各記憶體區段的權限。

在惡意程式鑑識中，`VadInfo` 可用來輔助判斷：

```text
Process 載入的檔案路徑
是否存在可疑記憶體權限
是否有 Private Memory
是否有可疑的可執行記憶體區塊
是否與 Malfind 結果相互吻合
```

---

## 2. 執行指令

本次針對兩個主要可疑 PID 執行 `VadInfo`：

```bash
.\vol.exe -f .\OtterCTF.vmem windows.vadinfo.VadInfo --pid 3820
```

```bash
.\vol.exe -f .\OtterCTF.vmem windows.vadinfo.VadInfo --pid 3720
```

---

## 3. 欄位說明

| 欄位              | 說明                            |
| --------------- | ----------------------------- |
| `PID`           | 行程編號                          |
| `Process`       | 行程名稱                          |
| `Offset`        | VAD 結構在記憶體中的位置                |
| `Start VPN`     | 記憶體區段起始位址                     |
| `End VPN`       | 記憶體區段結束位址                     |
| `Tag`           | VAD 標籤，例如 `Vad`、`VadS`、`Vadm` |
| `Protection`    | 記憶體保護權限                       |
| `CommitCharge`  | 配置的記憶體大小                      |
| `PrivateMemory` | 是否為私有記憶體                      |
| `Parent`        | VAD 父節點                       |
| `File`          | 該記憶體區段對應的檔案路徑                 |
| `File output`   | 是否有輸出檔案                       |

---

## 4. PID 3820：Rick And Morty 分析

### 4.1 主程式載入路徑

`VadInfo` 顯示 PID 3820 載入的主程式為：

```text
\Torrents\Rick And Morty season 1 download.exe
```

相關紀錄如下：

```text
PID 3820
Process: Rick And Morty
Protection: PAGE_EXECUTE_WRITECOPY
File: \Torrents\Rick And Morty season 1 download.exe
```

此結果確認 `Rick And Morty` 行程確實對應到 `C:\Torrents\Rick And Morty season 1 download.exe`。

該檔案位於 Torrents 目錄，且檔名偽裝成影片下載，但實際副檔名為 `.exe`，因此具有高度可疑性。

---

### 4.2 PID 3820 記憶體權限觀察

PID 3820 中大多數可執行區段對應到正常 Windows DLL，例如：

```text
\Windows\SysWOW64\kernel32.dll
\Windows\SysWOW64\user32.dll
\Windows\SysWOW64\ntdll.dll
\Windows\SysWOW64\shell32.dll
\Windows\SysWOW64\wininet.dll
```

這些屬於正常系統模組。

另外，PID 3820 也出現少數 `PAGE_EXECUTE_READWRITE` 且 `File = N/A` 的區塊，例如：

```text
0x774d0000 - 0x775c9fff  PAGE_EXECUTE_READWRITE  File: N/A
0x775d0000 - 0x776eefff  PAGE_EXECUTE_READWRITE  File: N/A
```

這些區塊需要注意，但前面 `Malfind` 並未針對 PID 3820 顯示明顯惡意注入結果，因此目前不作為主要惡意記憶體證據。

PID 3820 的主要價值在於確認可疑 EXE 的載入路徑。

---

## 5. PID 3720：vmware-tray.exe 分析

### 5.1 主程式載入路徑

`VadInfo` 顯示 PID 3720 載入的主程式為：

```text
\Users\Rick\AppData\Local\Temp\RarSFX0\vmware-tray.exe
```

相關紀錄如下：

```text
PID 3720
Process: vmware-tray.ex
Protection: PAGE_EXECUTE_WRITECOPY
File: \Users\Rick\AppData\Local\Temp\RarSFX0\vmware-tray.exe
```

此路徑非常可疑，因為正常 VMware 程式通常不應該位於使用者 Temp 目錄，也不應該從 `RarSFX0` 自解壓縮暫存資料夾中執行。

---

### 5.2 可疑記憶體區塊

`VadInfo` 在 PID 3720 中發現多個 `PAGE_EXECUTE_READWRITE` 且 `File = N/A` 的私有記憶體區塊：

```text
0x670000 - 0x6affff  PAGE_EXECUTE_READWRITE  PrivateMemory: 1  File: N/A
0x510000 - 0x54ffff  PAGE_EXECUTE_READWRITE  PrivateMemory: 1  File: N/A
0xc00000 - 0xc3ffff  PAGE_EXECUTE_READWRITE  PrivateMemory: 1  File: N/A
0xa10000 - 0xa4ffff  PAGE_EXECUTE_READWRITE  PrivateMemory: 1  File: N/A
```

這些位址與前面 `Malfind` 對 PID 3720 偵測到的可疑區塊一致。

`PAGE_EXECUTE_READWRITE` 代表該記憶體區塊同時具有可寫入與可執行權限。在惡意程式分析中，這種權限組合需要特別注意，因為它可能被用於：

```text
動態產生程式碼
Shellcode
程式解殼後的執行區
記憶體注入
惡意程式執行區段
```

---

### 5.3 .NET 程式跡象

PID 3720 也載入多個 .NET 相關模組，例如：

```text
\Windows\Microsoft.NET\Framework\v4.0.30319\clr.dll
\Windows\Microsoft.NET\Framework\v4.0.30319\mscoreei.dll
\Windows\Microsoft.NET\Framework\v4.0.30319\clrjit.dll
\Windows\assembly\NativeImages_v4.0.30319_32\System.Windows.Forms.ni.dll
\Windows\assembly\NativeImages_v4.0.30319_32\System.Core.ni.dll
\Windows\assembly\NativeImages_v4.0.30319_32\mscorlib.ni.dll
```

這代表 `vmware-tray.exe` 很可能是 .NET 程式或使用 .NET runtime。

此結果也與前面 `LdrModules` 中觀察到的 .NET 模組相互吻合。

---

## 6. 與 Malfind 的交叉驗證

前面 `Malfind` 在 PID 3720 中發現以下可疑區段：

```text
0x670000 - 0x6affff
0x510000 - 0x54ffff
0xc00000 - 0xc3ffff
0xa10000 - 0xa4ffff
```

本次 `VadInfo` 也顯示這些區段存在於 PID 3720，且權限皆為：

```text
PAGE_EXECUTE_READWRITE
```

並且：

```text
PrivateMemory: 1
File: N/A
```

因此，`VadInfo` 成功補強 `Malfind` 的結果，確認 PID 3720 中確實存在可疑可執行私有記憶體區塊。

---

## 7. 與其他證據的關聯

| Plugin        | 發現                                | 關聯            |
| ------------- | --------------------------------- | ------------- |
| `PsList`      | 發現 PID 3820 與 PID 3720            | 確認可疑行程存在      |
| `Pstree`      | Rick And Morty 啟動 vmware-tray.exe | 建立父子程序關係      |
| `CmdLine`     | 顯示完整執行路徑                          | 確認可疑檔案來源      |
| `UserAssist`  | Rick 使用者執行可疑程式                    | 證明使用者操作痕跡     |
| `Malfind`     | PID 3720 有可疑可執行記憶體                | 發現可疑記憶體區塊     |
| `VadInfo`     | 確認 PID 3720 可疑區塊權限與路徑             | 補強 Malfind 結果 |
| `READ_IT.txt` | 顯示檔案已被加密                          | 支持勒索/加密行為     |

---

## 8. 鑑識判斷

`VadInfo` 結果支持以下判斷：

```text
1. PID 3820 對應到 \Torrents\Rick And Morty season 1 download.exe
2. PID 3720 對應到 \Users\Rick\AppData\Local\Temp\RarSFX0\vmware-tray.exe
3. PID 3720 存在多個 PAGE_EXECUTE_READWRITE 私有記憶體區塊
4. PID 3720 的可疑區塊與 Malfind 結果一致
5. vmware-tray.exe 位於 Temp\RarSFX0，路徑不正常
```

因此，`VadInfo` 進一步確認 `vmware-tray.exe` 是本案中高度可疑的執行程式。

---

## 9. 結論

`windows.vadinfo.VadInfo` 成功補強本案的記憶體分析結果。

PID 3820 顯示主程式來自：

```text
\Torrents\Rick And Morty season 1 download.exe
```

PID 3720 顯示主程式來自：

```text
\Users\Rick\AppData\Local\Temp\RarSFX0\vmware-tray.exe
```

其中 PID 3720 `vmware-tray.exe` 存在多個 `PAGE_EXECUTE_READWRITE`、`PrivateMemory: 1`、`File: N/A` 的記憶體區塊，並且與前面 `Malfind` 發現的可疑區段一致。

因此，PID 3720 可判斷為高度可疑行程，而 PID 3820 則是主要感染來源或觸發程式。

整體事件流程可整理如下：

```text
BitTorrent 下載活動
↓
Rick 使用者執行 Rick And Morty season 1 download.exe
↓
Rick And Morty 啟動 Temp\RarSFX0\vmware-tray.exe
↓
vmware-tray.exe 產生可疑可執行記憶體區塊
↓
系統檔案遭加密
↓
READ_IT.txt 顯示加密提示
```

