# 測試內容
- .\vol.exe -f .\OtterCTF.vmem windows.vadwalk.VadWalk --pid 3820

```
D:\Forensic\G140A006\VolatilityWorkbench>.\vol.exe -f .\OtterCTF.vmem windows.vadwalk.VadWalk --pid 3820
Volatility 3 Framework 2.5.0
Progress:  100.00               PDB scanning finished
PID     Process Offset  Parent  Left    Right   Start   End     Tag

3820    Rick And Morty  0xfa801a7b7010  0xfa801b486f78  0xfa8018d71f70  0xfa801a7bc240  0x22d00000x230ffff       VadS
3820    Rick And Morty  0xfa8018d71f70  0xfa801a7b7010  0xfa801abb0550  0xfa801a53d240  0x4000000x455fff Vadm
3820    Rick And Morty  0xfa801abb0550  0xfa8018d71f70  0xfa801a627e80  0xfa801a7a9b10  0x2500000x251fff Vad
3820    Rick And Morty  0xfa801a627e80  0xfa801abb0550  0xfa801b46a6a0  0xfa801a577ac0  0x1900000x193fff Vad
3820    Rick And Morty  0xfa801b46a6a0  0xfa801a627e80  0xfa801aa92f70  0xfa801aadd420  0x40000 0x40fff  Vad
3820    Rick And Morty  0xfa801aa92f70  0xfa801b46a6a0  0xfa801b46c5c0  0xfa801aa9e010  0x20000 0x20fff  Vadm
3820    Rick And Morty  0xfa801b46c5c0  0xfa801aa92f70  0x0     0x0     0x10000 0x1ffff Vad
3820    Rick And Morty  0xfa801aa9e010  0xfa801aa92f70  0x0     0x0     0x30000 0x30fff Vadm
3820    Rick And Morty  0xfa801aadd420  0xfa801b46a6a0  0x0     0xfa801a7b4be0  0x50000 0x8ffff VadS
3820    Rick And Morty  0xfa801a7b4be0  0xfa801aadd420  0x0     0x0     0x90000 0x18ffff        VadS
3820    Rick And Morty  0xfa801a577ac0  0xfa801a627e80  0xfa801a53f850  0xfa801aa97730  0x1d00000x236fff Vad
3820    Rick And Morty  0xfa801a53f850  0xfa801a577ac0  0xfa801b491b40  0xfa801a586190  0x1b00000x1b0fff VadS
3820    Rick And Morty  0xfa801b491b40  0xfa801a53f850  0x0     0x0     0x1a0000        0x1a2fffVad
3820    Rick And Morty  0xfa801a586190  0xfa801a53f850  0x0     0x0     0x1c0000        0x1c0fffVadS
3820    Rick And Morty  0xfa801aa97730  0xfa801a577ac0  0x0     0x0     0x240000        0x244fffVad
3820    Rick And Morty  0xfa801a7a9b10  0xfa801abb0550  0xfa801a7f42c0  0xfa801b418510  0x2d00000x2dffff VadS
3820    Rick And Morty  0xfa801a7f42c0  0xfa801a7a9b10  0xfa801a51e1e0  0xfa801a56fd40  0x2a00000x2affff VadS
3820    Rick And Morty  0xfa801a51e1e0  0xfa801a7f42c0  0xfa801a5251e0  0xfa801a785170  0x2700000x27ffff VadS
3820    Rick And Morty  0xfa801a5251e0  0xfa801a51e1e0  0x0     0x0     0x260000        0x260fffVad
3820    Rick And Morty  0xfa801a785170  0xfa801a51e1e0  0x0     0x0     0x280000        0x29ffffVadS
3820    Rick And Morty  0xfa801a56fd40  0xfa801a7f42c0  0xfa801b0b2880  0x0     0x2c0000        0x2c6fff Vad
3820    Rick And Morty  0xfa801b0b2880  0xfa801a56fd40  0x0     0x0     0x2b0000        0x2b0fffVad
3820    Rick And Morty  0xfa801b418510  0xfa801a7a9b10  0xfa801a556790  0xfa801a528680  0x3200000x320fff Vad
3820    Rick And Morty  0xfa801a556790  0xfa801b418510  0xfa801aadb1a0  0xfa801a5baa60  0x2f00000x2fffff VadS
3820    Rick And Morty  0xfa801aadb1a0  0xfa801a556790  0x0     0x0     0x2e0000        0x2e1fffVad
3820    Rick And Morty  0xfa801a5baa60  0xfa801a556790  0x0     0xfa801a79c6b0  0x300000        0x300fff Vad
3820    Rick And Morty  0xfa801a79c6b0  0xfa801a5baa60  0x0     0x0     0x310000        0x313fffVad
3820    Rick And Morty  0xfa801a528680  0xfa801b418510  0xfa801a562a30  0xfa801a56f0c0  0x3b00000x3cbfff Vad
3820    Rick And Morty  0xfa801a562a30  0xfa801a528680  0x0     0x0     0x330000        0x3affffVadS
3820    Rick And Morty  0xfa801a56f0c0  0xfa801a528680  0x0     0x0     0x3d0000        0x3fffffVad
3820    Rick And Morty  0xfa801a53d240  0xfa8018d71f70  0xfa801a7caeb0  0xfa801b00d0b0  0x5400000x54ffff VadS
3820    Rick And Morty  0xfa801a7caeb0  0xfa801a53d240  0xfa801a541880  0xfa801a593fc0  0x4e00000x4e3fff Vad
3820    Rick And Morty  0xfa801a541880  0xfa801a7caeb0  0x0     0x0     0x460000        0x4dffffVadS
3820    Rick And Morty  0xfa801a593fc0  0xfa801a7caeb0  0x0     0xfa801afcca20  0x4f0000        0x52ffff VadS
3820    Rick And Morty  0xfa801afcca20  0xfa801a593fc0  0x0     0x0     0x530000        0x53dfffVad
3820    Rick And Morty  0xfa801b00d0b0  0xfa801a53d240  0xfa801a585ac0  0xfa801ad8b610  0x9e00000x1ddffff        Vad
3820    Rick And Morty  0xfa801a585ac0  0xfa801b00d0b0  0xfa801acefb90  0xfa801a7f2660  0x6c00000x847fff Vad
3820    Rick And Morty  0xfa801acefb90  0xfa801a585ac0  0xfa801a7e82c0  0x0     0x5c0000        0x6bffff Vadm
3820    Rick And Morty  0xfa801a7e82c0  0xfa801acefb90  0x0     0x0     0x550000        0x5b5fffVad
3820    Rick And Morty  0xfa801a7f2660  0xfa801a585ac0  0x0     0x0     0x850000        0x9d0fffVadm
3820    Rick And Morty  0xfa801ad8b610  0xfa801b00d0b0  0xfa80194326b0  0xfa801b3b30a0  0x1ec00000x218efff       Vad
3820    Rick And Morty  0xfa80194326b0  0xfa801ad8b610  0x0     0x0     0x1de0000       0x1ebefffVad
3820    Rick And Morty  0xfa801b3b30a0  0xfa801ad8b610  0x0     0x0     0x2190000       0x228ffffVadS
3820    Rick And Morty  0xfa801a7bc240  0xfa801a7b7010  0xfa801a7aff80  0xfa801a6b7960  0x75210000       0x7524efff      Vad
3820    Rick And Morty  0xfa801a7aff80  0xfa801a7bc240  0xfa801a7f6700  0xfa801a089260  0x6c2d0000       0x6c2e1fff      Vad
3820    Rick And Morty  0xfa801a7f6700  0xfa801a7aff80  0xfa801a79b950  0xfa801b1e8d70  0x30f00000x312ffff       VadS
3820    Rick And Morty  0xfa801a79b950  0xfa801a7f6700  0xfa801b1eeec0  0xfa801aadd6b0  0x2e800000x2f7ffff       VadS
3820    Rick And Morty  0xfa801b1eeec0  0xfa801a79b950  0xfa801a528b90  0xfa801a56ae00  0x2c400000x2d3ffff       VadS
3820    Rick And Morty  0xfa801a528b90  0xfa801b1eeec0  0x0     0x0     0x2310000       0x2c3ffffVad
3820    Rick And Morty  0xfa801a56ae00  0xfa801b1eeec0  0x0     0x0     0x2e40000       0x2e7ffffVadS
3820    Rick And Morty  0xfa801aadd6b0  0xfa801a79b950  0xfa801a52d2a0  0xfa801b0cd270  0x2fb00000x2feffff       VadS
3820    Rick And Morty  0xfa801a52d2a0  0xfa801aadd6b0  0xfa801aa3e280  0xfa801a545630  0x2f900000x2f90fff       Vad
3820    Rick And Morty  0xfa801aa3e280  0xfa801a52d2a0  0x0     0x0     0x2f80000       0x2f87fffVad
3820    Rick And Morty  0xfa801a545630  0xfa801a52d2a0  0x0     0x0     0x2fa0000       0x2facfffVad
3820    Rick And Morty  0xfa801b0cd270  0xfa801aadd6b0  0x0     0x0     0x2ff0000       0x30effffVadS
3820    Rick And Morty  0xfa801b1e8d70  0xfa801a7f6700  0xfa801aad6f40  0xfa801aa3b470  0x68770000       0x687e5fff      Vadm
3820    Rick And Morty  0xfa801aad6f40  0xfa801b1e8d70  0x0     0x0     0x3130000       0x322ffffVadS
3820    Rick And Morty  0xfa801aa3b470  0xfa801b1e8d70  0x0     0xfa801b227810  0x68870000      0x688c7fff       Vad
3820    Rick And Morty  0xfa801b227810  0xfa801aa3b470  0x0     0x0     0x68950000      0x6897dfff       Vad
3820    Rick And Morty  0xfa801a089260  0xfa801a7aff80  0xfa801afcd760  0xfa801a5ca480  0x73da0000       0x73da5fff      Vad
3820    Rick And Morty  0xfa801afcd760  0xfa801a089260  0xfa8019442120  0xfa80194ba830  0x72ce0000       0x72d2bfff      Vad
3820    Rick And Morty  0xfa8019442120  0xfa801afcd760  0xfa801a7b5b40  0xfa801a56e9c0  0x6c350000       0x6c3dcfff      Vad
3820    Rick And Morty  0xfa801a7b5b40  0xfa8019442120  0x0     0x0     0x6c2f0000      0x6c340fff       Vad
3820    Rick And Morty  0xfa801a56e9c0  0xfa8019442120  0x0     0x0     0x72080000      0x72174fff       Vad
3820    Rick And Morty  0xfa80194ba830  0xfa801afcd760  0xfa801a627c40  0xfa801a58e9e0  0x73c90000       0x73cb0fff      Vad
3820    Rick And Morty  0xfa801a627c40  0xfa80194ba830  0x0     0x0     0x73c70000      0x73c82fff       Vad
3820    Rick And Morty  0xfa801a58e9e0  0xfa80194ba830  0x0     0x0     0x73ce0000      0x73cf6fff       Vad
3820    Rick And Morty  0xfa801a5ca480  0xfa801a089260  0xfa801a7fb920  0xfa801b1f6260  0x75000000       0x7519dfff      Vad
3820    Rick And Morty  0xfa801a7fb920  0xfa801a5ca480  0xfa801a5b1890  0xfa801a56e930  0x741a0000       0x741aafff      Vad
3820    Rick And Morty  0xfa801a5b1890  0xfa801a7fb920  0x0     0x0     0x74120000      0x7419ffff       Vad
3820    Rick And Morty  0xfa801a56e930  0xfa801a7fb920  0x0     0x0     0x74820000      0x74828fff       Vad
3820    Rick And Morty  0xfa801b1f6260  0xfa801a5ca480  0x0     0xfa801b483280  0x751a0000      0x751a7fff       Vad
3820    Rick And Morty  0xfa801b483280  0xfa801b1f6260  0x0     0x0     0x751b0000      0x7520bfff       Vad
3820    Rick And Morty  0xfa801a6b7960  0xfa801a7bc240  0xfa801ab0b490  0xfa801a7d4970  0x76160000       0x7620bfff      Vad
3820    Rick And Morty  0xfa801ab0b490  0xfa801a6b7960  0xfa801a646330  0xfa801b47da20  0x75ad0000       0x75b6cfff      Vad
3820    Rick And Morty  0xfa801a646330  0xfa801ab0b490  0xfa801b0cd9e0  0xfa801b5952d0  0x756c0000       0x7574efff      Vad
3820    Rick And Morty  0xfa801b0cd9e0  0xfa801a646330  0xfa801a528710  0xfa801a56c0f0  0x754b0000       0x7559ffff      Vad
3820    Rick And Morty  0xfa801a528710  0xfa801b0cd9e0  0xfa801a53df80  0xfa801b490e30  0x75430000       0x7548ffff      Vad
3820    Rick And Morty  0xfa801a53df80  0xfa801a528710  0x0     0x0     0x75420000      0x7542bfff       Vad
3820    Rick And Morty  0xfa801b490e30  0xfa801a528710  0x0     0x0     0x75490000      0x754a1fff       Vad
3820    Rick And Morty  0xfa801a56c0f0  0xfa801b0cd9e0  0x0     0xfa801a7f9f80  0x755e0000      0x7567ffff       Vad
3820    Rick And Morty  0xfa801a7f9f80  0xfa801a56c0f0  0x0     0x0     0x75680000      0x756a6fff       Vad
3820    Rick And Morty  0xfa801b5952d0  0xfa801a646330  0xfa801a52a0e0  0xfa801a5283b0  0x757d0000       0x757d9fff      Vad
3820    Rick And Morty  0xfa801a52a0e0  0xfa801b5952d0  0x0     0x0     0x75750000      0x75794fff       Vad
3820    Rick And Morty  0xfa801a5283b0  0xfa801b5952d0  0x0     0xfa801986ad60  0x757e0000      0x758d4fff       Vad
3820    Rick And Morty  0xfa801986ad60  0xfa801a5283b0  0x0     0x0     0x759b0000      0x75accfff       Vad
3820    Rick And Morty  0xfa801b47da20  0xfa801ab0b490  0xfa801b64f890  0xfa801aac2250  0x75d30000       0x75d75fff      Vad
3820    Rick And Morty  0xfa801b64f890  0xfa801b47da20  0x0     0xfa801a585be0  0x75b70000      0x75beafff       Vad
3820    Rick And Morty  0xfa801a585be0  0xfa801b64f890  0x0     0x0     0x75bf0000      0x75d25fff       Vad
3820    Rick And Morty  0xfa801aac2250  0xfa801b47da20  0xfa801a54f010  0xfa801a561210  0x75de0000       0x75df8fff      Vad
3820    Rick And Morty  0xfa801a54f010  0xfa801aac2250  0x0     0x0     0x75d80000      0x75ddffff       Vad
3820    Rick And Morty  0xfa801a561210  0xfa801aac2250  0xfa801a55cb50  0x0     0x76000000      0x7615bfff       Vad
3820    Rick And Morty  0xfa801a55cb50  0xfa801a561210  0x0     0x0     0x75e00000      0x75ffafff       Vad
3820    Rick And Morty  0xfa801a7d4970  0xfa801a6b7960  0xfa801b000010  0xfa801aac5e00  0x7efb0000       0x7efd2fff      Vad
3820    Rick And Morty  0xfa801b000010  0xfa801a7d4970  0xfa801a40d4d0  0xfa801b0b5ce0  0x772f0000       0x773fffff      Vad
3820    Rick And Morty  0xfa801a40d4d0  0xfa801b000010  0xfa801a569f80  0xfa801afe6660  0x76f00000       0x76ffffff      Vadm
3820    Rick And Morty  0xfa801a569f80  0xfa801a40d4d0  0xfa801a71e750  0x0     0x76e70000      0x76efffff       Vad
3820    Rick And Morty  0xfa801a71e750  0xfa801a569f80  0x0     0x0     0x76220000      0x76e69fff       Vad
3820    Rick And Morty  0xfa801afe6660  0xfa801a40d4d0  0xfa801a54d6a0  0xfa801ab3dbf0  0x77200000       0x77256fff      Vad
3820    Rick And Morty  0xfa801a54d6a0  0xfa801afe6660  0x0     0x0     0x77060000      0x771fcfff       Vad
3820    Rick And Morty  0xfa801ab3dbf0  0xfa801afe6660  0x0     0x0     0x77260000      0x772e2fff       Vad
3820    Rick And Morty  0xfa801b0b5ce0  0xfa801b000010  0xfa801a7b9870  0xfa801a50b470  0x776f0000       0x77898fff      Vad
3820    Rick And Morty  0xfa801a7b9870  0xfa801b0b5ce0  0xfa801a57b940  0xfa801a547330  0x774d0000       0x775c9fff      VadS
3820    Rick And Morty  0xfa801a57b940  0xfa801a7b9870  0x0     0x0     0x77400000      0x774cbfff       Vad
3820    Rick And Morty  0xfa801a547330  0xfa801a7b9870  0x0     0x0     0x775d0000      0x776eefff       VadS
3820    Rick And Morty  0xfa801a50b470  0xfa801b0b5ce0  0xfa801a7d9200  0xfa801b485ee0  0x778d0000       0x77a4ffff      Vad
3820    Rick And Morty  0xfa801a7d9200  0xfa801a50b470  0x0     0x0     0x778a0000      0x778abfff       Vad
3820    Rick And Morty  0xfa801b485ee0  0xfa801a50b470  0xfa801a7a5f70  0x0     0x7efad000      0x7efaffff       Vadl
3820    Rick And Morty  0xfa801a7a5f70  0xfa801b485ee0  0x0     0x0     0x7efaa000      0x7efacfff       Vadl
3820    Rick And Morty  0xfa801aac5e00  0xfa801a7d4970  0xfa801a772910  0xfa801b1e8940  0x7f0e0000       0x7ffdffff      VadS
3820    Rick And Morty  0xfa801a772910  0xfa801aac5e00  0xfa801b5c3c00  0xfa801b0e2510  0x7efde000       0x7efdefff      Vadl
3820    Rick And Morty  0xfa801b5c3c00  0xfa801a772910  0xfa801b1e8a80  0x0     0x7efdb000      0x7efddfff       Vadl
3820    Rick And Morty  0xfa801b1e8a80  0xfa801b5c3c00  0x0     0x0     0x7efd5000      0x7efd7fff       Vadl
3820    Rick And Morty  0xfa801b0e2510  0xfa801a772910  0x0     0xfa801a7cae20  0x7efdf000      0x7efdffff       Vadl
3820    Rick And Morty  0xfa801a7cae20  0xfa801b0e2510  0x0     0x0     0x7efe0000      0x7f0dffff       Vad
3820    Rick And Morty  0xfa801b1e8940  0xfa801aac5e00  0x0     0xfa801b1e89e0  0x7ffe0000      0x7ffeffff       Vadl
3820    Rick And Morty  0xfa801b1e89e0  0xfa801b1e8940  0x0     0x0     0x7fff0000      0x7fffffeffff    Vadl

```

