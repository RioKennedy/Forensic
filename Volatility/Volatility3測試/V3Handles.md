# 測試內容


- vol.exe -f .\OtterCTF.vmem windows.handles.Handles --pid 3820
```
D:\Forensic\G140A006\VolatilityWorkbench>.\vol.exe -f .\OtterCTF.vmem windows.handles.Handles --pid 3820
Volatility 3 Framework 2.5.0
Progress:  100.00               PDB scanning finished
PID     Process Offset  HandleValue     Type    GrantedAccess   Name

3820    Rick And Morty  0xf8a003346dd0  0x4     Key     0x9     MACHINE\SOFTWARE\MICROSOFT\WINDOWS NT\CURRENTVERSION\IMAGE FILE EXECUTION OPTIONS
3820    Rick And Morty  0xf8a000566af0  0x8     Directory       0x3     KnownDlls
3820    Rick And Morty  0xf8a0038d5990  0xc     Directory       0x3     KnownDlls32
3820    Rick And Morty  0xfa801a7ce260  0x10    File    0x100020        \Device\HarddiskVolume1\Windows
3820    Rick And Morty  0xf8a00336f800  0x14    Key     0x9     MACHINE\SOFTWARE\MICROSOFT\WINDOWS NT\CURRENTVERSION\IMAGE FILE EXECUTION OPTIONS
3820    Rick And Morty  0xf8a0038d5990  0x18    Directory       0x3     KnownDlls32
3820    Rick And Morty  0xfa801b0c4760  0x1c    EtwRegistration 0x804
3820    Rick And Morty  0xfa801a5e0070  0x20    File    0x100020        \Device\HarddiskVolume1\Windows\winsxs\x86_microsoft.windows.common-controls_6595b64144ccf1df_6.0.7601.17514_none_41e6975e2bd6f2b2
3820    Rick And Morty  0xfa801adc74b0  0x24    Semaphore       0x100003
3820    Rick And Morty  0xfa801b48de60  0x28    ALPC Port       0x1f0001
3820    Rick And Morty  0xfa801b237060  0x2c    Semaphore       0x100003
3820    Rick And Morty  0xf8a003338fa0  0x30    Key     0x1     MACHINE\SYSTEM\CONTROLSET001\CONTROL\NLS\CUSTOMLOCALE
3820    Rick And Morty  0xf8a001e0c600  0x34    Key     0x20019 MACHINE\SYSTEM\CONTROLSET001\CONTROL\NLS\SORTING\VERSIONS
3820    Rick And Morty  0xfa801a796ac0  0x38    Mutant  0x1f0001
3820    Rick And Morty  0xf8a00377a470  0x3c    Key     0x20019 MACHINE
3820    Rick And Morty  0xfa801a7bceb0  0x40    Event   0x1f0003
3820    Rick And Morty  0xf8a0001cdac0  0x44    Key     0x1     MACHINE\SYSTEM\CONTROLSET001\CONTROL\SESSION MANAGER
3820    Rick And Morty  0xfa801a7db190  0x48    EtwRegistration 0x804
3820    Rick And Morty  0xfa801b3d13c0  0x4c    Event   0x21f0003
3820    Rick And Morty  0xfa801ab08cc0  0x50    WindowStation   0xf037f WinSta0
3820    Rick And Morty  0xfa801aaeaeb0  0x54    Desktop 0xf01ff Default
3820    Rick And Morty  0xfa801ab08cc0  0x58    WindowStation   0xf037f WinSta0
3820    Rick And Morty  0xfa801a4e4a20  0x5c    EtwRegistration 0x804
3820    Rick And Morty  0xfa801ab4b870  0x60    EtwRegistration 0x804
3820    Rick And Morty  0xfa801af12760  0x64    EtwRegistration 0x804
3820    Rick And Morty  0xfa801a578e50  0x68    EtwRegistration 0x804
3820    Rick And Morty  0xfa801b1d8b90  0x6c    EtwRegistration 0x804
3820    Rick And Morty  0xfa801adf7ab0  0x70    EtwRegistration 0x804
3820    Rick And Morty  0xfa801ae6b9d0  0x74    EtwRegistration 0x804
3820    Rick And Morty  0xfa801b538150  0x78    EtwRegistration 0x804
3820    Rick And Morty  0xfa801acae9b0  0x7c    EtwRegistration 0x804
3820    Rick And Morty  0xfa801b54ad60  0x80    EtwRegistration 0x804
3820    Rick And Morty  0xfa801ad45fb0  0x84    EtwRegistration 0x804
3820    Rick And Morty  0xfa801b550f20  0x88    EtwRegistration 0x804
3820    Rick And Morty  0xfa801ad99260  0x8c    EtwRegistration 0x804
3820    Rick And Morty  0xfa801ae86240  0x90    EtwRegistration 0x804
3820    Rick And Morty  0xfa801a5209c0  0x94    Event   0x1f0003
3820    Rick And Morty  0xfa801afef100  0x98    Event   0x1f0003
3820    Rick And Morty  0xfa801a3d01b0  0x9c    Event   0x1f0003
3820    Rick And Morty  0xfa80193c13f0  0xa0    Event   0x1f0003
3820    Rick And Morty  0xfa801a637220  0xa4    Event   0x1f0003
3820    Rick And Morty  0xfa801ae471e0  0xa8    Event   0x1f0003
3820    Rick And Morty  0xf8a0015481c0  0xac    Directory       0xf     BaseNamedObjects
3820    Rick And Morty  0xfa801a635e30  0xb0    EtwRegistration 0x804
3820    Rick And Morty  0xfa801a577070  0xb4    EtwRegistration 0x804
3820    Rick And Morty  0xfa801ac28440  0xb8    EtwRegistration 0x804
3820    Rick And Morty  0xfa801ad94790  0xbc    EtwRegistration 0x804
3820    Rick And Morty  0xfa801ac29900  0xc0    EtwRegistration 0x804
3820    Rick And Morty  0xfa801aa38fb0  0xc4    EtwRegistration 0x804
3820    Rick And Morty  0xfa801aaa0cd0  0xc8    EtwRegistration 0x804
3820    Rick And Morty  0xfa801a7e7770  0xcc    Event   0x1f0003
3820    Rick And Morty  0xf8a002744560  0xd0    Key     0x20019 MACHINE\SYSTEM\CONTROLSET001\CONTROL\NETWORKPROVIDER\HWORDER
3820    Rick And Morty  0xfa801a7f5c00  0xd4    Semaphore       0x100003
3820    Rick And Morty  0xfa801a7f5c80  0xd8    Semaphore       0x100003
3820    Rick And Morty  0xfa801a599630  0xdc    Event   0x1f0003
3820    Rick And Morty  0xfa801ac0b810  0xe0    Event   0x1f0003
3820    Rick And Morty  0xfa801b40a500  0xe4    File    0x100001        \Device\KsecDD
3820    Rick And Morty  0xfa801a566590  0xe8    EtwRegistration 0x804
3820    Rick And Morty  0xfa80193af570  0xec    EtwRegistration 0x804
3820    Rick And Morty  0xfa801a6bbe60  0xf0    ALPC Port       0x1f0001
3820    Rick And Morty  0xf8a0018403b0  0xf4    Section 0x4
3820    Rick And Morty  0xf8a003356120  0xf8    Key     0x20019 MACHINE\SYSTEM\CONTROLSET001\CONTROL\NLS\LOCALE
3820    Rick And Morty  0xf8a0063f8be0  0xfc    Key     0x20019 MACHINE\SYSTEM\CONTROLSET001\CONTROL\NLS\LOCALE\ALTERNATE SORTS
3820    Rick And Morty  0xf8a0064242a0  0x100   Key     0x20019 MACHINE\SYSTEM\CONTROLSET001\CONTROL\NLS\LANGUAGE GROUPS
3820    Rick And Morty  0xfa80194124c0  0x104   EtwRegistration 0x804
3820    Rick And Morty  0xfa801a592530  0x108   EtwRegistration 0x804
3820    Rick And Morty  0xfa801b5accc0  0x10c   File    0x120089        \Device\HarddiskVolume1\Windows\SysWOW64\en-US\user32.dll.mui
3820    Rick And Morty  0xfa8018e4d5b0  0x110   File    0x100020        \Device\HarddiskVolume1\Windows\winsxs\x86_microsoft.windows.common-controls_6595b64144ccf1df_6.0.7601.17514_none_41e6975e2bd6f2b2
3820    Rick And Morty  0xfa801b0dfdd0  0x114   File    0x120089        \Device\HarddiskVolume1\Windows\Fonts\StaticCache.dat
3820    Rick And Morty  0xf8a00156afc0  0x118   Section 0xf0005
3820    Rick And Morty  0xf8a006302970  0x11c   Key     0x20019 MACHINE\SOFTWARE\POLICIES
3820    Rick And Morty  0xf8a0015bcad0  0x120   Key     0xf003f USER\S-1-5-21-1923827501-2510115606-422599235-1000
3820    Rick And Morty  0xf8a003357690  0x124   Key     0x20019 USER\S-1-5-21-1923827501-2510115606-422599235-1000\SOFTWARE\POLICIES
3820    Rick And Morty  0xf8a0001cd8f0  0x128   Key     0x20019 USER\S-1-5-21-1923827501-2510115606-422599235-1000\SOFTWARE
3820    Rick And Morty  0xf8a00377ab90  0x12c   Key     0x20019 MACHINE\SOFTWARE\WOW6432NODE
3820    Rick And Morty  0xf8a001756b00  0x130   Section 0x4     __ComCatalogCache__
3820    Rick And Morty  0xf8a002605e30  0x134   Key     0xf003f USER\S-1-5-21-1923827501-2510115606-422599235-1000_CLASSES
3820    Rick And Morty  0xfa8018dc4140  0x138   Event   0x100001        MaximumCommitCondition
3820    Rick And Morty  0xf8a001756b00  0x13c   Section 0x4     __ComCatalogCache__
3820    Rick And Morty  0xfa801a630070  0x140   EtwRegistration 0x804
3820    Rick And Morty  0xfa801b3bfe90  0x144   File    0x120089        \Device\HarddiskVolume1\Windows\Registration\R000000000006.clb
3820    Rick And Morty  0xf8a0025d2fc0  0x148   Section 0xf0005
3820    Rick And Morty  0xfa801b45ecd0  0x14c   File    0x100020        \Device\HarddiskVolume1\Windows\winsxs\x86_microsoft.windows.common-controls_6595b64144ccf1df_6.0.7601.17514_none_41e6975e2bd6f2b2
3820    Rick And Morty  0xf8a00641b220  0x150   Key     0xf003f USER\S-1-5-21-1923827501-2510115606-422599235-1000_CLASSES
3820    Rick And Morty  0xfa801abdeb30  0x154   EtwRegistration 0x804
3820    Rick And Morty  0xfa801b21adf0  0x158   Event   0x1f0003
3820    Rick And Morty  0xfa801acf3d80  0x15c   Event   0x1f0003
3820    Rick And Morty  0xfa801b579e80  0x160   Event   0x1f0003
3820    Rick And Morty  0xfa801aadd7f0  0x164   EtwRegistration 0x804
3820    Rick And Morty  0xfa801b565e30  0x168   EtwRegistration 0x804
3820    Rick And Morty  0xfa801aa11460  0x16c   Mutant  0x1f0001
3820    Rick And Morty  0xf8a0022a24a0  0x170   Section 0x6     windows_shell_global_counters
3820    Rick And Morty  0xfa801b3fa2d0  0x174   EtwRegistration 0x804
3820    Rick And Morty  0xfa801b5f9070  0x178   File    0x100020        \Device\HarddiskVolume1\Users\Rick\AppData\Local\Temp\RarSFX0
3820    Rick And Morty  0xf8a00643d060  0x17c   Key     0x1     USER\S-1-5-21-1923827501-2510115606-422599235-1000\SOFTWARE\MICROSOFT\WINDOWS\CURRENTVERSION\EXPLORER
3820    Rick And Morty  0xf8a00236e950  0x180   Section 0x4     C:*ProgramData*Microsoft*Windows*Caches*cversions.2.ro
3820    Rick And Morty  0xf8a00642b060  0x184   Key     0x20019 USER\S-1-5-21-1923827501-2510115606-422599235-1000\SOFTWARE\MICROSOFT\WINDOWS\CURRENTVERSION\EXPLORER\FILEEXTS
3820    Rick And Morty  0xf8a0016f8d30  0x188   Section 0x6     windows_shell_global_counters
3820    Rick And Morty  0xf8a001aa3890  0x18c   Key     0x20019 MACHINE\SOFTWARE\WOW6432NODE\MICROSOFT\WINDOWS\CURRENTVERSION\EXPLORER\FOLDERDESCRIPTIONS\{B4BFCC3A-DB2C-424C-B029-7FE99A87C641}\PROPERTYBAG
3820    Rick And Morty  0xfa801b0d11c0  0x190   EtwRegistration 0x804
3820    Rick And Morty  0xfa801aa633e0  0x194   Event   0x1f0003
3820    Rick And Morty  0xfa801b0c6890  0x198   Semaphore       0x100003
3820    Rick And Morty  0xfa801b567c80  0x19c   Semaphore       0x100003
3820    Rick And Morty  0xfa801a7e5810  0x1a0   Semaphore       0x100003
3820    Rick And Morty  0xfa801a7a7e70  0x1a4   Semaphore       0x100003
3820    Rick And Morty  0xfa801a57f770  0x1a8   Semaphore       0x100003
3820    Rick And Morty  0xfa801a54d120  0x1ac   Semaphore       0x100003
3820    Rick And Morty  0xfa801af5ad20  0x1b0   Semaphore       0x100003
3820    Rick And Morty  0xfa801ac7eed0  0x1b4   Semaphore       0x100003
3820    Rick And Morty  0xf8a002371d40  0x1b8   Section 0x4     C:*ProgramData*Microsoft*Windows*Caches*{6AF0698E-D558-4F6E-9B3C-3716689AF493}.2.ver0x000000000000000a.db
3820    Rick And Morty  0xf8a0033609a0  0x1bc   Key     0x20019 MACHINE\SOFTWARE\WOW6432NODE\MICROSOFT\WINDOWS\CURRENTVERSION\EXPLORER\FOLDERDESCRIPTIONS\{F3CE0F7C-4901-4ACC-8648-D5D44B04EF8F}\PROPERTYBAG
3820    Rick And Morty  0xf8a00236e950  0x1c0   Section 0x4     C:*ProgramData*Microsoft*Windows*Caches*cversions.2.ro
3820    Rick And Morty  0xf8a00235dfc0  0x1c4   Section 0x4     C:*ProgramData*Microsoft*Windows*Caches*{DDF571F2-BE98-426D-8288-1A9A39C3FDA2}.2.ver0x0000000000000002.db
3820    Rick And Morty  0xf8a001919060  0x1c8   Key     0x20019 MACHINE\SOFTWARE\WOW6432NODE\MICROSOFT\WINDOWS\CURRENTVERSION\EXPLORER\FOLDERDESCRIPTIONS\{F38BF404-1D43-42F2-9305-67DE0B28FC23}\PROPERTYBAG
3820    Rick And Morty  0xf8a002751fa0  0x1cc   Key     0x20019 MACHINE\SOFTWARE\WOW6432NODE\MICROSOFT\WINDOWS\CURRENTVERSION\EXPLORER\FOLDERDESCRIPTIONS\{18989B1D-99B5-455B-841C-AB7C74E4DDFC}\PROPERTYBAG
3820    Rick And Morty  0xf8a002dff8b0  0x1d0   Key     0x20019 MACHINE\SOFTWARE\WOW6432NODE\MICROSOFT\WINDOWS\CURRENTVERSION\EXPLORER\FOLDERDESCRIPTIONS\{2112AB0A-C86A-4FFE-A368-0DE96E47012E}\PROPERTYBAG
3820    Rick And Morty  0xf8a0062a2e90  0x1d4   Key     0x20019 MACHINE\SOFTWARE\WOW6432NODE\MICROSOFT\WINDOWS\CURRENTVERSION\EXPLORER\FOLDERDESCRIPTIONS\{491E922F-5643-4AF4-A7EB-4E7A138D8174}\PROPERTYBAG
3820    Rick And Morty  0xf8a006332a60  0x1d8   Key     0x20019 MACHINE\SOFTWARE\WOW6432NODE\MICROSOFT\WINDOWS\CURRENTVERSION\EXPLORER\FOLDERDESCRIPTIONS\{33E28130-4E1E-4676-835A-98395C3BC3BB}\PROPERTYBAG
3820    Rick And Morty  0xf8a0028898d0  0x1dc   Key     0x20019 MACHINE\SOFTWARE\WOW6432NODE\MICROSOFT\WINDOWS\CURRENTVERSION\EXPLORER\FOLDERDESCRIPTIONS\{1AC14E77-02E7-4E5D-B744-2EB1AE5198B7}\PROPERTYBAG
3820    Rick And Morty  0xf8a0018e9930  0x1e0   Key     0x20019 MACHINE\SOFTWARE\WOW6432NODE\MICROSOFT\WINDOWS\CURRENTVERSION\EXPLORER\FOLDERDESCRIPTIONS\{2400183A-6185-49FB-A2D8-4A392A602BA3}\PROPERTYBAG
3820    Rick And Morty  0xf8a003337ed0  0x1e4   Key     0x20019 MACHINE\SOFTWARE\WOW6432NODE\MICROSOFT\WINDOWS\CURRENTVERSION\EXPLORER\FOLDERDESCRIPTIONS\{56784854-C6CB-462B-8169-88E350ACB882}\PROPERTYBAG
3820    Rick And Morty  0xf8a00288dd50  0x1e8   Key     0x20019 MACHINE\SOFTWARE\WOW6432NODE\MICROSOFT\WINDOWS\CURRENTVERSION\EXPLORER\FOLDERDESCRIPTIONS\{A302545D-DEFF-464B-ABE8-61C8648D939B}\PROPERTYBAG
3820    Rick And Morty  0xf8a001fb8df0  0x1ec   Key     0x20019 MACHINE\SOFTWARE\WOW6432NODE\MICROSOFT\WINDOWS\CURRENTVERSION\EXPLORER\FOLDERDESCRIPTIONS\{52528A6B-B9E3-4ADD-B60D-588C2DBA842D}\PROPERTYBAG
3820    Rick And Morty  0xf8a0019c9570  0x1f0   Key     0x20019 MACHINE\SOFTWARE\WOW6432NODE\MICROSOFT\WINDOWS\CURRENTVERSION\EXPLORER\FOLDERDESCRIPTIONS\{4BD8D571-6D19-48D3-BE97-422220080E43}\PROPERTYBAG
3820    Rick And Morty  0xf8a0037ae4d0  0x1f4   Key     0x20019 MACHINE\SOFTWARE\WOW6432NODE\MICROSOFT\WINDOWS\CURRENTVERSION\EXPLORER\FOLDERDESCRIPTIONS\{D65231B0-B2F1-4857-A4CE-A8E7C6EA7D27}\PROPERTYBAG
3820    Rick And Morty  0xf8a0020025c0  0x1f8   Key     0x20019 MACHINE\SOFTWARE\WOW6432NODE\MICROSOFT\WINDOWS\CURRENTVERSION\EXPLORER\FOLDERDESCRIPTIONS\{7B0DB17D-9CD2-4A93-9733-46CC89022E7C}\PROPERTYBAG
3820    Rick And Morty  0xf8a005f53bc0  0x1fc   Key     0x20019 MACHINE\SOFTWARE\WOW6432NODE\MICROSOFT\WINDOWS\CURRENTVERSION\EXPLORER\FOLDERDESCRIPTIONS\{B6EBFB86-6907-413C-9AF7-4FC2ABF07CC5}\PROPERTYBAG
3820    Rick And Morty  0xf8a005e12820  0x200   Key     0x20019 MACHINE\SOFTWARE\WOW6432NODE\MICROSOFT\WINDOWS\CURRENTVERSION\EXPLORER\FOLDERDESCRIPTIONS\{A990AE9F-A03B-4E80-94BC-9912D7504104}\PROPERTYBAG
3820    Rick And Morty  0xf8a0026e0510  0x204   Key     0x20019 MACHINE\SOFTWARE\WOW6432NODE\MICROSOFT\WINDOWS\CURRENTVERSION\EXPLORER\FOLDERDESCRIPTIONS\{ED4824AF-DCE4-45A8-81E2-FC7965083634}\PROPERTYBAG
3820    Rick And Morty  0xf8a006439e20  0x208   Key     0x20019 MACHINE\SOFTWARE\WOW6432NODE\MICROSOFT\WINDOWS\CURRENTVERSION\EXPLORER\FOLDERDESCRIPTIONS\{905E63B6-C1BF-494E-B29C-65B732D3D21A}\PROPERTYBAG
3820    Rick And Morty  0xf8a001b73cd0  0x20c   Key     0x20019 MACHINE\SOFTWARE\WOW6432NODE\MICROSOFT\WINDOWS\CURRENTVERSION\EXPLORER\FOLDERDESCRIPTIONS\{3214FAB5-9757-4298-BB61-92A9DEAA44FF}\PROPERTYBAG
3820    Rick And Morty  0xf8a002cb33b0  0x210   Key     0x20019 MACHINE\SOFTWARE\WOW6432NODE\MICROSOFT\WINDOWS\CURRENTVERSION\EXPLORER\FOLDERDESCRIPTIONS\{FD228CB7-AE11-4AE3-864C-16F3910AB8FE}\PROPERTYBAG
3820    Rick And Morty  0xf8a0037ab650  0x214   Key     0x20019 MACHINE\SOFTWARE\WOW6432NODE\MICROSOFT\WINDOWS\CURRENTVERSION\EXPLORER\FOLDERDESCRIPTIONS\{7C5A40EF-A0FB-4BFC-874A-C0F2E0B9FA8E}\PROPERTYBAG
3820    Rick And Morty  0xf8a006633b90  0x218   Key     0x20019 MACHINE\SOFTWARE\WOW6432NODE\MICROSOFT\WINDOWS\CURRENTVERSION\EXPLORER\FOLDERDESCRIPTIONS\{FDD39AD0-238F-46AF-ADB4-6C85480369C7}\PROPERTYBAG
3820    Rick And Morty  0xfa801a5f8270  0x21c   IoCompletion    0x1f0003
3820    Rick And Morty  0xfa801a551630  0x220   TpWorkerFactory 0xf00ff
3820    Rick And Morty  0xfa801a551630  0x224   TpWorkerFactory 0xf00ff
3820    Rick And Morty  0xfa801982a590  0x22c   File    0x120089        \Device\HarddiskVolume1\Windows\SysWOW64\en-US\propsys.dll.mui
3820    Rick And Morty  0xf8a002cb34e0  0x230   Key     0x20019 MACHINE\SOFTWARE\WOW6432NODE\MICROSOFT\INTERNET EXPLORER\MAIN\FEATURECONTROL\FEATURE_UNC_SAVEDFILECHECK
3820    Rick And Morty  0xfa801a783b60  0x234   Thread  0x1fffff        Tid 3136 Pid 3820
3820    Rick And Morty  0xfa801b465430  0x238   Event   0x1f0003
3820    Rick And Morty  0xfa801b2c5db0  0x240   Mutant  0x1f0001        ZonesCounterMutex
3820    Rick And Morty  0xfa801ae96070  0x244   EtwRegistration 0x804
3820    Rick And Morty  0xf8a006426800  0x248   Key     0x20019 USER\S-1-5-21-1923827501-2510115606-422599235-1000\SOFTWARE\POLICIES
3820    Rick And Morty  0xf8a0025d5ee0  0x24c   Key     0x20019 MACHINE\SOFTWARE\POLICIES
3820    Rick And Morty  0xf8a0062c7230  0x250   Key     0x20019 USER\S-1-5-21-1923827501-2510115606-422599235-1000\SOFTWARE
3820    Rick And Morty  0xf8a0063378e0  0x254   Key     0x20019 MACHINE\SOFTWARE\WOW6432NODE
3820    Rick And Morty  0xfa801a7b3dc0  0x258   File    0x120089        \Device\HarddiskVolume1\Windows\SysWOW64\en-US\setupapi.dll.mui
3820    Rick And Morty  0xfa801a56c250  0x25c   Event   0x1f0003
3820    Rick And Morty  0xfa801b2c6f40  0x260   Mutant  0x100001        !IETld!Mutex
3820    Rick And Morty  0xfa801aadc060  0x264   Thread  0x1fffff        Tid 2564 Pid 3820
3820    Rick And Morty  0xf8a001589a00  0x26c   KeyedEvent      0xf0003
3820    Rick And Morty  0xfa801a7fa360  0x270   Timer   0x100002
3820    Rick And Morty  0xfa801a52c060  0x274   Timer   0x1f0003
3820    Rick And Morty  0xfa801a554b60  0x278   Thread  0x1fffff        Tid 2648 Pid 3820
3820    Rick And Morty  0xfa801a554b60  0x27c   Thread  0x1fffff        Tid 2648 Pid 3820
3820    Rick And Morty  0xfa801ae47320  0x280   Timer   0x100002
3820    Rick And Morty  0xf8a00337e650  0x284   Key     0x20019 USER\S-1-5-21-1923827501-2510115606-422599235-1000\SOFTWARE\MICROSOFT\INTERNET EXPLORER\IETLD
3820    Rick And Morty  0xfa801b380f20  0x288   File    0x120089        \Device\HarddiskVolume1\Windows\SysWOW64\en-US\urlmon.dll.mui
3820    Rick And Morty  0xf8a0027435f0  0x28c   Key     0x20019 USER\S-1-5-21-1923827501-2510115606-422599235-1000\SOFTWARE\POLICIES\MICROSOFT\WINDOWS\CURRENTVERSION\INTERNET SETTINGS
3820    Rick And Morty  0xf8a006436130  0x290   Key     0x20019 MACHINE\SOFTWARE\POLICIES\MICROSOFT\WINDOWS\CURRENTVERSION\INTERNET SETTINGS
3820    Rick And Morty  0xf8a0037b15f0  0x294   Key     0x20019 USER\S-1-5-21-1923827501-2510115606-422599235-1000\SOFTWARE\MICROSOFT\WINDOWS\CURRENTVERSION\INTERNET SETTINGS
3820    Rick And Morty  0xf8a001a8c060  0x298   Key     0x20019 MACHINE\SOFTWARE\WOW6432NODE\MICROSOFT\WINDOWS\CURRENTVERSION\INTERNET SETTINGS
3820    Rick And Morty  0xf8a003785550  0x29c   Key     0x20019 MACHINE\SOFTWARE\WOW6432NODE\MICROSOFT\INTERNET EXPLORER\MAIN\FEATURECONTROL\FEATURE_HTTP_USERNAME_PASSWORD_DISABLE
3820    Rick And Morty  0xf8a0023bcc40  0x2a0   Section 0xf0007 UrlZonesSM_Rick
3820    Rick And Morty  0xfa801aa9e4c0  0x2a4   ALPC Port       0x1f0001
3820    Rick And Morty  0xfa801b2c6100  0x2a8   Mutant  0x1f0001        ZoneAttributeCacheCounterMutex
3820    Rick And Morty  0xf8a0037b1530  0x2ac   Key     0x20019 MACHINE\SOFTWARE\WOW6432NODE\MICROSOFT\INTERNET EXPLORER\MAIN\FEATURECONTROL\FEATURE_LOCALMACHINE_LOCKDOWN
3820    Rick And Morty  0xfa801b2c6540  0x2b0   Mutant  0x1f0001        ZonesCacheCounterMutex
3820    Rick And Morty  0xfa801b2c6100  0x2b4   Mutant  0x1f0001        ZoneAttributeCacheCounterMutex
3820    Rick And Morty  0xfa801b66b5c0  0x2b8   Event   0x1f0003
3820    Rick And Morty  0xfa801b2c1080  0x2bc   Mutant  0x1f0001        ZonesLockedCacheCounterMutex
3820    Rick And Morty  0xf8a002747d30  0x2c0   Key     0x20019 MACHINE\SOFTWARE\WOW6432NODE\MICROSOFT\INTERNET EXPLORER\MAIN\FEATURECONTROL\FEATURE_PROTOCOL_LOCKDOWN
3820    Rick And Morty  0xfa8019166990  0x2c4   EtwRegistration 0x804
3820    Rick And Morty  0xfa801a7bfa70  0x2c8   Mutant  0x1f0001
3820    Rick And Morty  0xfa801af5c180  0x2cc   Event   0x1f0003
3820    Rick And Morty  0xfa801a7a80f0  0x2d0   Mutant  0x1f0001
3820    Rick And Morty  0xfa801a6cbde0  0x2dc   ALPC Port       0x1f0001
3820    Rick And Morty  0xfa801a4c5b30  0x2e0   Process 0x121101        vmware-tray.ex Pid 3720
3820    Rick And Morty  0xfa801a7d7720  0x2e4   Thread  0x1fffff        Tid 3756 Pid 3820
3820    Rick And Morty  0xfa801b1c4430  0x2e8   ALPC Port       0x1f0001
3820    Rick And Morty  0xfa80198533a0  0x2ec   Event   0x1f0003
3820    Rick And Morty  0xf8a002252260  0x2f0   Key     0x8     USER\S-1-5-21-1923827501-2510115606-422599235-1000\SOFTWARE\MICROSOFT\WINDOWS NT\CURRENTVERSION
3820    Rick And Morty  0xf8a002286bc0  0x2f4   Key     0x8     MACHINE\SOFTWARE\WOW6432NODE\MICROSOFT\WINDOWS NT\CURRENTVERSION\APPCOMPATFLAGS
3820    Rick And Morty  0xfa801b547340  0x2f8   ALPC Port       0x1f0001
```

