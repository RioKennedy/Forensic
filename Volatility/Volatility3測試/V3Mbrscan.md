# 測試內容


- vol.exe -f .\OtterCTF.vmem windows.mbrscan.MBRScan | findstr "Potential MBR"
```
D:\Forensic\G140A006\VolatilityWorkbench>.\vol.exe -f .\OtterCTF.vmem windows.mbrscan.MBRScan | findstr "Potential MBR"
Potential MBR at Physical OffsetPDB scanDisk Signature  Bootcode MD5    Full MBR MD5    PartitionIndex   Bootable        PartitionType   SectorInSize    Disasm
* 0x22be4ac     dc-41-64-21     0f94c791288a9275c4c2658fdd64f258        6d9510b3e13429ba03cacc4693c96e27 4       False   Microsoft MBR,Dynamic Disk      0x876c758       N/A
* 0x9d21305     1c-56-93-a8     f35091a43a7f0dbbbbe20ca35c2ff8cd        2c00a710d2f0b24176ca5ae98777f1ba 2       False   Microsoft MBR,Dynamic Disk      0x8731a9f5      N/A
* 0xe37f408     bd-00-28-bd     bf196e85a20b0cc7bfcb4b537cb52330        10fee8680b082af57d4eb77c6e935346 4       False   Microsoft MBR,Dynamic Disk      0xbdaa50        N/A
* 0x12259b00    50-69-a8-67     535de392e94f71edfe1c0a133c682daa        4c42e2a3fed2d2ca29ab82494e83369c 4       False   Microsoft MBR,Dynamic Disk      0x6a50574a      N/A
* 0x12550f68    af-ff-19-6f     b343599008abad067a972eb20864b1ad        6ef1b3ca7da2878bde4a6801cba8884b 4       False   Microsoft MBR,Dynamic Disk      0xffcaa954      N/A
* 0x143871ce    68-57-8c-da     058ff02523cbc3cab2673fa4358d2e58        47c65edb5a04beca9ea181f2002a189b 3       False   Microsoft MBR,Dynamic Disk      0xa121424       N/A
* 0x159feb3e    50-69-a8-67     535de392e94f71edfe1c0a133c682daa        4c42e2a3fed2d2ca29ab82494e83369c 4       False   Microsoft MBR,Dynamic Disk      0x6a50574a      N/A
* 0x1847766a    00-dc-57-62     9d5f1c81755b8df1e70649d2841172b6        4dc521c8e8152c51f08970a5164441c4 2       False   Microsoft MBR,Dynamic Disk      0x7420c369      N/A
* 0x1d2bd365    80-ff-80-80     8064663eabf7735e89855bac98212b11        81ba2fb34716d6c944ba4943814209d5 1       True    Microsoft MBR,Dynamic Disk      0x8000000       N/A
* 0x1e5a7319    a8-8f-08-53     43b8fb804aa13c51a914951e5cfb7da9        6453b1060098566ff17fbb913e709b48 4       False   Microsoft MBR,Dynamic Disk      0x48ed0223      N/A
* 0x1e6ce297    f3-5f-e8-f2     57bd92d80d64a1966e834e1a0e6badd1        ae29b9241db9c7fbd9231540948c0546 2       False   Microsoft MBR,Dynamic Disk      0x7a463e14      N/A
* 0x2345f02e    f1-26-18-ea     18427c8facec255eb0a1d77cb9b3d9b6        73c589bd6ce13c9dc28c100c3c13391a 2       False   Microsoft MBR,Dynamic Disk      0x65ca26b0      N/A
* 0x2424d532    00-00-00-00     254729b924f10460854358c2a10ecb8a        b8a92fcc7ecc0e34d3585b3593c75bc2 2       False   Microsoft MBR,Dynamic Disk      0xa621f830      N/A
* 0x24d9a32b    1c-56-93-a8     f35091a43a7f0dbbbbe20ca35c2ff8cd        2c00a710d2f0b24176ca5ae98777f1ba 2       False   Microsoft MBR,Dynamic Disk      0x8731a9f5      N/A
* 0x29a2c14a    00-06-3b-de     218ce20b0b23c0b36970f96c20e0afe3        27ed9f4a63821ea3dc2ce02a352a3824 2       False   Microsoft MBR,Dynamic Disk      0x6009044       N/A
* 0x2bae0514    07-00-30-d2     4b35f7184c02aadd6fbc5765a341fd57        18795ec6089b77458d908ef7609cfbb0 4       False   Microsoft MBR,Dynamic Disk      0x7aa42 N/A
* 0x2bae051c    07-00-57-a9     6d76b6c213a1f4d1f5ca6b084fe0c485        f94c3e2d41b4e48a517777cf00c12383 4       False   Microsoft MBR,Dynamic Disk      0x12d3cc        N/A
* 0x2f397a74    30-00-30-00     6c25c19743dbbf288424127c704ed91e        576667621d06b4fcf7a9d64bc96868fb 3       False   Microsoft MBR,Dynamic Disk      0x4     N/A
* 0x33759310    00-00-00-00     eb10427c60dd1496f345d0b368e85471        0d9086f0e46233e0285ee171c4152521 4       False   Microsoft MBR,Dynamic Disk      0xffc7a54f      N/A
* 0x38e19e38    af-ff-19-6f     b343599008abad067a972eb20864b1ad        6ef1b3ca7da2878bde4a6801cba8884b 4       False   Microsoft MBR,Dynamic Disk      0xffcaa954      N/A
* 0x3ac4dc61    00-39-01-0e     f417bbfa7d65733d02805e46d4531779        99053b15a30b1cc23a18d00934525d78 4       False   Microsoft MBR,Dynamic Disk      0xb8182070      N/A
* 0x4394e714    07-00-30-d2     4b35f7184c02aadd6fbc5765a341fd57        18795ec6089b77458d908ef7609cfbb0 4       False   Microsoft MBR,Dynamic Disk      0x7aa42 N/A
* 0x4394e71c    07-00-57-a9     6d76b6c213a1f4d1f5ca6b084fe0c485        f94c3e2d41b4e48a517777cf00c12383 4       False   Microsoft MBR,Dynamic Disk      0x12d3cc        N/A
* 0x43c43ecb    0f-c5-cb-65     f7188caf2fdf1db6a2cb47a553fa5a81        5ed560d85f47d9139ae8ccd7f02320f5 1       False   Microsoft MBR,Dynamic Disk      0x3cc20862      N/A
* 0x49c00290    1f-6f-f9-49     784e98306f06e4a1ee7b1ce8c93f2feb        95c42ff71d6c6ea22bc496d99d379fdc 4       False   Microsoft MBR,Dynamic Disk      0xcc67017e      N/A
* 0x4e6ffdeb    71-f1-ee-dc     63eb827e6b3a14ea9f21b74fce9bbe25        f4fa204516aaec5643d928d724b73f8f 1       False   Microsoft MBR,Dynamic Disk      0xa8b53209      N/A
* 0x4e96754a    71-f1-ee-dc     63eb827e6b3a14ea9f21b74fce9bbe25        f4fa204516aaec5643d928d724b73f8f 1       False   Microsoft MBR,Dynamic Disk      0xa8b53209      N/A
* 0x50489eff    0c-7d-27-75     d9c3ef896f307302f9e38cdba00f3eaf        48bc10a8f76aea3d1fe9cb8780c99c61 3       False   Microsoft MBR,Dynamic Disk      0xfe486ad0      N/A
* 0x50b07376    12-50-af-09     a146b9c3b7ca7876e60f828cb28f0b4a        5c5194d51d9585f789e8ac17fc8059ca 3       False   Microsoft MBR,Dynamic Disk      0x8842109a      N/A
* 0x511e5644    2f-85-75-af     ca26a0066fb074a1adb82fe4b8232b4e        4cc78173cdbeb82e76e2511327410dc6 3       False   Microsoft MBR,Dynamic Disk      0xf29e78d2      N/A
* 0x51824adb    e5-d9-53-83     8ae54670c3fcc88bdb00666b16e58221        694038d0d340da8803e95a88e6957e8f 2       False   Microsoft MBR,Dynamic Disk      0xe99e7333      N/A
* 0x51b4b154    c0-7a-e6-c9     df009420a3d73ee24619a35bd3ae9d0e        93a4b35146b0ce2797f22cf1770492ed 3       False   Microsoft MBR,Dynamic Disk      0x5bc4ba2a      N/A
* 0x5212f8ae    c6-d5-a0-75     a80ef0da9ab9ca5af78101ddcee9e692        63b952d3ecf06e2cd11c9a33d942ccb4 3       False   Microsoft MBR,Dynamic Disk      0x39fcb519      N/A
* 0x5284bb39    c6-d5-a0-75     d211685e20af1fe9c1815e8fcb35bd96        eeea7931d3de463397f98f3fc9cc7985 3       False   Microsoft MBR,Dynamic Disk      0x39fcb519      N/A
* 0x529b5832    49-95-cc-ab     989c4c52d80c3d9c788215f68fde480a        5c7bc601cffea46efbfd8ad38ab29ead 2       False   Microsoft MBR,Dynamic Disk      0xd6f55d8c      N/A
* 0x52b90a90    49-95-cc-ab     989c4c52d80c3d9c788215f68fde480a        5c7bc601cffea46efbfd8ad38ab29ead 2       False   Microsoft MBR,Dynamic Disk      0xd6f55d8c      N/A
* 0x530f9df2    ad-72-57-ad     4fa55816d72a26b464016a1e4d84f7b4        76ca8df8b9ce13cacb92d32770d45634 3       False   Microsoft MBR,Dynamic Disk      0x7085b205      N/A
* 0x56830d4b    9e-fc-80-cf     25be5d453b5bce8e55704e72411b49c2        3be890c97494335f8401a89b4dccc52b 3       False   Microsoft MBR,Dynamic Disk      0xfb543b91      N/A
* 0x58daf2f1    3d-9d-1e-d1     e53a4dd285413e1eeaddd753c28e8891        d78d17895788637f7d4662027a673298 4       False   Microsoft MBR,Dynamic Disk      0x3ef755e3      N/A
* 0x5967e375    b4-f1-cc-61     059f6c2c5bc3335e618c1519ded9be96        086419d76fcc5cb2105df9cb64e1586c 4       False   Microsoft MBR,Dynamic Disk      0x6459d4dd      N/A
* 0x5c314545    00-73-00-74     8ba9cd8bc97a1312af3d207474e55867        1e901e3c5de99038cbe2d490bcbbb642 2       False   Microsoft MBR,Dynamic Disk      0x246f09f6      N/A
* 0x5db77b30    1f-6f-f9-49     784e98306f06e4a1ee7b1ce8c93f2feb        95c42ff71d6c6ea22bc496d99d379fdc 4       False   Microsoft MBR,Dynamic Disk      0xcc67017e      N/A
* 0x5dedda7d    64-85-ac-c0     a764d3ae8c061891167db90767eeb0e7        7d6c3e9fcff375561ce47187a5185f6c 2       False   Microsoft MBR,Dynamic Disk      0x7fad26bd      N/A
* 0x5df4bce0    47-c8-d5-e5     6a1434b15fc8e27fcab952f8f5ebca18        faacf1d02f3aa0f3d6b5d85774a61d09 3       False   Microsoft MBR,Dynamic Disk      0x857edecd      N/A
* 0x5e153c10    47-c8-d5-e5     6a1434b15fc8e27fcab952f8f5ebca18        faacf1d02f3aa0f3d6b5d85774a61d09 3       False   Microsoft MBR,Dynamic Disk      0x857edecd      N/A
* 0x6105478e    af-7d-41-45     a2455f82e63c282938d99f4a7949be75        48f5cfa3cce362d63ecf37a01d2acea4 4       False   Microsoft MBR,Dynamic Disk      0xe2ae24d2      N/A
* 0x616987da    fa-80-f3-c2     b99e34a35f663fed2406925f2e331f1f        a71ea0a9019b758e2c0081cf1266f304 2       False   Microsoft MBR,Dynamic Disk      0x226a2ca5      N/A
* 0x63208b20    78-e0-3b-ef     af87f49343fbf013ed25a9f0708731fa        4924c0d6b82a7f70b023dd27fd9528da 4       False   Microsoft MBR,Dynamic Disk      0x5bbe53e1      N/A
* 0x63208e50    78-e0-3b-ef     82426a2528ca8a3fed7a1febf751a5f5        72d5668710166daa54e04075001e3e37 4       False   Microsoft MBR,Dynamic Disk      0x5bbe53e1      N/A
* 0x6cb246a9    55-b0-7c-55     4bb3490a9f698ad7a06aade0a75440e9        297ff8ceac3b443d230ae2d4c0e8bd84 4       False   Microsoft MBR,Dynamic Disk      0xb74200c0      N/A
* 0x6f6b4d55    92-88-01-5e     c8c0504c36f5d36957faf428c707080d        117c9e6ec9f39b5e4b5a24a6f387b0ee 4       False   Microsoft MBR,Dynamic Disk      0xbfc21758      N/A
* 0x7218fa3b    bd-12-eb-88     bf6016770b440b180bfec4d8a4736977        56ca56badfa89edc858aa40fa0a0452c 2       False   Microsoft MBR,Dynamic Disk      0x749a1073      N/A
* 0x74f78fb0    e5-ff-5e-68     012cf58b8765415d4ba84ea8c714966b        3cef7beaf92f038e8f22d4fd3df98b3a 4       False   Microsoft MBR,Dynamic Disk      0xffcaa954      N/A
* 0x7a92a275    80-ff-80-80     e7fe0de8dc202607351e23fdfba15d87        c294766db987c4d4bfdefa5c50478488 1       True    Microsoft MBR,Dynamic Disk      0x8000000       N/A
* 0x7e7ce3e3    dc-41-64-21     0f94c791288a9275c4c2658fdd64f258        6d9510b3e13429ba03cacc4693c96e27 4       False   Microsoft MBR,Dynamic Disk      0x876c758       N/A
* 0x7ef470bf    36-69-37-67     e87be597cda1c4dd5ba67ef4180f234d        a2470bbaee5eca8f21f3629c89cdf0e8 4       False   Microsoft MBR,Dynamic Disk      0x876c758       N/A
```