# 測試內容
- .\vol.exe -f .\OtterCTF.vmem windows.vadwalk.VadWalk --pid 3720

```
D:\Forensic\G140A006\VolatilityWorkbench>.\vol.exe -f .\OtterCTF.vmem windows.vadwalk.VadWalk --pid 3720
Volatility 3 Framework 2.5.0
Progress:  100.00               PDB scanning finished
PID     Process Offset  Parent  Left    Right   Start   End     Tag

3720    vmware-tray.ex  0xfa801aaaab00  0xfa801a4c5f78  0xfa801afec060  0xfa801a6afee0  0xec00000xf2dfff Vad
3720    vmware-tray.ex  0xfa801afec060  0xfa801aaaab00  0xfa801ac9c8a0  0xfa801ad6a0f0  0x3300000x3affff VadS
3720    vmware-tray.ex  0xfa801ac9c8a0  0xfa801afec060  0xfa801b4f2bd0  0xfa801a46c1f0  0x1100000x14ffff VadS
3720    vmware-tray.ex  0xfa801b4f2bd0  0xfa801ac9c8a0  0xfa801afe6770  0xfa801a591530  0x60000 0x60fff  Vad
3720    vmware-tray.ex  0xfa801afe6770  0xfa801b4f2bd0  0xfa801ad15c00  0xfa801aa635e0  0x40000 0x40fff  Vad
3720    vmware-tray.ex  0xfa801ad15c00  0xfa801afe6770  0xfa801a5c43e0  0xfa801b536bb0  0x20000 0x20fff  Vadm
3720    vmware-tray.ex  0xfa801a5c43e0  0xfa801ad15c00  0x0     0x0     0x10000 0x1ffff Vad
3720    vmware-tray.ex  0xfa801b536bb0  0xfa801ad15c00  0x0     0x0     0x30000 0x30fff Vadm
3720    vmware-tray.ex  0xfa801aa635e0  0xfa801afe6770  0x0     0x0     0x50000 0x53fff Vad
3720    vmware-tray.ex  0xfa801a591530  0xfa801b4f2bd0  0xfa801a7b94c0  0xfa801a6cf9a0  0x80000 0xe6fff  Vad
3720    vmware-tray.ex  0xfa801a7b94c0  0xfa801a591530  0x0     0x0     0x70000 0x70fff VadS
3720    vmware-tray.ex  0xfa801a6cf9a0  0xfa801a591530  0x0     0xfa801a597110  0xf0000 0xf0fff Vad
3720    vmware-tray.ex  0xfa801a597110  0xfa801a6cf9a0  0x0     0x0     0x100000        0x10ffffVad
3720    vmware-tray.ex  0xfa801a46c1f0  0xfa801ac9c8a0  0xfa801a4dc180  0xfa801b2fa4b0  0x1b00000x1b0fff VadS
3720    vmware-tray.ex  0xfa801a4dc180  0xfa801a46c1f0  0xfa801ac660f0  0xfa801b0e92a0  0x1700000x17ffff VadS
3720    vmware-tray.ex  0xfa801ac660f0  0xfa801a4dc180  0xfa801b0c4430  0x0     0x160000        0x16ffff VadS
3720    vmware-tray.ex  0xfa801b0c4430  0xfa801ac660f0  0x0     0x0     0x150000        0x15ffffVadS
3720    vmware-tray.ex  0xfa801b0e92a0  0xfa801a4dc180  0xfa801aaab340  0xfa801a42a240  0x1900000x19ffff VadS
3720    vmware-tray.ex  0xfa801aaab340  0xfa801b0e92a0  0x0     0x0     0x180000        0x18ffffVadS
3720    vmware-tray.ex  0xfa801a42a240  0xfa801b0e92a0  0x0     0x0     0x1a0000        0x1affffVadS
3720    vmware-tray.ex  0xfa801b2fa4b0  0xfa801a46c1f0  0xfa801a7d5510  0xfa801aabb9d0  0x1f00000x2effff Vadm
3720    vmware-tray.ex  0xfa801a7d5510  0xfa801b2fa4b0  0xfa801a46c3a0  0xfa801a57db80  0x1d00000x1dffff VadS
3720    vmware-tray.ex  0xfa801a46c3a0  0xfa801a7d5510  0x0     0x0     0x1c0000        0x1c0fffVadS
3720    vmware-tray.ex  0xfa801a57db80  0xfa801a7d5510  0x0     0x0     0x1e0000        0x1effffVadS
3720    vmware-tray.ex  0xfa801aabb9d0  0xfa801b2fa4b0  0xfa801afe1070  0xfa801af7deb0  0x3000000x301fff Vad
3720    vmware-tray.ex  0xfa801afe1070  0xfa801aabb9d0  0x0     0x0     0x2f0000        0x2fffffVadS
3720    vmware-tray.ex  0xfa801af7deb0  0xfa801aabb9d0  0xfa801af75240  0x0     0x320000        0x321fff Vad
3720    vmware-tray.ex  0xfa801af75240  0xfa801af7deb0  0x0     0x0     0x310000        0x31ffffVadS
3720    vmware-tray.ex  0xfa801ad6a0f0  0xfa801afec060  0xfa801a4baef0  0xfa801a4b5ae0  0x6700000x6affff VadS
3720    vmware-tray.ex  0xfa801a4baef0  0xfa801ad6a0f0  0xfa801b5a00f0  0xfa801a42a090  0x5100000x54ffff VadS
3720    vmware-tray.ex  0xfa801b5a00f0  0xfa801a4baef0  0xfa801a785280  0xfa801aa06f80  0x3f00000x4effff Vadm
3720    vmware-tray.ex  0xfa801a785280  0xfa801b5a00f0  0xfa801b3a9c20  0xfa801ace0680  0x3d00000x3dffff VadS
3720    vmware-tray.ex  0xfa801b3a9c20  0xfa801a785280  0x0     0x0     0x3b0000        0x3cffffVadS
3720    vmware-tray.ex  0xfa801ace0680  0xfa801a785280  0x0     0x0     0x3e0000        0x3e0fffVadm
3720    vmware-tray.ex  0xfa801aa06f80  0xfa801b5a00f0  0x0     0xfa801a53d650  0x4f0000        0x4f0fff Vad
3720    vmware-tray.ex  0xfa801a53d650  0xfa801aa06f80  0x0     0x0     0x500000        0x500fffVadm
3720    vmware-tray.ex  0xfa801a42a090  0xfa801a4baef0  0xfa801af3d200  0xfa801a5e6340  0x5900000x59ffff VadS
3720    vmware-tray.ex  0xfa801af3d200  0xfa801a42a090  0x0     0x0     0x550000        0x56dfffVadm
3720    vmware-tray.ex  0xfa801a5e6340  0xfa801a42a090  0x0     0xfa801a73d920  0x5d0000        0x5dffff VadS
3720    vmware-tray.ex  0xfa801a73d920  0xfa801a5e6340  0x0     0x0     0x600000        0x63ffffVadS
3720    vmware-tray.ex  0xfa801a4b5ae0  0xfa801ad6a0f0  0xfa801b0533e0  0xfa801a416df0  0xc000000xc3ffff VadS
3720    vmware-tray.ex  0xfa801b0533e0  0xfa801a4b5ae0  0xfa801b1f2fc0  0xfa801adaf990  0xa100000xa4ffff VadS
3720    vmware-tray.ex  0xfa801b1f2fc0  0xfa801b0533e0  0xfa801b52b8a0  0xfa8018e01010  0x8400000x84ffff VadS
3720    vmware-tray.ex  0xfa801b52b8a0  0xfa801b1f2fc0  0x0     0x0     0x6b0000        0x837fffVad
3720    vmware-tray.ex  0xfa8018e01010  0xfa801b1f2fc0  0x0     0x0     0x850000        0x9d0fffVadm
3720    vmware-tray.ex  0xfa801adaf990  0xfa801b0533e0  0xfa801b30ac00  0xfa801aad6be0  0xb100000xb4ffff VadS
3720    vmware-tray.ex  0xfa801b30ac00  0xfa801adaf990  0x0     0x0     0xa50000        0xaeffffVadS
3720    vmware-tray.ex  0xfa801aad6be0  0xfa801adaf990  0x0     0x0     0xb70000        0xbaffffVadS
3720    vmware-tray.ex  0xfa801a416df0  0xfa801a4b5ae0  0xfa801a4b5d50  0xfa801919e8d0  0xe100000xe4ffff VadS
3720    vmware-tray.ex  0xfa801a4b5d50  0xfa801a416df0  0xfa801b4636d0  0xfa801a56ff80  0xc900000xd8ffff VadS
3720    vmware-tray.ex  0xfa801b4636d0  0xfa801a4b5d50  0x0     0x0     0xc50000        0xc8ffffVadS
3720    vmware-tray.ex  0xfa801a56ff80  0xfa801a4b5d50  0x0     0x0     0xd90000        0xdeafffVad
3720    vmware-tray.ex  0xfa801919e8d0  0xfa801a416df0  0x0     0x0     0xe60000        0xe9ffffVadS
3720    vmware-tray.ex  0xfa801a6afee0  0xfa801aaaab00  0xfa801a46a260  0xfa801a6448b0  0x74a00000       0x74a65fff      Vad
3720    vmware-tray.ex  0xfa801a46a260  0xfa801a6afee0  0xfa801a6b8670  0xfa801a2f5240  0x66660000       0x667f5fff      Vad
3720    vmware-tray.ex  0xfa801a6b8670  0xfa801a46a260  0xfa801b0b5120  0xfa801b5cb4b0  0x4f200000x4f95fff       VadS
3720    vmware-tray.ex  0xfa801b0b5120  0xfa801a6b8670  0xfa801a416f00  0xfa801a627630  0x49600000x4a5ffff       VadS
3720    vmware-tray.ex  0xfa801a416f00  0xfa801b0b5120  0xfa801a73aae0  0xfa801a406010  0x44800000x457ffff       VadS
3720    vmware-tray.ex  0xfa801a73aae0  0xfa801a416f00  0xfa801b558510  0xfa801b1f7200  0x23300000x432ffff       Vadm
3720    vmware-tray.ex  0xfa801b558510  0xfa801a73aae0  0x0     0x0     0xf30000        0x232ffffVad
3720    vmware-tray.ex  0xfa801b1f7200  0xfa801a73aae0  0x0     0xfa801b3dfa00  0x4330000       0x440efff        Vad
3720    vmware-tray.ex  0xfa801b3dfa00  0xfa801b1f7200  0x0     0x0     0x4410000       0x444ffffVadS
3720    vmware-tray.ex  0xfa801a406010  0xfa801a416f00  0x0     0xfa801a7dc210  0x4580000       0x484efff        Vad
3720    vmware-tray.ex  0xfa801a7dc210  0xfa801a406010  0x0     0x0     0x4850000       0x494ffffVadS
3720    vmware-tray.ex  0xfa801a627630  0xfa801b0b5120  0xfa801a56aa20  0xfa801ab4f830  0x4e900000x4e9ffff       VadS
3720    vmware-tray.ex  0xfa801a56aa20  0xfa801a627630  0x0     0xfa801ad8dca0  0x4a60000       0x4d31fff        Vad
3720    vmware-tray.ex  0xfa801ad8dca0  0xfa801a56aa20  0x0     0x0     0x4d70000       0x4e6ffffVadS
3720    vmware-tray.ex  0xfa801ab4f830  0xfa801a627630  0x0     0x0     0x4ea0000       0x4f1ffffVadS
3720    vmware-tray.ex  0xfa801b5cb4b0  0xfa801a6b8670  0xfa801a6c58a0  0xfa801aa64f70  0x54d00000x5dfffff       Vad
3720    vmware-tray.ex  0xfa801a6c58a0  0xfa801b5cb4b0  0xfa801a5863c0  0xfa801b1aa380  0x50e00000x511ffff       VadS
3720    vmware-tray.ex  0xfa801a5863c0  0xfa801a6c58a0  0x0     0x0     0x4fa0000       0x509ffffVadS
3720    vmware-tray.ex  0xfa801b1aa380  0xfa801a6c58a0  0xfa801aa64fc0  0x0     0x52d0000       0x54cffff        VadS
3720    vmware-tray.ex  0xfa801aa64fc0  0xfa801b1aa380  0x0     0x0     0x5240000       0x527ffffVadS
3720    vmware-tray.ex  0xfa801aa64f70  0xfa801b5cb4b0  0xfa801b438bd0  0xfa801aea1ae0  0x7bd00000x7ccffff       VadS
3720    vmware-tray.ex  0xfa801b438bd0  0xfa801aa64f70  0xfa801a656590  0xfa801a6351a0  0x79700000x7a6ffff       VadS
3720    vmware-tray.ex  0xfa801a656590  0xfa801b438bd0  0x0     0x0     0x5e00000       0x789ffffVadS
3720    vmware-tray.ex  0xfa801a6351a0  0xfa801b438bd0  0x0     0x0     0x7a80000       0x7b7ffffVadS
3720    vmware-tray.ex  0xfa801aea1ae0  0xfa801aa64f70  0x0     0xfa801a585430  0x65330000      0x659e5fff       Vad
3720    vmware-tray.ex  0xfa801a585430  0xfa801aea1ae0  0x0     0x0     0x659f0000      0x6665afff       Vad
3720    vmware-tray.ex  0xfa801a2f5240  0xfa801a46a260  0xfa801b19e380  0xfa801a0b5390  0x69720000       0x697ddfff      Vad
3720    vmware-tray.ex  0xfa801b19e380  0xfa801a2f5240  0xfa801a528c20  0xfa801aaa4ef0  0x68070000       0x686defff      Vad
3720    vmware-tray.ex  0xfa801a528c20  0xfa801b19e380  0xfa801b19eb60  0xfa801a733390  0x670a0000       0x67e62fff      Vad
3720    vmware-tray.ex  0xfa801b19eb60  0xfa801a528c20  0x0     0x0     0x66800000      0x67097fff       Vad
3720    vmware-tray.ex  0xfa801a733390  0xfa801a528c20  0x0     0x0     0x68010000      0x6806ffff       Vad
3720    vmware-tray.ex  0xfa801aaa4ef0  0xfa801b19e380  0x0     0x0     0x68860000      0x6886ffff       Vad
3720    vmware-tray.ex  0xfa801a0b5390  0xfa801a2f5240  0xfa801aefd4b0  0xfa801ae3aac0  0x73fe0000       0x74063fff      Vad
3720    vmware-tray.ex  0xfa801aefd4b0  0xfa801a0b5390  0xfa801b5886b0  0xfa801a627460  0x73c70000       0x73c82fff      Vad
3720    vmware-tray.ex  0xfa801b5886b0  0xfa801aefd4b0  0x0     0x0     0x71990000      0x71a8afff       Vad
3720    vmware-tray.ex  0xfa801a627460  0xfa801aefd4b0  0x0     0x0     0x73f60000      0x73f76fff       Vad
3720    vmware-tray.ex  0xfa801ae3aac0  0xfa801a0b5390  0xfa801b0ae0e0  0xfa801ae95ce0  0x741a0000       0x741aafff      Vad
3720    vmware-tray.ex  0xfa801b0ae0e0  0xfa801ae3aac0  0xfa801ad0fb00  0xfa801a561180  0x74100000       0x74115fff      Vad
3720    vmware-tray.ex  0xfa801ad0fb00  0xfa801b0ae0e0  0x0     0x0     0x740c0000      0x740fafff       Vad
3720    vmware-tray.ex  0xfa801a561180  0xfa801b0ae0e0  0x0     0x0     0x74120000      0x7419ffff       Vad
3720    vmware-tray.ex  0xfa801ae95ce0  0xfa801ae3aac0  0x0     0x0     0x74870000      0x749fffff       Vad
3720    vmware-tray.ex  0xfa801a6448b0  0xfa801a6afee0  0xfa801a7df6f0  0xfa801b5685b0  0x774d0000       0x775c9fff      VadS
3720    vmware-tray.ex  0xfa801a7df6f0  0xfa801a6448b0  0xfa801b050840  0xfa801a79b8c0  0x754b0000       0x7559ffff      Vad
3720    vmware-tray.ex  0xfa801b050840  0xfa801a7df6f0  0xfa801b485c60  0xfa801a520a00  0x75210000       0x7524efff      Vad
3720    vmware-tray.ex  0xfa801b485c60  0xfa801b050840  0xfa801ae4aca0  0xfa801b4857b0  0x751a0000       0x751a7fff      Vad
3720    vmware-tray.ex  0xfa801ae4aca0  0xfa801b485c60  0x0     0xfa801b48c100  0x74f60000      0x74fa9fff       Vad
3720    vmware-tray.ex  0xfa801b48c100  0xfa801ae4aca0  0x0     0x0     0x75000000      0x7519dfff       Vad
3720    vmware-tray.ex  0xfa801b4857b0  0xfa801b485c60  0x0     0x0     0x751b0000      0x7520bfff       Vad
3720    vmware-tray.ex  0xfa801a520a00  0xfa801b050840  0xfa801ab21700  0x0     0x75430000      0x7548ffff       Vad
3720    vmware-tray.ex  0xfa801ab21700  0xfa801a520a00  0x0     0x0     0x75420000      0x7542bfff       Vad
3720    vmware-tray.ex  0xfa801a79b8c0  0xfa801a7df6f0  0xfa801a7fba60  0xfa801ad6bc60  0x76160000       0x7620bfff      Vad
3720    vmware-tray.ex  0xfa801a7fba60  0xfa801a79b8c0  0xfa801b19b4b0  0xfa801ac9e150  0x75d30000       0x75d75fff      Vad
3720    vmware-tray.ex  0xfa801b19b4b0  0xfa801a7fba60  0xfa801b439370  0xfa801b42e280  0x757d0000       0x757d9fff      Vad
3720    vmware-tray.ex  0xfa801b439370  0xfa801b19b4b0  0x0     0x0     0x755e0000      0x7567ffff       Vad
3720    vmware-tray.ex  0xfa801b42e280  0xfa801b19b4b0  0x0     0x0     0x75ad0000      0x75b6cfff       Vad
3720    vmware-tray.ex  0xfa801ac9e150  0xfa801a7fba60  0xfa801af4a870  0xfa8019fbbc90  0x75de0000       0x75df8fff      Vad
3720    vmware-tray.ex  0xfa801af4a870  0xfa801ac9e150  0x0     0x0     0x75d80000      0x75ddffff       Vad
3720    vmware-tray.ex  0xfa8019fbbc90  0xfa801ac9e150  0x0     0x0     0x76000000      0x7615bfff       Vad
3720    vmware-tray.ex  0xfa801ad6bc60  0xfa801a79b8c0  0xfa801b502a00  0xfa80195bf8a0  0x77200000       0x77256fff      Vad
3720    vmware-tray.ex  0xfa801b502a00  0xfa801ad6bc60  0xfa801b1f5580  0xfa801a614590  0x76e70000       0x76efffff      Vad
3720    vmware-tray.ex  0xfa801b1f5580  0xfa801b502a00  0x0     0x0     0x76220000      0x76e69fff       Vad
3720    vmware-tray.ex  0xfa801a614590  0xfa801b502a00  0x0     0x0     0x76f00000      0x76ffffff       Vadm
3720    vmware-tray.ex  0xfa80195bf8a0  0xfa801ad6bc60  0x0     0xfa801b3d7a80  0x772f0000      0x773fffff       Vad
3720    vmware-tray.ex  0xfa801b3d7a80  0xfa80195bf8a0  0x0     0x0     0x77400000      0x774cbfff       Vad
3720    vmware-tray.ex  0xfa801b5685b0  0xfa801a6448b0  0xfa801a7963b0  0xfa801a627bb0  0x80000000       0x8000ffff      VadS
3720    vmware-tray.ex  0xfa801a7963b0  0xfa801b5685b0  0xfa801a0a5510  0xfa801b59d580  0x7f0e0000       0x7ffdffff      VadS
3720    vmware-tray.ex  0xfa801a0a5510  0xfa801a7963b0  0xfa801a7e7530  0xfa80197aabf0  0x776f0000       0x77898fff      Vad
3720    vmware-tray.ex  0xfa801a7e7530  0xfa801a0a5510  0x0     0x0     0x775d0000      0x776eefff       VadS
3720    vmware-tray.ex  0xfa80197aabf0  0xfa801a0a5510  0x0     0xfa801a5699a0  0x778d0000      0x77a4ffff       Vad
3720    vmware-tray.ex  0xfa801a5699a0  0xfa80197aabf0  0x0     0x0     0x7efe0000      0x7f0dffff       Vad
3720    vmware-tray.ex  0xfa801b59d580  0xfa801a7963b0  0xfa801b0aa520  0x0     0x7fff0000      0x7fffffff       VadS
3720    vmware-tray.ex  0xfa801b0aa520  0xfa801b59d580  0x0     0x0     0x7ffe0000      0x7ffeffff       Vadl
3720    vmware-tray.ex  0xfa801a627bb0  0xfa801b5685b0  0xfa801b3c10b0  0xfa801aee8780  0xfffb0000       0xfffd2fff      Vad
3720    vmware-tray.ex  0xfa801b3c10b0  0xfa801a627bb0  0xfa801a6726f0  0xfa801a6a42a0  0xfffaa000       0xfffacfff      Vadl
3720    vmware-tray.ex  0xfa801a6726f0  0xfa801b3c10b0  0xfa801a4f07c0  0xfa801aac3740  0xfffa4000       0xfffa6fff      Vadl
3720    vmware-tray.ex  0xfa801a4f07c0  0xfa801a6726f0  0x0     0x0     0xfffa1000      0xfffa3fff       Vadl
3720    vmware-tray.ex  0xfa801aac3740  0xfa801a6726f0  0x0     0x0     0xfffa7000      0xfffa9fff       Vadl
3720    vmware-tray.ex  0xfa801a6a42a0  0xfa801b3c10b0  0x0     0x0     0xfffad000      0xfffaffff       Vadl
3720    vmware-tray.ex  0xfa801aee8780  0xfa801a627bb0  0xfa801b3e02e0  0xfa801a5be2d0  0xfffde000       0xfffdefff      Vadl
3720    vmware-tray.ex  0xfa801b3e02e0  0xfa801aee8780  0xfa801a7ded20  0xfa801afe5500  0xfffd8000       0xfffdafff      Vadl
3720    vmware-tray.ex  0xfa801a7ded20  0xfa801b3e02e0  0x0     0x0     0xfffd5000      0xfffd7fff       Vadl
3720    vmware-tray.ex  0xfa801afe5500  0xfa801b3e02e0  0x0     0x0     0xfffdb000      0xfffddfff       Vadl
3720    vmware-tray.ex  0xfa801a5be2d0  0xfa801aee8780  0x0     0xfa801b227a20  0xfffdf000      0xfffdffff       Vadl
3720    vmware-tray.ex  0xfa801b227a20  0xfa801a5be2d0  0x0     0x0     0xfffe0000      0x7fffffeffff    Vadl
```