# 測試內容
- .\vol.exe -f .\OtterCTF.vmem windows.handles.Handles --pid 3720
Volatility 3 Framework 2.5.0
```
D:\Forensic\G140A006\VolatilityWorkbench>.\vol.exe -f .\OtterCTF.vmem windows.handles.Handles --pid 3720
Volatility 3 Framework 2.5.0
Progress:  100.00               PDB scanning finished
PID     Process Offset  HandleValue     Type    GrantedAccess   Name

3720    vmware-tray.ex  0xf8a006600880  0x4     Key     0x9     MACHINE\SOFTWARE\MICROSOFT\WINDOWS NT\CURRENTVERSION\IMAGE FILE EXECUTION OPTIONS
3720    vmware-tray.ex  0xf8a000566af0  0x8     Directory       0x3     KnownDlls
3720    vmware-tray.ex  0xf8a0038d5990  0xc     Directory       0x3     KnownDlls32
3720    vmware-tray.ex  0xfa801b4654c0  0x10    File    0x100020        \Device\HarddiskVolume1\Windows
3720    vmware-tray.ex  0xf8a00221a930  0x14    Key     0x9     MACHINE\SOFTWARE\MICROSOFT\WINDOWS NT\CURRENTVERSION\IMAGE FILE EXECUTION OPTIONS
3720    vmware-tray.ex  0xf8a0038d5990  0x18    Directory       0x3     KnownDlls32
3720    vmware-tray.ex  0xfa801b301070  0x1c    File    0x100020        \Device\HarddiskVolume1\Users\Rick\AppData\Local\Temp\RarSFX0
3720    vmware-tray.ex  0xf8a00335e530  0x20    Key     0x20019 MACHINE\SYSTEM\CONTROLSET001\CONTROL\NLS\SORTING\VERSIONS
3720    vmware-tray.ex  0xfa801b5028e0  0x24    Mutant  0x1f0001
3720    vmware-tray.ex  0xfa801ac437d0  0x28    ALPC Port       0x1f0001
3720    vmware-tray.ex  0xf8a00377a060  0x2c    Key     0x1     MACHINE\SYSTEM\CONTROLSET001\CONTROL\SESSION MANAGER
3720    vmware-tray.ex  0xfa801aab7850  0x30    Semaphore       0x100003
3720    vmware-tray.ex  0xfa801b3bc730  0x34    Semaphore       0x100003
3720    vmware-tray.ex  0xfa801a6b35a0  0x38    Mutant  0x1f0001
3720    vmware-tray.ex  0xf8a003352f60  0x3c    Key     0xf003f MACHINE
3720    vmware-tray.ex  0xfa801b067560  0x40    Event   0x1f0003
3720    vmware-tray.ex  0xfa801ac9ee90  0x44    Mutant  0x1f0001
3720    vmware-tray.ex  0xfa801b5dfef0  0x48    EtwRegistration 0x804
3720    vmware-tray.ex  0xfa801b3d7b60  0x4c    Event   0x21f0003
3720    vmware-tray.ex  0xfa801ab08cc0  0x50    WindowStation   0xf037f WinSta0
3720    vmware-tray.ex  0xfa801aaeaeb0  0x54    Desktop 0xf01ff Default
3720    vmware-tray.ex  0xfa801ab08cc0  0x58    WindowStation   0xf037f WinSta0
3720    vmware-tray.ex  0xfa801b41a5b0  0x5c    EtwRegistration 0x804
3720    vmware-tray.ex  0xfa801b19b860  0x60    EtwRegistration 0x804
3720    vmware-tray.ex  0xf8a0028fe5e0  0x64    Key     0xf003f USER\S-1-5-21-1923827501-2510115606-422599235-1000
3720    vmware-tray.ex  0xf8a00377a630  0x68    Key     0x20019 MACHINE\SOFTWARE\WOW6432NODE\MICROSOFT\.NETFRAMEWORK
3720    vmware-tray.ex  0xfa801b109b30  0x6c    Event   0x1f0003
3720    vmware-tray.ex  0xfa801a7a53b0  0x70    Event   0x1f0003
3720    vmware-tray.ex  0xfa801b2c1300  0x74    Event   0x1f0003
3720    vmware-tray.ex  0xfa801b18a600  0x78    EtwRegistration 0x804
3720    vmware-tray.ex  0xfa801af0caa0  0x7c    EtwRegistration 0x804
3720    vmware-tray.ex  0xfa801a40eab0  0x80    EtwRegistration 0x804
3720    vmware-tray.ex  0xfa801a42a6c0  0x84    EtwRegistration 0x804
3720    vmware-tray.ex  0xf8a0015481c0  0x88    Directory       0xf     BaseNamedObjects
3720    vmware-tray.ex  0xf8a006466af0  0x8c    Section 0xf0007 Cor_SxSPublic_IPCBlock
3720    vmware-tray.ex  0xf8a003770700  0x90    Section 0xf0007 Cor_Private_IPCBlock_v4_3720
3720    vmware-tray.ex  0xf8a00299f7f0  0x94    Directory       0xf000f
3720    vmware-tray.ex  0xfa801a5d8160  0x98    Event   0x1f0003
3720    vmware-tray.ex  0xfa801a2f2f60  0x9c    Event   0x1f0003
3720    vmware-tray.ex  0xfa801ab94980  0xa0    Mutant  0x1f0001
3720    vmware-tray.ex  0xfa801a7074b0  0xa4    Event   0x1f0003
3720    vmware-tray.ex  0xfa801b20ae90  0xa8    Event   0x1f0003
3720    vmware-tray.ex  0xfa801adc2c70  0xac    Event   0x1f0003
3720    vmware-tray.ex  0xfa801ae234c0  0xb0    Event   0x1f0003
3720    vmware-tray.ex  0xfa801b1f6dd0  0xb4    Event   0x1f0003
3720    vmware-tray.ex  0xfa801b0d4ac0  0xb8    Event   0x1f0003
3720    vmware-tray.ex  0xfa801aa0adf0  0xbc    Event   0x1f0003
3720    vmware-tray.ex  0xfa801b213b30  0xc0    Event   0x1f0003
3720    vmware-tray.ex  0xfa801a590f60  0xc4    Event   0x1f0003
3720    vmware-tray.ex  0xfa801b1fb500  0xc8    Mutant  0x1f0001
3720    vmware-tray.ex  0xfa801a48eb60  0xcc    Thread  0x1fffff        Tid 1664 Pid 3720
3720    vmware-tray.ex  0xfa801aca9b60  0xd0    Thread  0x1fffff        Tid 3708 Pid 3720
3720    vmware-tray.ex  0xfa801b593840  0xd4    Event   0x1f0003
3720    vmware-tray.ex  0xfa801b264b30  0xd8    Event   0x1f0003
3720    vmware-tray.ex  0xfa801b19c900  0xdc    Event   0x1f0003
3720    vmware-tray.ex  0xfa801ac30730  0xe0    Event   0x1f0003
3720    vmware-tray.ex  0xfa801a690d00  0xe4    Event   0x1f0003
3720    vmware-tray.ex  0xfa8018de93d0  0xe8    Event   0x100001        LowMemoryCondition
3720    vmware-tray.ex  0xfa801a39a060  0xec    Event   0x1f0003
3720    vmware-tray.ex  0xfa801b547810  0xf0    Event   0x1f0003
3720    vmware-tray.ex  0xfa801b3db510  0xf4    Event   0x1f0003
3720    vmware-tray.ex  0xfa801a60e390  0xf8    Event   0x1f0003
3720    vmware-tray.ex  0xfa801a520da0  0xfc    Event   0x1f0003
3720    vmware-tray.ex  0xfa801a646990  0x100   Event   0x1f0003
3720    vmware-tray.ex  0xfa801a5868a0  0x104   Event   0x1f0003
3720    vmware-tray.ex  0xfa801ac287c0  0x108   Event   0x1f0003
3720    vmware-tray.ex  0xfa801b1ce6d0  0x10c   Event   0x1f0003
3720    vmware-tray.ex  0xfa801b22db40  0x110   Event   0x1f0003
3720    vmware-tray.ex  0xfa801b27c060  0x114   Thread  0x1fffff        Tid 1280 Pid 3720
3720    vmware-tray.ex  0xfa801b5a85d0  0x118   Event   0x1f0003
3720    vmware-tray.ex  0xfa801b054440  0x11c   Event   0x1f0003
3720    vmware-tray.ex  0xfa801acf14f0  0x120   Event   0x1f0003
3720    vmware-tray.ex  0xfa801a499e70  0x124   EtwRegistration 0x804
3720    vmware-tray.ex  0xfa801b0185f0  0x128   EtwRegistration 0x804
3720    vmware-tray.ex  0xfa801abf2fe0  0x12c   Event   0x1f0003
3720    vmware-tray.ex  0xfa801b27c060  0x130   Thread  0x1fffff        Tid 1280 Pid 3720
3720    vmware-tray.ex  0xfa801ae68370  0x138   IoCompletion    0x1f0003
3720    vmware-tray.ex  0xfa801b495370  0x13c   TpWorkerFactory 0xf00ff
3720    vmware-tray.ex  0xfa801b495370  0x140   TpWorkerFactory 0xf00ff
3720    vmware-tray.ex  0xf8a001add5b0  0x144   KeyedEvent      0xf0003
3720    vmware-tray.ex  0xfa801a6d9060  0x148   Timer   0x100002
3720    vmware-tray.ex  0xfa801a40e840  0x14c   Timer   0x1f0003
3720    vmware-tray.ex  0xfa801ab07b60  0x150   Thread  0x1fffff        Tid 1276 Pid 3720
3720    vmware-tray.ex  0xfa801ab07b60  0x154   Thread  0x1fffff        Tid 1276 Pid 3720
3720    vmware-tray.ex  0xfa801ac806c0  0x158   IoCompletion    0x1f0003
3720    vmware-tray.ex  0xfa801b3f8060  0x15c   TpWorkerFactory 0xf00ff
3720    vmware-tray.ex  0xfa801b3f8060  0x160   TpWorkerFactory 0xf00ff
3720    vmware-tray.ex  0xfa801b583220  0x164   Timer   0x100002
3720    vmware-tray.ex  0xfa801a7d03e0  0x168   Event   0x1f0003        CPFATE_3720_v4.0.30319
3720    vmware-tray.ex  0xf8a002011910  0x16c   Key     0x20019 MACHINE\SOFTWARE\MICROSOFT\FUSION\GACCHANGENOTIFICATION\DEFAULT
3720    vmware-tray.ex  0xfa801b207640  0x170   Event   0x1f0003
3720    vmware-tray.ex  0xfa801b668070  0x174   EtwRegistration 0x804
3720    vmware-tray.ex  0xfa801a717650  0x178   Event   0x1f0003
3720    vmware-tray.ex  0xfa801a6c3060  0x17c   Event   0x1f0003
3720    vmware-tray.ex  0xfa801a7821c0  0x180   Event   0x1f0003
3720    vmware-tray.ex  0xfa801aadb3a0  0x184   Event   0x1f0003
3720    vmware-tray.ex  0xfa801b1f0620  0x188   Event   0x1f0003
3720    vmware-tray.ex  0xfa801a571ba0  0x18c   Event   0x1f0003
3720    vmware-tray.ex  0xfa801aa7e9b0  0x190   Event   0x1f0003
3720    vmware-tray.ex  0xfa801b1dae40  0x194   File    0x100001        \Device\KsecDD
3720    vmware-tray.ex  0xfa801ae90760  0x198   EtwRegistration 0x804
3720    vmware-tray.ex  0xfa801a5f8c00  0x19c   EtwRegistration 0x804
3720    vmware-tray.ex  0xfa801a3d6e60  0x1a0   ALPC Port       0x1f0001
3720    vmware-tray.ex  0xf8a0018403b0  0x1a4   Section 0x4
3720    vmware-tray.ex  0xfa801ae7a1a0  0x1a8   Event   0x1f0003
3720    vmware-tray.ex  0xfa801afea6e0  0x1ac   Event   0x1f0003
3720    vmware-tray.ex  0xfa801a5b1aa0  0x1b0   Event   0x1f0003
3720    vmware-tray.ex  0xf8a001eaba00  0x1b4   Key     0x20019 MACHINE\SOFTWARE\MICROSOFT\FUSION\NATIVEIMAGESINDEX\V4.0.30319_32
3720    vmware-tray.ex  0xfa801afe57a0  0x1b8   File    0x120089        \Device\HarddiskVolume1\Windows\assembly\NativeImages_v4.0.30319_32\index18.dat
3720    vmware-tray.ex  0xf8a005fcb880  0x1bc   Key     0x20019 MACHINE\SOFTWARE\MICROSOFT\FUSION\PUBLISHERPOLICY\DEFAULT
3720    vmware-tray.ex  0xfa801b1f0070  0x1c0   File    0x120089        \Device\HarddiskVolume1\Windows\assembly\pubpol4.dat
3720    vmware-tray.ex  0xf8a001663a40  0x1c4   Key     0x1     MACHINE\SYSTEM\CONTROLSET001\CONTROL\NLS\CUSTOMLOCALE
3720    vmware-tray.ex  0xfa801aca9b60  0x1c8   Thread  0x1fffff        Tid 3708 Pid 3720
3720    vmware-tray.ex  0xfa801a449ad0  0x1cc   Event   0x1f0003
3720    vmware-tray.ex  0xfa801b1137c0  0x1d0   ALPC Port       0x1f0001
3720    vmware-tray.ex  0xfa801a610420  0x1d4   File    0x100020        \Device\HarddiskVolume1\Windows\winsxs\x86_microsoft.windows.common-controls_6595b64144ccf1df_5.82.7601.17514_none_ec83dffa859149af
3720    vmware-tray.ex  0xfa801aca9b60  0x1d8   Thread  0x1fffff        Tid 3708 Pid 3720
3720    vmware-tray.ex  0xfa801b460320  0x1dc   File    0x100020        \Device\HarddiskVolume1\Windows\winsxs\x86_microsoft.windows.common-controls_6595b64144ccf1df_6.0.7601.17514_none_41e6975e2bd6f2b2
3720    vmware-tray.ex  0xfa801a38a6f0  0x1e0   EtwRegistration 0x804
3720    vmware-tray.ex  0xfa801b48aa00  0x1e4   EtwRegistration 0x804
3720    vmware-tray.ex  0xf8a003765fa0  0x1e8   Key     0x20019 MACHINE\SYSTEM\CONTROLSET001\CONTROL\NLS\LOCALE\ALTERNATE SORTS
3720    vmware-tray.ex  0xf8a002ab95b0  0x1ec   Key     0x20019 MACHINE\SYSTEM\CONTROLSET001\CONTROL\NLS\LOCALE
3720    vmware-tray.ex  0xf8a00379a3e0  0x1f0   Key     0x20019 MACHINE\SYSTEM\CONTROLSET001\CONTROL\NLS\LANGUAGE GROUPS
3720    vmware-tray.ex  0xfa801ae53d10  0x1f4   EtwRegistration 0x804
3720    vmware-tray.ex  0xfa801b40f400  0x1f8   File    0x100020        \Device\HarddiskVolume1\Windows\winsxs\x86_microsoft.windows.gdiplus_6595b64144ccf1df_1.1.7601.17514_none_72d18a4386696c80
3720    vmware-tray.ex  0xfa801b3beee0  0x1fc   Event   0x1f0003
3720    vmware-tray.ex  0xfa80198bab60  0x200   Thread  0x1fffff        Tid 3548 Pid 3720
3720    vmware-tray.ex  0xfa801b2b2260  0x204   Event   0x21f0003
3720    vmware-tray.ex  0xf8a002dffa10  0x208   Key     0xf003f USER\S-1-5-21-1923827501-2510115606-422599235-1000_CLASSES
3720    vmware-tray.ex  0xfa801a2f4a80  0x20c   File    0x120089        \Device\HarddiskVolume1\Windows\Fonts\StaticCache.dat
3720    vmware-tray.ex  0xf8a0003f7cd0  0x210   Section 0xf0005
3720    vmware-tray.ex  0xfa801b068880  0x214   EtwRegistration 0x804
3720    vmware-tray.ex  0xfa801a79d3b0  0x218   EtwRegistration 0x804
3720    vmware-tray.ex  0xfa801a598eb0  0x21c   EtwRegistration 0x804
3720    vmware-tray.ex  0xfa801a5b54c0  0x220   EtwRegistration 0x804
3720    vmware-tray.ex  0xfa801a5ea8c0  0x224   EtwRegistration 0x804
3720    vmware-tray.ex  0xfa801a2f0d50  0x228   EtwRegistration 0x804
3720    vmware-tray.ex  0xfa801a5f8b20  0x22c   EtwRegistration 0x804
3720    vmware-tray.ex  0xf8a0022a24a0  0x230   Section 0x6     windows_shell_global_counters
3720    vmware-tray.ex  0xfa801a450790  0x234   Semaphore       0x100003
3720    vmware-tray.ex  0xf8a003358af0  0x238   Key     0x1     USER\S-1-5-21-1923827501-2510115606-422599235-1000\SOFTWARE\MICROSOFT\WINDOWS\CURRENTVERSION\EXPLORER
3720    vmware-tray.ex  0xfa801ab13a30  0x23c   EtwRegistration 0x804
3720    vmware-tray.ex  0xfa801abb4560  0x240   Semaphore       0x100003
3720    vmware-tray.ex  0xfa801a4dc720  0x244   Event   0x1f0003
3720    vmware-tray.ex  0xfa801a613dc0  0x248   File    0x100003        \Device\KsecDD
3720    vmware-tray.ex  0xfa801b5c2750  0x250   Event   0x1f0003
3720    vmware-tray.ex  0xfa801b47e060  0x254   Thread  0x1fffff        Tid 2112 Pid 3720

```