- vol.exe -f .\OtterCTF.vmem windows.mbrscan.MBRScan | findstr "Disk Signature"
```
D:\Forensic\G140A006\VolatilityWorkbench>.\vol.exe -f .\OtterCTF.vmem windows.mbrscan.MBRScan | findstr "Disk Signature"
Potential MBR at Physical OffsetPDB scanDisk Signature  Bootcode MD5    Full MBR MD5    PartitionIndex   Bootable        PartitionType   SectorInSize    Disasm
* 0x22be4ac     dc-41-64-21     0f94c791288a9275c4c2658fdd64f258        6d9510b3e13429ba03cacc4693c96e27 4       False   Microsoft MBR,Dynamic Disk      0x876c758       N/A
* 0x9d21305     1c-56-93-a8     f35091a43a7f0dbbbbe20ca35c2ff8cd        2c00a710d2f0b24176ca5ae98777f1ba 2       False   Microsoft MBR,Dynamic Disk      0x8731a9f5      N/A
* 0xadd16ad     6e-e8-c2-b8     0b595118de8fa51b9f742c39fa9735ad        2a9820714516d35952d19e276fa90d68 2       False   EFI GPT Disk    0x1ac9a4a0      N/A
* 0xda5a235     b8-1d-46-93     add52abef05ffa425ce7de6655a1934e        11e7bc812fea2923b73f91acbdbb0e85 1       False   EFI GPT Disk    0x874541c7      N/A
* 0xe37f408     bd-00-28-bd     bf196e85a20b0cc7bfcb4b537cb52330        10fee8680b082af57d4eb77c6e935346 4       False   Microsoft MBR,Dynamic Disk      0xbdaa50        N/A
* 0x116817a9    00-00-00-00     8bcbbddc06cc0de3ad5a15c48e1bea32        9d8a022f5a42a2f24f22657607254f55 4       False   EFI GPT Disk    0xffdd00        N/A
* 0x116817ad    00-00-00-00     bd9672f9857b80ee8e5861cf92e4a566        eaf41b098f074ddfdc1402d6ea0c5ed5 3       False   EFI GPT Disk    0x11ffffee      N/A
* 0x11681825    00-00-00-00     f21b81a89cd5620947813f83ee2dd109        6f5682720ebf45013fdc317222fcb25b 3       False   EFI GPT Disk    0x11ffffee      N/A
* 0x116818a1    00-00-00-00     822260ac999d4de1de7a6bf9a2df56e2        ccb40f84f5d7fccbed500c4116d1e097 2       False   EFI GPT Disk    0xffff00        N/A
* 0x12259b00    50-69-a8-67     535de392e94f71edfe1c0a133c682daa        4c42e2a3fed2d2ca29ab82494e83369c 4       False   Microsoft MBR,Dynamic Disk      0x6a50574a      N/A
* 0x12550f68    af-ff-19-6f     b343599008abad067a972eb20864b1ad        6ef1b3ca7da2878bde4a6801cba8884b 4       False   Microsoft MBR,Dynamic Disk      0xffcaa954      N/A
* 0x126818ad    00-00-00-00     8bcbbddc06cc0de3ad5a15c48e1bea32        9d8a022f5a42a2f24f22657607254f55 4       False   EFI GPT Disk    0xffdd00        N/A
* 0x126818b1    00-00-00-00     bd9672f9857b80ee8e5861cf92e4a566        eaf41b098f074ddfdc1402d6ea0c5ed5 3       False   EFI GPT Disk    0x11ffffee      N/A
* 0x12681929    00-00-00-00     f21b81a89cd5620947813f83ee2dd109        6f5682720ebf45013fdc317222fcb25b 3       False   EFI GPT Disk    0x11ffffee      N/A
* 0x126819a5    00-00-00-00     327a8c9ca8bc5f420dd60809c2b7a4c3        2748f3c624ac5c694c64facef7bd90f0 2       False   EFI GPT Disk    0xffff00        N/A
* 0x143871ce    68-57-8c-da     058ff02523cbc3cab2673fa4358d2e58        47c65edb5a04beca9ea181f2002a189b 3       False   Microsoft MBR,Dynamic Disk      0xa121424       N/A
* 0x159feb3e    50-69-a8-67     535de392e94f71edfe1c0a133c682daa        4c42e2a3fed2d2ca29ab82494e83369c 4       False   Microsoft MBR,Dynamic Disk      0x6a50574a      N/A
* 0x172fe8ea    e7-3c-7c-7c     86f209d90d94a20d7ac24785aa357007        fda3418fde73a3530c3dead114695933 4       False   EFI GPT Disk    0x793e568b      N/A
* 0x1847766a    00-dc-57-62     9d5f1c81755b8df1e70649d2841172b6        4dc521c8e8152c51f08970a5164441c4 2       False   Microsoft MBR,Dynamic Disk      0x7420c369      N/A
* 0x1a970a6d    00-00-00-00     0fb71f6f896559fe504cc1f5dcd1f11e        7a8139404afbcd74981e647a8b3f89c8 2       False   EFI GPT Disk    0xee00eeee      N/A
* 0x1a970a6d    00-00-00-00     0fb71f6f896559fe504cc1f5dcd1f11e        7a8139404afbcd74981e647a8b3f89c8 3       False   EFI GPT Disk    0xcc00eeee      N/A
* 0x1a970a75    00-00-11-22     95eb8c6b61787456dd5daab300cd7877        7b6d0ea63d2b1a219c6e802ce1c28620 2       False   EFI GPT Disk    0xee00eeee      N/A
* 0x1a970a75    00-00-11-22     95eb8c6b61787456dd5daab300cd7877        7b6d0ea63d2b1a219c6e802ce1c28620 3       False   EFI GPT Disk    0x5500dd99      N/A
* 0x1d2bd365    80-ff-80-80     8064663eabf7735e89855bac98212b11        81ba2fb34716d6c944ba4943814209d5 1       True    Microsoft MBR,Dynamic Disk      0x8000000       N/A
* 0x1e5a7319    a8-8f-08-53     43b8fb804aa13c51a914951e5cfb7da9        6453b1060098566ff17fbb913e709b48 4       False   Microsoft MBR,Dynamic Disk      0x48ed0223      N/A
* 0x1e6ce297    f3-5f-e8-f2     57bd92d80d64a1966e834e1a0e6badd1        ae29b9241db9c7fbd9231540948c0546 2       False   Microsoft MBR,Dynamic Disk      0x7a463e14      N/A
* 0x2345f02e    f1-26-18-ea     18427c8facec255eb0a1d77cb9b3d9b6        73c589bd6ce13c9dc28c100c3c13391a 2       False   Microsoft MBR,Dynamic Disk      0x65ca26b0      N/A
* 0x2424d532    00-00-00-00     254729b924f10460854358c2a10ecb8a        b8a92fcc7ecc0e34d3585b3593c75bc2 2       False   Microsoft MBR,Dynamic Disk      0xa621f830      N/A
* 0x24d9a32b    1c-56-93-a8     f35091a43a7f0dbbbbe20ca35c2ff8cd        2c00a710d2f0b24176ca5ae98777f1ba 2       False   Microsoft MBR,Dynamic Disk      0x8731a9f5      N/A
* 0x2770b9a8    99-00-ff-ee     aebe38028fc815ca10942c5bd8778f28        4262f21c8f88055978c2bddaf982b669 1       False   EFI GPT Disk    0x66bb  N/A
* 0x2847c80c    6e-e8-c2-b8     0b595118de8fa51b9f742c39fa9735ad        2a9820714516d35952d19e276fa90d68 2       False   EFI GPT Disk    0x1ac9a4a0      N/A
* 0x2911d20f    23-22-00-11     6f5c9087c2403bffacd7ba7f6c9dfad7        2afb888263a7f375682aa55af01ddce6 3       False   EFI GPT Disk    0x66b44c5c      N/A
* 0x29a2c14a    00-06-3b-de     218ce20b0b23c0b36970f96c20e0afe3        27ed9f4a63821ea3dc2ce02a352a3824 2       False   Microsoft MBR,Dynamic Disk      0x6009044       N/A
* 0x2b730e78    6e-e8-c2-b8     0b595118de8fa51b9f742c39fa9735ad        2a9820714516d35952d19e276fa90d68 2       False   EFI GPT Disk    0x1ac9a4a0      N/A
* 0x2bae0514    07-00-30-d2     4b35f7184c02aadd6fbc5765a341fd57        18795ec6089b77458d908ef7609cfbb0 4       False   Microsoft MBR,Dynamic Disk      0x7aa42 N/A
* 0x2bae051c    07-00-57-a9     6d76b6c213a1f4d1f5ca6b084fe0c485        f94c3e2d41b4e48a517777cf00c12383 4       False   Microsoft MBR,Dynamic Disk      0x12d3cc        N/A
* 0x2c176e6d    00-00-00-00     8bcbbddc06cc0de3ad5a15c48e1bea32        9d8a022f5a42a2f24f22657607254f55 4       False   EFI GPT Disk    0xffdd00        N/A
* 0x2c176e71    00-00-00-00     bd9672f9857b80ee8e5861cf92e4a566        eaf41b098f074ddfdc1402d6ea0c5ed5 3       False   EFI GPT Disk    0x11ffffee      N/A
* 0x2c176ee9    00-00-00-00     f21b81a89cd5620947813f83ee2dd109        6f5682720ebf45013fdc317222fcb25b 3       False   EFI GPT Disk    0x11ffffee      N/A
* 0x2c176f65    00-00-00-00     327a8c9ca8bc5f420dd60809c2b7a4c3        2748f3c624ac5c694c64facef7bd90f0 2       False   EFI GPT Disk    0xffff00        N/A
* 0x2c1f906d    00-00-00-00     d7bbf3699972b7f6781829a1e40d32bc        57150d72f0d13ec25f92511e8a17e2b8 4       False   EFI GPT Disk    0xffdd00        N/A
* 0x2c1f9071    00-00-00-00     20390f587edf7617f6a5300d77aa3dc8        d4bd17833073e6af538640d3cc0ae21e 3       False   EFI GPT Disk    0x11ffffee      N/A
* 0x2c1f90e9    00-00-00-00     7cb58f9774d4f8d561c45d18d30d5c0d        de963759223dbf9fe3b510bfd1e16cf3 3       False   EFI GPT Disk    0x11ffffee      N/A
* 0x2c1f9165    00-00-00-00     5122322ad2ca52f7510516edd47cdeab        c58a857f2e4f1033e19777e1015cb7a1 2       False   EFI GPT Disk    0xffff00        N/A
* 0x2c2993fd    00-00-00-00     44a318f8d334d79dbc96be73a9e18659        0dc18933cb2e5f458403a91a790e044e 2       False   EFI GPT Disk    0xeeffffff      N/A
* 0x2c2993fd    00-00-00-00     44a318f8d334d79dbc96be73a9e18659        0dc18933cb2e5f458403a91a790e044e 3       False   EFI GPT Disk    0xeeffffff      N/A
* 0x2c2993fd    00-00-00-00     44a318f8d334d79dbc96be73a9e18659        0dc18933cb2e5f458403a91a790e044e 4       False   EFI GPT Disk    0x55ffaaaa      N/A
* 0x2c7982fd    00-00-00-00     44a318f8d334d79dbc96be73a9e18659        0dc18933cb2e5f458403a91a790e044e 2       False   EFI GPT Disk    0xeeffffff      N/A
* 0x2c7982fd    00-00-00-00     44a318f8d334d79dbc96be73a9e18659        0dc18933cb2e5f458403a91a790e044e 3       False   EFI GPT Disk    0xeeffffff      N/A
* 0x2c7982fd    00-00-00-00     44a318f8d334d79dbc96be73a9e18659        0dc18933cb2e5f458403a91a790e044e 4       False   EFI GPT Disk    0x55ffaaaa      N/A
* 0x2c886eed    00-00-00-00     8bcbbddc06cc0de3ad5a15c48e1bea32        9d8a022f5a42a2f24f22657607254f55 4       False   EFI GPT Disk    0xffdd00        N/A
* 0x2c886ef1    00-00-00-00     bd9672f9857b80ee8e5861cf92e4a566        eaf41b098f074ddfdc1402d6ea0c5ed5 3       False   EFI GPT Disk    0x11ffffee      N/A
* 0x2c886f69    00-00-00-00     f21b81a89cd5620947813f83ee2dd109        6f5682720ebf45013fdc317222fcb25b 3       False   EFI GPT Disk    0x11ffffee      N/A
* 0x2c886fe5    00-00-00-00     327a8c9ca8bc5f420dd60809c2b7a4c3        2748f3c624ac5c694c64facef7bd90f0 2       False   EFI GPT Disk    0xffff00        N/A
* 0x2c8fa189    00-00-00-00     7732b5bdbfd90e0e317f285941b458a8        814d4b51076ad7d941ab4b73f9783e1c 4       False   EFI GPT Disk    0xffdd00        N/A
* 0x2c8fa18d    00-00-00-00     afa7cc6a3905512aa6f6797f976a356e        673c1d32a280666fa0ed19a122f19d24 3       False   EFI GPT Disk    0x11ffffee      N/A
* 0x2c8fa205    00-00-00-00     f21b81a89cd5620947813f83ee2dd109        6f5682720ebf45013fdc317222fcb25b 3       False   EFI GPT Disk    0x11ffffee      N/A
* 0x2c8fa281    00-00-00-00     822260ac999d4de1de7a6bf9a2df56e2        ccb40f84f5d7fccbed500c4116d1e097 2       False   EFI GPT Disk    0xffff00        N/A
* 0x2c93f6ad    00-00-00-00     8bcbbddc06cc0de3ad5a15c48e1bea32        9d8a022f5a42a2f24f22657607254f55 4       False   EFI GPT Disk    0xffdd00        N/A
* 0x2c93f6b1    00-00-00-00     bd9672f9857b80ee8e5861cf92e4a566        eaf41b098f074ddfdc1402d6ea0c5ed5 3       False   EFI GPT Disk    0x11ffffee      N/A
* 0x2c93f729    00-00-00-00     f21b81a89cd5620947813f83ee2dd109        6f5682720ebf45013fdc317222fcb25b 3       False   EFI GPT Disk    0x11ffffee      N/A
* 0x2c93f7a5    00-00-00-00     327a8c9ca8bc5f420dd60809c2b7a4c3        2748f3c624ac5c694c64facef7bd90f0 2       False   EFI GPT Disk    0xffff00        N/A
* 0x2c94accd    00-00-00-00     18f4098a237da7e87adaaae1054f2ecd        67d8831f5ebd6feef4e4093f84efbcda 4       False   EFI GPT Disk    0xff0088        N/A
* 0x2c94acd1    00-00-00-00     53b6c4bb78eb538737dff2171dbc2d2d        55a1b6b6c522c5674369e8607017e1d0 3       False   EFI GPT Disk    0x11ffffee      N/A
* 0x2c94ad49    00-00-00-00     4e6d7a949deb483f1691bcea0a509792        251f14680e2fe552fef55b25268da942 3       False   EFI GPT Disk    0x11ffffee      N/A
* 0x2c94adc5    00-00-00-00     7d5c4f85672fd8a1236ad9556eab7b1c        df5232b3317705c6f6e6ed41b6abdb0e 2       False   EFI GPT Disk    0xff11bb        N/A
* 0x2c975d69    00-00-00-00     8bcbbddc06cc0de3ad5a15c48e1bea32        9d8a022f5a42a2f24f22657607254f55 4       False   EFI GPT Disk    0xffdd00        N/A
* 0x2c975d6d    00-00-00-00     bd9672f9857b80ee8e5861cf92e4a566        eaf41b098f074ddfdc1402d6ea0c5ed5 3       False   EFI GPT Disk    0x11ffffee      N/A
* 0x2c975de5    00-00-00-00     f21b81a89cd5620947813f83ee2dd109        6f5682720ebf45013fdc317222fcb25b 3       False   EFI GPT Disk    0x11ffffee      N/A
* 0x2c975e61    00-00-00-00     822260ac999d4de1de7a6bf9a2df56e2        ccb40f84f5d7fccbed500c4116d1e097 2       False   EFI GPT Disk    0xffff00        N/A
* 0x2c9b8061    00-00-00-00     fcd5bec89ecd93c0c6b8a7cb98040fe3        3eacb77a248f22047c9356f3086a853d 2       False   EFI GPT Disk    0xffff00        N/A
* 0x2d905de9    00-00-00-00     8bcbbddc06cc0de3ad5a15c48e1bea32        9d8a022f5a42a2f24f22657607254f55 4       False   EFI GPT Disk    0xffdd00        N/A
* 0x2d905ded    00-00-00-00     bd9672f9857b80ee8e5861cf92e4a566        eaf41b098f074ddfdc1402d6ea0c5ed5 3       False   EFI GPT Disk    0x11ffffee      N/A
* 0x2d905e65    00-00-00-00     f21b81a89cd5620947813f83ee2dd109        6f5682720ebf45013fdc317222fcb25b 3       False   EFI GPT Disk    0x11ffffee      N/A
* 0x2d905ee1    00-00-00-00     822260ac999d4de1de7a6bf9a2df56e2        ccb40f84f5d7fccbed500c4116d1e097 2       False   EFI GPT Disk    0xffff00        N/A
* 0x2d97e5a9    00-00-00-00     8bcbbddc06cc0de3ad5a15c48e1bea32        9d8a022f5a42a2f24f22657607254f55 4       False   EFI GPT Disk    0xffdd00        N/A
* 0x2d97e5ad    00-00-00-00     bd9672f9857b80ee8e5861cf92e4a566        eaf41b098f074ddfdc1402d6ea0c5ed5 3       False   EFI GPT Disk    0x11ffffee      N/A
* 0x2d97e625    00-00-00-00     f21b81a89cd5620947813f83ee2dd109        6f5682720ebf45013fdc317222fcb25b 3       False   EFI GPT Disk    0x11ffffee      N/A
* 0x2d97e6a1    00-00-00-00     822260ac999d4de1de7a6bf9a2df56e2        ccb40f84f5d7fccbed500c4116d1e097 2       False   EFI GPT Disk    0xffff00        N/A
* 0x2d99af9d    ff-11-11-11     3179b05678a22f18d21c6c42d3bea1b7        a9864fd1f7db4c56490b8d86f242151a 3       False   EFI GPT Disk    0xffee99        N/A
* 0x2d99afa1    ff-11-11-11     4ec40b6091137e674672b52fbf6779cb        03d9c73e961f13b1a37327f6dc455504 3       False   EFI GPT Disk    0xffbb66        N/A
* 0x2da77f69    00-00-00-00     8bcbbddc06cc0de3ad5a15c48e1bea32        9d8a022f5a42a2f24f22657607254f55 4       False   EFI GPT Disk    0xffdd00        N/A
* 0x2da77f6d    00-00-00-00     bd9672f9857b80ee8e5861cf92e4a566        eaf41b098f074ddfdc1402d6ea0c5ed5 3       False   EFI GPT Disk    0x11ffffee      N/A
* 0x2da77fe5    00-00-00-00     f21b81a89cd5620947813f83ee2dd109        6f5682720ebf45013fdc317222fcb25b 3       False   EFI GPT Disk    0x11ffffee      N/A
* 0x2dcdb02d    00-00-00-00     f1ad23587a8aed044d8f636f07f3729d        3b22db2ccbd68023a2d8ee029d434e3d 2       False   EFI GPT Disk    0xffbb66        N/A
* 0x2dcdb099    ff-11-11-11     7e7beeb03ad1b9801691145624bc8c7a        dc97f6823aecd9ef8c4a33d7f28698c7 3       False   EFI GPT Disk    0xffee99        N/A
* 0x2dcdb09d    ff-11-11-11     1d50a8d56b1ed5a4bb1d12fa47b2f6ec        f0c5371424094b457090a791df4cfcbd 3       False   EFI GPT Disk    0xffbb66        N/A
* 0x2dcdb0ad    ff-11-11-11     236fac80bc6dae9f4678dfeb7a55393b        e4d83099931c69b7feb2681a2495a78e 2       False   EFI GPT Disk    0xffbb66        N/A
* 0x2dcdb129    00-00-00-00     423caec4f7144c6536e5c0d8478ae00b        37f09204374ee764b5b33a5dc284c8cc 2       False   EFI GPT Disk    0xffbb66        N/A
* 0x2dcdb295    00-00-00-00     e51db2465a0cddc71dc6c96abb50356a        7614bc7bc216584006281bc05010fd0b 3       False   EFI GPT Disk    0xffee99        N/A
* 0x2ddfb28d    00-00-00-00     8bcbbddc06cc0de3ad5a15c48e1bea32        9d8a022f5a42a2f24f22657607254f55 4       False   EFI GPT Disk    0xffdd00        N/A
* 0x2ddfb291    00-00-00-00     bd9672f9857b80ee8e5861cf92e4a566        eaf41b098f074ddfdc1402d6ea0c5ed5 3       False   EFI GPT Disk    0x11ffffee      N/A
* 0x2ddfb309    00-00-00-00     f21b81a89cd5620947813f83ee2dd109        6f5682720ebf45013fdc317222fcb25b 3       False   EFI GPT Disk    0x11ffffee      N/A
* 0x2ddfb385    00-00-00-00     327a8c9ca8bc5f420dd60809c2b7a4c3        2748f3c624ac5c694c64facef7bd90f0 2       False   EFI GPT Disk    0xffff00        N/A
* 0x2ddfc389    00-00-00-00     8bcbbddc06cc0de3ad5a15c48e1bea32        9d8a022f5a42a2f24f22657607254f55 4       False   EFI GPT Disk    0xffdd00        N/A
* 0x2ddfc38d    00-00-00-00     bd9672f9857b80ee8e5861cf92e4a566        eaf41b098f074ddfdc1402d6ea0c5ed5 3       False   EFI GPT Disk    0x11ffffee      N/A
* 0x2ddfc405    00-00-00-00     f21b81a89cd5620947813f83ee2dd109        6f5682720ebf45013fdc317222fcb25b 3       False   EFI GPT Disk    0x11ffffee      N/A
* 0x2ddfc481    00-00-00-00     822260ac999d4de1de7a6bf9a2df56e2        ccb40f84f5d7fccbed500c4116d1e097 2       False   EFI GPT Disk    0xffff00        N/A
* 0x2dfdc09d    ff-11-11-11     6374f9671652f633dbe5125f60a75136        daafff7dfc38861ffade3ec572a30944 3       False   EFI GPT Disk    0xffee99        N/A
* 0x2dfdc0a1    ff-11-11-11     33f8010e843fe80330b559c0addba1ab        e42112435bab49013f29071040184d05 3       False   EFI GPT Disk    0xffbb66        N/A
* 0x2dfdc12d    ff-00-66-bb     25f0f59ce9d21fa805cb18109a848538        c7fb663b60b7473d30705c4fbe42a155 2       False   EFI GPT Disk    0xffbb66        N/A
* 0x2dfdc199    ff-11-11-11     336fd265be18004977853632aaffbf39        34b0fe9e850b67fd34fae610ebf3608a 3       False   EFI GPT Disk    0xffee99        N/A
* 0x2dfdc19d    ff-11-11-11     b87005439745ee1cf9001dee389f715c        d7aead2c09bf4f195d82c4c43f355017 3       False   EFI GPT Disk    0xffbb66        N/A
* 0x2dfdc1ad    ff-11-11-11     a02ba04648fdd2b836de36ebf4e66d1a        d25c4ec44c6e449e029187ef6a43eebb 2       False   EFI GPT Disk    0xffbb66        N/A
* 0x2dfdc229    00-00-00-00     2677cdbd40439fbfb870140f25cdc3cf        4949c379e4d64b9414ce7557b75189fb 2       False   EFI GPT Disk    0xffbb66        N/A
* 0x2dfdc395    00-00-00-00     e51db2465a0cddc71dc6c96abb50356a        7614bc7bc216584006281bc05010fd0b 3       False   EFI GPT Disk    0xffee99        N/A
* 0x2e0c4bc5    00-00-00-00     18f4098a237da7e87adaaae1054f2ecd        67d8831f5ebd6feef4e4093f84efbcda 4       False   EFI GPT Disk    0xff0088        N/A
* 0x2e0c4bc9    00-00-00-00     53b6c4bb78eb538737dff2171dbc2d2d        55a1b6b6c522c5674369e8607017e1d0 3       False   EFI GPT Disk    0x11ffffee      N/A
* 0x2e0c4c41    00-00-00-00     4e6d7a949deb483f1691bcea0a509792        251f14680e2fe552fef55b25268da942 3       False   EFI GPT Disk    0x11ffffee      N/A
* 0x2e0c4cbd    00-00-00-00     55a2b2d52251005dcf0b53281647071e        c78c026036afee691dff709ba68e375c 2       False   EFI GPT Disk    0xff11bb        N/A
* 0x2e17d48d    00-00-00-00     8bcbbddc06cc0de3ad5a15c48e1bea32        9d8a022f5a42a2f24f22657607254f55 4       False   EFI GPT Disk    0xffdd00        N/A
* 0x2e17d491    00-00-00-00     bd9672f9857b80ee8e5861cf92e4a566        eaf41b098f074ddfdc1402d6ea0c5ed5 3       False   EFI GPT Disk    0x11ffffee      N/A
* 0x2e17d509    00-00-00-00     f21b81a89cd5620947813f83ee2dd109        6f5682720ebf45013fdc317222fcb25b 3       False   EFI GPT Disk    0x11ffffee      N/A
* 0x2e17d585    00-00-00-00     327a8c9ca8bc5f420dd60809c2b7a4c3        2748f3c624ac5c694c64facef7bd90f0 2       False   EFI GPT Disk    0xffff00        N/A
* 0x2ee2ba74    71-00-75-00     e9ed9a7586e7c0e319caf83ff0155219        6c971596b70f4a0233c78d12d3c79cf2 1       False   EFI GPT Disk    0xddf9a316      N/A
* 0x2f397a74    30-00-30-00     6c25c19743dbbf288424127c704ed91e        576667621d06b4fcf7a9d64bc96868fb 3       False   Microsoft MBR,Dynamic Disk      0x4     N/A
* 0x2fed4b85    0d-3e-2f-4f     197fb422558f92349477f82c5301f095        5755a325beba957e4efbe8cfcaa7a123 3       False   EFI GPT Disk    0x26af6802      N/A
* 0x305ca3bc    6e-dd-3a-d7     1d01db9178b666d235d227cb16d762cc        4d4a4bbed3739283dfb73b7ac2e381f0 3       False   EFI GPT Disk    0xeca78b77      N/A
* 0x310dd7e2    e9-73-c5-7e     9143116ea5e166b7a816407f42555ab5        66a2821e54daac20941b7947e6263872 3       False   EFI GPT Disk    0xf1d86b97      N/A
* 0x33759310    00-00-00-00     eb10427c60dd1496f345d0b368e85471        0d9086f0e46233e0285ee171c4152521 4       False   Microsoft MBR,Dynamic Disk      0xffc7a54f      N/A
* 0x387b0981    00-22-44-66     9e7a4a91e61ad641880a8b0f160ac9e3        f3676ae85cd97ce4ef99e80d9262fce3 3       False   EFI GPT Disk    0x9900eeee      N/A
* 0x38e19e38    af-ff-19-6f     b343599008abad067a972eb20864b1ad        6ef1b3ca7da2878bde4a6801cba8884b 4       False   Microsoft MBR,Dynamic Disk      0xffcaa954      N/A
* 0x3ac4dc61    00-39-01-0e     f417bbfa7d65733d02805e46d4531779        99053b15a30b1cc23a18d00934525d78 4       False   Microsoft MBR,Dynamic Disk      0xb8182070      N/A
* 0x3caa8b77    5f-5d-be-87     fd785248816982afec3322e1fed3eda4        b0855419ae415ac6f07415072dd3257a 3       False   EFI GPT Disk    0xeca181f3      N/A
* 0x3e986158    00-00-bb-66     d9f9cd91cf4a1d98ccc2778096d7afd5        4443b334cfef9ccb08ecc3fa48c17311 1       False   EFI GPT Disk    0xaabbdd        N/A
* 0x40321c7d    00-00-00-00     b7e0c18c77c64531bc3ea141bb31c4b0        0155c8da756b7157310035490459fd92 2       False   EFI GPT Disk    0xee00ffff      N/A
* 0x40321c7d    00-00-00-00     b7e0c18c77c64531bc3ea141bb31c4b0        0155c8da756b7157310035490459fd92 3       False   EFI GPT Disk    0xee00ffff      N/A
* 0x40321c7d    00-00-00-00     b7e0c18c77c64531bc3ea141bb31c4b0        0155c8da756b7157310035490459fd92 4       False   EFI GPT Disk    0x5500aaaa      N/A
* 0x413b2a8f    70-ee-c6-5d     7160449e42739f9f50c53daa616453e5        8de60717b8f12625287821ece02c49ec 4       False   EFI GPT Disk    0x7f02fed9      N/A
* 0x4394e714    07-00-30-d2     4b35f7184c02aadd6fbc5765a341fd57        18795ec6089b77458d908ef7609cfbb0 4       False   Microsoft MBR,Dynamic Disk      0x7aa42 N/A
* 0x4394e71c    07-00-57-a9     6d76b6c213a1f4d1f5ca6b084fe0c485        f94c3e2d41b4e48a517777cf00c12383 4       False   Microsoft MBR,Dynamic Disk      0x12d3cc        N/A
* 0x43c43ecb    0f-c5-cb-65     f7188caf2fdf1db6a2cb47a553fa5a81        5ed560d85f47d9139ae8ccd7f02320f5 1       False   Microsoft MBR,Dynamic Disk      0x3cc20862      N/A
* 0x44ee6389    26-6c-72-5c     170103c22f2cc91cab85e9316604ce4c        ff55d9a08d6bc2d27acfaab83a8996e8 2       False   EFI GPT Disk    0x685ccec8      N/A
* 0x49c00290    1f-6f-f9-49     784e98306f06e4a1ee7b1ce8c93f2feb        95c42ff71d6c6ea22bc496d99d379fdc 4       False   Microsoft MBR,Dynamic Disk      0xcc67017e      N/A
* 0x4e2d60fe    f2-a2-c4-cc     cf1204684f227b1da56cbbf50f0ec69b        d0f83dfe8327b872b90456550ac8829e 3       False   EFI GPT Disk    0x6aa9d382      N/A
* 0x4e6ffdeb    71-f1-ee-dc     63eb827e6b3a14ea9f21b74fce9bbe25        f4fa204516aaec5643d928d724b73f8f 1       False   Microsoft MBR,Dynamic Disk      0xa8b53209      N/A
* 0x4e8e1eab    5d-b6-fa-62     0632f91c549980975895179323bc7a4e        516946203ce7adcb32be5909dbb279a4 2       False   EFI GPT Disk    0x9553ddf5      N/A
* 0x4e96754a    71-f1-ee-dc     63eb827e6b3a14ea9f21b74fce9bbe25        f4fa204516aaec5643d928d724b73f8f 1       False   Microsoft MBR,Dynamic Disk      0xa8b53209      N/A
* 0x4f0b94e0    00-00-00-00     e2ff817112306721d2d2cd386d36a7b5        93521895a5750b4c0b66a13a1d180a97 1       False   EFI GPT Disk    0xffffeecc      N/A
* 0x4f98a4a4    00-00-00-00     bac4114d521069783ab74ab89f551374        67cd2f4f28668a09113e1ccd618c761d 4       False   EFI GPT Disk    0xffffcc88      N/A
* 0x50489eff    0c-7d-27-75     d9c3ef896f307302f9e38cdba00f3eaf        48bc10a8f76aea3d1fe9cb8780c99c61 3       False   Microsoft MBR,Dynamic Disk      0xfe486ad0      N/A
* 0x50862d26    ab-c8-6b-4c     5ec891252b2dc8f653981924a892ff4c        e8cd63c17a5bd307ac69941fd074fe9b 2       False   EFI GPT Disk    0xde9b55ba      N/A
* 0x5088613c    8c-45-2e-d5     ccaa422fe93bd1882b03e6ce9e989267        b03ec0544a029e6b7fabaa00724fd467 2       False   EFI GPT Disk    0x64d4739f      N/A
* 0x50b07376    12-50-af-09     a146b9c3b7ca7876e60f828cb28f0b4a        5c5194d51d9585f789e8ac17fc8059ca 3       False   Microsoft MBR,Dynamic Disk      0x8842109a      N/A
* 0x50f330dc    ae-c9-05-d9     8e805c2c0213aa0a807893e138c6838b        e4374a88e6bb6ac89078a38763fb8984 3       False   EFI GPT Disk    0x46370bdf      N/A
* 0x511e5644    2f-85-75-af     ca26a0066fb074a1adb82fe4b8232b4e        4cc78173cdbeb82e76e2511327410dc6 3       False   Microsoft MBR,Dynamic Disk      0xf29e78d2      N/A
* 0x517ec560    63-1e-77-09     54eca0c02372bb6b0df5e39c193c834a        8597361a421a0cc522bb3c72827daa6c 3       False   EFI GPT Disk    0x1362317       N/A
* 0x51824adb    e5-d9-53-83     8ae54670c3fcc88bdb00666b16e58221        694038d0d340da8803e95a88e6957e8f 2       False   Microsoft MBR,Dynamic Disk      0xe99e7333      N/A
* 0x5199c39f    e7-66-15-0e     b2a30b7f959ad2c041470a6a8ec47522        2825707552c33f8a6cc096716f15509a 3       False   EFI GPT Disk    0x3fc83e21      N/A
* 0x51b4b154    c0-7a-e6-c9     df009420a3d73ee24619a35bd3ae9d0e        93a4b35146b0ce2797f22cf1770492ed 3       False   Microsoft MBR,Dynamic Disk      0x5bc4ba2a      N/A
* 0x5212f8ae    c6-d5-a0-75     a80ef0da9ab9ca5af78101ddcee9e692        63b952d3ecf06e2cd11c9a33d942ccb4 3       False   Microsoft MBR,Dynamic Disk      0x39fcb519      N/A
* 0x523c5df8    78-e4-b9-60     5d1e7f5008d8fe00b6067ce7c9373eb7        8deabb6671adc6f4cb8142e84b3683ed 1       False   EFI GPT Disk    0x6e510e3       N/A
* 0x5284bb39    c6-d5-a0-75     d211685e20af1fe9c1815e8fcb35bd96        eeea7931d3de463397f98f3fc9cc7985 3       False   Microsoft MBR,Dynamic Disk      0x39fcb519      N/A
* 0x529b5832    49-95-cc-ab     989c4c52d80c3d9c788215f68fde480a        5c7bc601cffea46efbfd8ad38ab29ead 2       False   Microsoft MBR,Dynamic Disk      0xd6f55d8c      N/A
* 0x52b90a90    49-95-cc-ab     989c4c52d80c3d9c788215f68fde480a        5c7bc601cffea46efbfd8ad38ab29ead 2       False   Microsoft MBR,Dynamic Disk      0xd6f55d8c      N/A
* 0x530f9df2    ad-72-57-ad     4fa55816d72a26b464016a1e4d84f7b4        76ca8df8b9ce13cacb92d32770d45634 3       False   Microsoft MBR,Dynamic Disk      0x7085b205      N/A
* 0x55aa4082    44-c8-5d-43     fa7e23dcd09ff40e6b0376af8f805732        c04bd72f84f633f5a5bec8afed758094 4       False   EFI GPT Disk    0x698f694e      N/A
* 0x5606c198    44-c8-5d-43     7fca225a49619afcdc6f311ed21e0605        029233b980aeac80142088a7fe37f0df 4       False   EFI GPT Disk    0x698f694e      N/A
* 0x5627d4f1    44-c8-5d-43     ac23c62a4b4aa227944290d9a76b0fd9        a158c342a0fbc9e9757a16ea60c47d4c 4       False   EFI GPT Disk    0x698f694e      N/A
* 0x563a4179    79-51-ed-fa     4ab1a61a96adc73ad041fe1a07f8df74        707a79caef2e2db47409ed052b249c2e 4       False   EFI GPT Disk    0xfdf6ed76      N/A
* 0x56830d4b    9e-fc-80-cf     25be5d453b5bce8e55704e72411b49c2        3be890c97494335f8401a89b4dccc52b 3       False   Microsoft MBR,Dynamic Disk      0xfb543b91      N/A
* 0x56fc4be8    49-a9-d8-69     0caa719e79eb0c122fc0357a51c11683        86623d75d89051daad0e12d587d1ddae 3       False   EFI GPT Disk    0xa79e0aca      N/A
* 0x572f4b36    ea-31-ee-fe     3f1c49a74a716b96f1cf44a20f1b0ac2        a090ae80d3b1e2f978daf34c11831c4a 4       False   EFI GPT Disk    0x2c1ad594      N/A
* 0x57e232bc    55-8f-7d-83     b5392da48901811e82c718999a2c48cf        238ce1c6cf58ac5b38188481347feaa2 1       False   EFI GPT Disk    0xafc6c88b      N/A
* 0x588b7b7b    9e-7b-57-c6     0c8ebfdc4e2b73e2e01f72b7d0a37ce4        ae29330517b9861292894986fc371cbf 3       False   EFI GPT Disk    0xfd12eb58      N/A
* 0x58a6e6ac    98-6a-22-ad     13e8334a4e609872f1ad42660ffe7122        002270ef5949e573be217be16e2a8532 2       False   EFI GPT Disk    0x3b958ae4      N/A
* 0x58a7dae0    cc-55-d4-71     5ae0382b263e643d938d7b31c1779b3d        8adccd9bd31bd3e6fc5484b89ac5a109 2       False   EFI GPT Disk    0x605c478a      N/A
* 0x58bcb81f    50-09-05-c6     f58145760a20969b0dd39b920460bf18        04f3d6a5d64f77e8cfdb96626978fe16 4       False   EFI GPT Disk    0xb5d43fe4      N/A
* 0x58daf2f1    3d-9d-1e-d1     e53a4dd285413e1eeaddd753c28e8891        d78d17895788637f7d4662027a673298 4       False   Microsoft MBR,Dynamic Disk      0x3ef755e3      N/A
* 0x58ea2752    f9-88-d0-35     55c0b9f408f7f5a73a6cb274b138cad9        2113c947f0fbe194a4075e006bdd47e5 4       False   EFI GPT Disk    0x44b353b7      N/A
* 0x5967e375    b4-f1-cc-61     059f6c2c5bc3335e618c1519ded9be96        086419d76fcc5cb2105df9cb64e1586c 4       False   Microsoft MBR,Dynamic Disk      0x6459d4dd      N/A
* 0x5c314545    00-73-00-74     8ba9cd8bc97a1312af3d207474e55867        1e901e3c5de99038cbe2d490bcbbb642 2       False   Microsoft MBR,Dynamic Disk      0x246f09f6      N/A
* 0x5d6b156a    eb-d4-a4-73     fc7be888ef50aaf72f4e507a8e648c6a        c25b99bb4810c6eab52897db780c2beb 2       False   EFI GPT Disk    0xcd0cfaf2      N/A
* 0x5d6b1e66    eb-d4-a4-73     fc7be888ef50aaf72f4e507a8e648c6a        c25b99bb4810c6eab52897db780c2beb 2       False   EFI GPT Disk    0xcd0cfaf2      N/A
* 0x5db77b30    1f-6f-f9-49     784e98306f06e4a1ee7b1ce8c93f2feb        95c42ff71d6c6ea22bc496d99d379fdc 4       False   Microsoft MBR,Dynamic Disk      0xcc67017e      N/A
* 0x5dedda7d    64-85-ac-c0     a764d3ae8c061891167db90767eeb0e7        7d6c3e9fcff375561ce47187a5185f6c 2       False   Microsoft MBR,Dynamic Disk      0x7fad26bd      N/A
* 0x5df4bce0    47-c8-d5-e5     6a1434b15fc8e27fcab952f8f5ebca18        faacf1d02f3aa0f3d6b5d85774a61d09 3       False   Microsoft MBR,Dynamic Disk      0x857edecd      N/A
* 0x5dfa3032    00-d4-71-64     71d753338a56b6a42ccb6f943e49414b        a63cf8b0f89121b03312823db540dae6 4       False   EFI GPT Disk    0xde891c0e      N/A
* 0x5e153c10    47-c8-d5-e5     6a1434b15fc8e27fcab952f8f5ebca18        faacf1d02f3aa0f3d6b5d85774a61d09 3       False   Microsoft MBR,Dynamic Disk      0x857edecd      N/A
* 0x5e3ff861    75-ed-f7-d1     a711f4beb30018578aa402a4b2e35225        5bc79e4242216de8c6bbb0f9c30d0c22 2       False   EFI GPT Disk    0xf508dff0      N/A
* 0x604c33d6    7e-f7-2a-09     b38d90a174050c50322ac54f501bb5a0        79ecc88fa94795de845d1c1944780ddc 2       False   EFI GPT Disk    0x6d996e1a      N/A
* 0x6105478e    af-7d-41-45     a2455f82e63c282938d99f4a7949be75        48f5cfa3cce362d63ecf37a01d2acea4 4       False   Microsoft MBR,Dynamic Disk      0xe2ae24d2      N/A
* 0x616987da    fa-80-f3-c2     b99e34a35f663fed2406925f2e331f1f        a71ea0a9019b758e2c0081cf1266f304 2       False   Microsoft MBR,Dynamic Disk      0x226a2ca5      N/A
* 0x63208b20    78-e0-3b-ef     af87f49343fbf013ed25a9f0708731fa        4924c0d6b82a7f70b023dd27fd9528da 4       False   Microsoft MBR,Dynamic Disk      0x5bbe53e1      N/A
* 0x63208e50    78-e0-3b-ef     82426a2528ca8a3fed7a1febf751a5f5        72d5668710166daa54e04075001e3e37 4       False   Microsoft MBR,Dynamic Disk      0x5bbe53e1      N/A
* 0x6beb82fe    e1-b9-48-1d     37d67093b6dd9cf48d1574089f120365        583db40efa6b07cc077a55a1f0056b97 3       False   EFI GPT Disk    0xec7546c8      N/A
* 0x6cb246a9    55-b0-7c-55     4bb3490a9f698ad7a06aade0a75440e9        297ff8ceac3b443d230ae2d4c0e8bd84 4       False   Microsoft MBR,Dynamic Disk      0xb74200c0      N/A
* 0x6f6b4d55    92-88-01-5e     c8c0504c36f5d36957faf428c707080d        117c9e6ec9f39b5e4b5a24a6f387b0ee 4       False   Microsoft MBR,Dynamic Disk      0xbfc21758      N/A
* 0x7218fa3b    bd-12-eb-88     bf6016770b440b180bfec4d8a4736977        56ca56badfa89edc858aa40fa0a0452c 2       False   Microsoft MBR,Dynamic Disk      0x749a1073      N/A
* 0x72a9db77    5f-5d-be-87     fd785248816982afec3322e1fed3eda4        b0855419ae415ac6f07415072dd3257a 3       False   EFI GPT Disk    0xeca181f3      N/A
* 0x748a63a1    00-ff-ff-ff     5e5e610d626727d8a427fe3080af727b        2dc52d81123d57c9d50760e5e1e2c608 2       False   EFI GPT Disk    0x33009933      N/A
* 0x74f78fb0    e5-ff-5e-68     012cf58b8765415d4ba84ea8c714966b        3cef7beaf92f038e8f22d4fd3df98b3a 4       False   Microsoft MBR,Dynamic Disk      0xffcaa954      N/A
* 0x76a93f0f    ff-ff-e8-50     fc2ec681682a13a971d56a3fe031790f        e5ffe0aee9d5448e4583b4522535517e 2       False   EFI GPT Disk    0xffb6d663      N/A
* 0x7a59d1f5    00-00-22-55     a4c0938c85fee0e9d08dba72c89b49f2        7c8f6ae68c9d281a1b3c531417a3f1f6 4       False   EFI GPT Disk    0x2200ddbb      N/A
* 0x7a92a275    80-ff-80-80     e7fe0de8dc202607351e23fdfba15d87        c294766db987c4d4bfdefa5c50478488 1       True    Microsoft MBR,Dynamic Disk      0x8000000       N/A
* 0x7e7ce3e3    dc-41-64-21     0f94c791288a9275c4c2658fdd64f258        6d9510b3e13429ba03cacc4693c96e27 4       False   Microsoft MBR,Dynamic Disk      0x876c758       N/A
* 0x7ef470bf    36-69-37-67     e87be597cda1c4dd5ba67ef4180f234d        a2470bbaee5eca8f21f3629c89cdf0e8 4       False   Microsoft MBR,Dynamic Disk      0x876c758       N/A
```