# windows.vadwalk.VadWalk 分析

## 1. Plugin 功能說明

`windows.vadwalk.VadWalk` 用來走訪指定 Process 的 VAD Tree。

VAD 是 Windows 用來管理行程虛擬記憶體區段的資料結構。透過 `VadWalk` 可以查看某個 Process 的 VAD 節點、記憶體起始位置、結束位置，以及 VAD 節點之間的父子關係。

在數位鑑識中，`VadWalk` 可用來輔助確認可疑 Process 是否存在特定記憶體區段，並與 `VadInfo`、`Malfind` 進行交叉比對。

---

## 2. 執行指令

本次針對兩個主要可疑 PID 執行：

```bash
.\vol.exe -f .\OtterCTF.vmem windows.vadwalk.VadWalk --pid 3820
```

```bash
.\vol.exe -f .\OtterCTF.vmem windows.vadwalk.VadWalk --pid 3720
```

---

## 3. 欄位說明

| 欄位        | 說明                                     |
| --------- | -------------------------------------- |
| `PID`     | 行程編號                                   |
| `Process` | 行程名稱                                   |
| `Offset`  | VAD 節點在記憶體中的位置                         |
| `Parent`  | 父 VAD 節點                               |
| `Left`    | 左子節點                                   |
| `Right`   | 右子節點                                   |
| `Start`   | 記憶體區段起始位址                              |
| `End`     | 記憶體區段結束位址                              |
| `Tag`     | VAD 類型標籤，例如 `Vad`、`VadS`、`Vadm`、`Vadl` |