# windows.handles.Handles 分析

## 1. Plugin 功能說明

`windows.handles.Handles` 用來列出指定 Process 所開啟的 Handle。

Handle 是 Process 存取系統物件的參考，例如：

```text
File
Registry Key
Mutant
Section
Event
Thread
Process
ALPC Port
Semaphore
```

在數位鑑識中，`Handles` 可以用來觀察可疑 Process 是否正在存取特定檔案、暫存目錄、登錄機碼、子行程或同步物件。

本案針對兩個可疑行程進行分析：

```text
PID 3820：Rick And Morty
PID 3720：vmware-tray.ex
```

---

## 2. 執行指令

```bash
.\vol.exe -f .\OtterCTF.vmem windows.handles.Handles --pid 3820
```

```bash
.\vol.exe -f .\OtterCTF.vmem windows.handles.Handles --pid 3720
```

---

## 3. 欄位說明

| 欄位              | 說明                     |
| --------------- | ---------------------- |
| `PID`           | Process ID             |
| `Process`       | Process 名稱             |
| `Offset`        | Handle Object 在記憶體中的位置 |
| `HandleValue`   | Handle 數值              |
| `Type`          | Handle 類型              |
| `GrantedAccess` | 權限                     |
| `Name`          | Handle 指向的物件名稱         |