- vol.exe -f .\OtterCTF.vmem windows.mbrscan.MBRScan | findstr "Bootcode"
```
D:\Forensic\G140A006\VolatilityWorkbench>.\vol.exe -f .\OtterCTF.vmem windows.mbrscan.MBRScan | findstr "Bootcode"
Potential MBR at Physical OffsetPDB scanDisk Signature  Bootcode MD5    Full MBR MD5    PartitionIndex   Bootable        PartitionType   SectorInSize    Disasm
```

- vol.exe -f .\OtterCTF.vmem windows.mbrscan.MBRScan | findstr "Physical"
```
D:\Forensic\G140A006\VolatilityWorkbench>.\vol.exe -f .\OtterCTF.vmem windows.mbrscan.MBRScan | findstr "Physical"
Potential MBR at Physical OffsetPDB scanDisk Signature  Bootcode MD5    Full MBR MD5    PartitionIndex   Bootable        PartitionType   SectorInSize    Disasm
```

# windows.mbrscan.MBRScan 分析

## 1. Plugin 功能說明

`windows.mbrscan.MBRScan` 用來掃描記憶體中的 MBR（Master Boot Record）結構。

MBR 是磁碟開機區的重要資料，主要包含：

* Boot code
* Disk Signature
* Partition Table
* Bootable 狀態
* Partition Type