---

## 4. PID 3820：Rick And Morty 分析

`VadWalk` 顯示 PID 3820 `Rick And Morty` 存在大量 VAD 節點，代表該 Process 有正常的記憶體配置與 DLL 載入狀態。

其中可觀察到主程式附近的 VAD 區段：

```text
Start: 0x400000
End:   0x455fff
Tag:   Vadm
```

此區段與前面 `VadInfo` 中的結果相符。

前面 `VadInfo` 已確認此區段對應到：

```text
\Torrents\Rick And Morty season 1 download.exe
```

因此，`VadWalk` 可補強 PID 3820 確實存在此程式的 VAD 記憶體結構。

---

## 5. PID 3720：vmware-tray.exe 分析

`VadWalk` 顯示 PID 3720 `vmware-tray.ex` 存在多個 VAD 節點。

其中最重要的是以下幾個區段：

```text
Start: 0x670000
End:   0x6affff
Tag:   VadS

Start: 0x510000
End:   0x54ffff
Tag:   VadS

Start: 0xc00000
End:   0xc3ffff
Tag:   VadS

Start: 0xa10000
End:   0xa4ffff
Tag:   VadS
```

這些區段與前面 `Malfind` 和 `VadInfo` 的發現一致。

前面 `VadInfo` 顯示這些區段具有：

```text
PAGE_EXECUTE_READWRITE
PrivateMemory: 1
File: N/A
```

因此，`VadWalk` 結果可用來確認這些可疑記憶體區段確實存在於 PID 3720 的 VAD Tree 中。

---

## 6. 與 VadInfo / Malfind 的交叉驗證

本案中三個 Plugin 的關聯如下：

| Plugin    | 功能             | 本案發現                                             |
| --------- | -------------- | ------------------------------------------------ |
| `Malfind` | 偵測可疑可執行記憶體     | 發現 PID 3720 有多個 `PAGE_EXECUTE_READWRITE` 區段      |
| `VadInfo` | 顯示 VAD 權限與對應檔案 | 確認 PID 3720 可疑區段為 `PrivateMemory: 1`、`File: N/A` |
| `VadWalk` | 走訪 VAD Tree    | 確認相同區段存在於 PID 3720 的 VAD 節點中                     |

三者互相補強，表示 PID 3720 的可疑記憶體區段不是單一 Plugin 的誤判，而是在不同 VAD 分析 Plugin 中都可以觀察到。