---

## 4. PID 3820：Rick And Morty 分析

PID 3820 `Rick And Morty` 的 Handles 中，出現許多一般 Windows Process 常見的物件，例如：

```text
KnownDlls
KnownDlls32
Windows
SysWOW64
WinSta0
Default
Registry Key
Event
Semaphore
ALPC Port
```

其中最重要的發現有兩項。

### 4.1 開啟 RarSFX0 暫存目錄

PID 3820 有開啟以下 File handle：

```text
\Device\HarddiskVolume1\Users\Rick\AppData\Local\Temp\RarSFX0
```

此結果表示 `Rick And Morty` Process 與 `RarSFX0` 暫存目錄存在關聯。

`RarSFX0` 常見於 WinRAR SFX 自解壓程式執行時產生的暫存目錄。前面分析中，PID 3720 `vmware-tray.exe` 的路徑正是：

```text
C:\Users\Rick\AppData\Local\Temp\RarSFX0\vmware-tray.exe
```

因此，此 Handle 結果支持 `Rick And Morty` 可能解壓或啟動了位於 RarSFX 暫存目錄中的 `vmware-tray.exe`。

### 4.2 持有 vmware-tray.exe 的 Process Handle

PID 3820 也出現以下 Process handle：

```text
Process    vmware-tray.ex Pid 3720
```