此 Plugin 主要用來檢查是否存在 MBR Bootkit、開機區感染或異常的磁碟啟動紀錄。

---

## 2. Plugin 欄位說明

| 欄位                                 | 說明                  |
| ---------------------------------- | ------------------- |
| `Potential MBR at Physical Offset` | 可能的 MBR 在記憶體中的實體位址  |
| `Disk Signature`                   | 磁碟簽章                |
| `Bootcode MD5`                     | Boot code 的 MD5 雜湊值 |
| `Full MBR MD5`                     | 完整 MBR 的 MD5 雜湊值    |
| `PartitionIndex`                   | Partition 編號        |
| `Bootable`                         | 是否為可開機分割區           |
| `PartitionType`                    | 分割區類型               |
| `SectorInSize`                     | 分割區大小或 Sector 相關資訊  |
| `Disasm`                           | Boot code 反組譯結果     |

---

## 3. 執行指令

```bash
.\vol.exe -f .\OtterCTF.vmem windows.mbrscan.MBRScan
```

由於輸出內容很多，因此使用 `findstr` 篩選重點：

```bash
.\vol.exe -f .\OtterCTF.vmem windows.mbrscan.MBRScan | findstr "Potential MBR"
.\vol.exe -f .\OtterCTF.vmem windows.mbrscan.MBRScan | findstr "Disk Signature"
.\vol.exe -f .\OtterCTF.vmem windows.mbrscan.MBRScan | findstr "Bootcode"
.\vol.exe -f .\OtterCTF.vmem windows.mbrscan.MBRScan | findstr "Physical"
```