這是本次 `Handles` 分析中最重要的結果。

此結果表示 PID 3820 `Rick And Morty` 持有 PID 3720 `vmware-tray.ex` 的 Process handle。

這可以補強前面 `Pstree` 中看到的父子關係：

```text
Rick And Morty → vmware-tray.exe
```

因此，PID 3820 與 PID 3720 並非無關行程，而是存在明確的 Process 關聯。

---

## 5. PID 3720：vmware-tray.ex 分析

PID 3720 `vmware-tray.ex` 的 Handles 中，同樣出現以下重要 File handle：

```text
\Device\HarddiskVolume1\Users\Rick\AppData\Local\Temp\RarSFX0
```

這表示 `vmware-tray.ex` 執行時仍與 `RarSFX0` 暫存目錄有關。

由於真正的 VMware 工具程式通常不應該從使用者 Temp 目錄下的 `RarSFX0` 執行，因此此結果具有可疑性。

---

## 6. .NET / CLR 相關跡象

PID 3720 `vmware-tray.ex` 的 Handles 中也出現多個與 .NET Framework 相關的物件，例如：

```text
MACHINE\SOFTWARE\WOW6432NODE\MICROSOFT\.NETFRAMEWORK
Cor_SxSPublic_IPCBlock
Cor_Private_IPCBlock_v4_3720
CPFATE_3720_v4.0.30319
MACHINE\SOFTWARE\MICROSOFT\FUSION
NativeImages_v4.0.30319_32
```

這與前面 `VadInfo`、`LdrModules` 觀察到的結果一致，表示 `vmware-tray.ex` 很可能是 .NET 程式，並且載入 CLR / .NET Framework 相關元件。

這一點本身不一定代表惡意，但結合其執行路徑：

```text
C:\Users\Rick\AppData\Local\Temp\RarSFX0\vmware-tray.exe
```

以及前面 `Malfind` / `VadInfo` 發現的可疑記憶體區段，使 PID 3720 的可疑程度提高。

---

## 7. 鑑識判斷

本次 `Handles` 結果提供了幾個重要證據：

```text
1. PID 3820 Rick And Morty 開啟 RarSFX0 暫存目錄
2. PID 3820 Rick And Morty 持有 PID 3720 vmware-tray.ex 的 Process handle
3. PID 3720 vmware-tray.ex 也開啟 RarSFX0 暫存目錄
4. PID 3720 出現多個 .NET / CLR 相關 Handle
```

這些結果支持以下執行鏈：

```text
Rick 使用者執行 Rick And Morty season 1 download.exe
↓
該程式與 RarSFX0 暫存目錄產生關聯
↓
RarSFX0 目錄中出現並執行 vmware-tray.exe
↓
Rick And Morty 持有 vmware-tray.exe 的 Process handle
↓
vmware-tray.exe 進一步出現可疑記憶體區段與加密相關跡象
```