---

## 4. 結果重點

本次 `MBRScan` 掃描到大量 Potential MBR 紀錄，常見類型包含：

```text
Microsoft MBR, Dynamic Disk
EFI GPT Disk
```

其中可注意的 Bootable 紀錄如下：

```text
0x1d2bd365    Bootable=True    Microsoft MBR,Dynamic Disk
0x7a92a275    Bootable=True    Microsoft MBR,Dynamic Disk
```

另外，多數紀錄的 `Disasm` 欄位為：

```text
N/A
```

---

## 5. 分析結果

本次 `MBRScan` 雖然出現大量 Potential MBR，但多數紀錄屬於：

```text
Microsoft MBR, Dynamic Disk
EFI GPT Disk
```

這些結果本身不一定代表惡意行為。

此外，輸出中沒有看到明確可疑字串，也沒有出現明顯 Bootkit 相關反組譯內容。

`Bootcode` 與 `Physical` 篩選結果主要只顯示欄位標題，沒有額外可疑內容，代表目前沒有明顯可疑 Boot code 證據。

---

## 6. 鑑識判斷

本次 `MBRScan` 的用途主要是確認是否存在 MBR Bootkit 或開機區感染。

根據目前結果：

```text
1. 有掃描到多筆 Potential MBR
2. 多數類型為 Microsoft MBR, Dynamic Disk 或 EFI GPT Disk
3. 部分紀錄 Bootable=True
4. Disasm 多為 N/A
5. 未發現明顯可疑 Bootkit 字串或異常 Boot code
```

因此，目前沒有足夠證據顯示本案存在 MBR Bootkit 或開機區感染。

---

## 7. 結論

`windows.mbrscan.MBRScan` 在本案中屬於輔助檢查，用來排除 MBR 層級感染。

本次結果雖然出現大量 Potential MBR 紀錄，但未發現明顯異常的 Boot code、Bootkit 反組譯內容或可疑字串。

因此，本案目前較不像 MBR Bootkit 感染，而是較符合使用者執行可疑程式後造成檔案加密的情境。

目前主要攻擊線仍然是：

```text
BitTorrent 下載活動
↓
Rick And Morty season 1 download.exe
↓
Temp\RarSFX0\vmware-tray.exe
↓
檔案加密
↓
READ_IT.txt 提示檔
```