---

## 8. 與其他 Plugin 的關聯

`Handles` 結果可與前面 Plugin 互相補強：

```text
Pstree：顯示 Rick And Morty → vmware-tray.exe 父子關係
CmdLine：顯示 Rick And Morty 來自 Torrents，vmware-tray.exe 來自 Temp\RarSFX0
UserAssist：證明 Rick 使用者執行過 Rick And Morty season 1 download.exe
Malfind：發現 vmware-tray.exe 有可疑 PAGE_EXECUTE_READWRITE 記憶體區段
VadInfo：確認 vmware-tray.exe 有 PrivateMemory、File N/A 的可疑 VAD
DumpFiles：成功取得 READ_IT.txt，內容顯示檔案已被加密
```

因此，`Handles` 不是單獨證據，而是用來補強整體感染鏈的重要輔助證據。

---

## 9. 結論

`windows.handles.Handles` 成功針對 PID 3820 與 PID 3720 進行分析。

結果顯示 PID 3820 `Rick And Morty` 與 `RarSFX0` 暫存目錄存在關聯，且持有 PID 3720 `vmware-tray.ex` 的 Process handle。

同時，PID 3720 `vmware-tray.ex` 本身也開啟 `RarSFX0` 暫存目錄，並出現多個 .NET / CLR 相關 Handle。

綜合判斷，`Handles` 結果進一步支持本案的感染鏈：

```text
Rick And Morty season 1 download.exe
→ Temp\RarSFX0
→ vmware-tray.exe
→ 可疑記憶體區段
→ READ_IT.txt 加密提示
```

因此，PID 3820 與 PID 3720 應視為本案的主要可疑行程。
