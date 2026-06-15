# 測試內

- vol.exe -f .\OtterCTF.vmem windows.malfind.Malfind
- 
```
D:\Forensic\G140A006\VolatilityWorkbench>.\vol.exe -f .\OtterCTF.vmem windows.malfind.Malfind
Volatility 3 Framework 2.5.0
Progress:  100.00               PDB scanning finished
PID     Process Start VPN       End VPN Tag     Protection      CommitCharge    PrivateMemory   File output      Hexdump Disasm

2136    WmiPrvSE.exe    0x1170000       0x11effff       VadS    PAGE_EXECUTE_READWRITE  2       1Disabled
00 00 00 00 00 00 00 00 ........
9d 88 3b aa 5a 4c 00 01 ..;.ZL..
ee ff ee ff 00 00 00 00 ........
28 01 17 01 00 00 00 00 (.......
28 01 17 01 00 00 00 00 (.......
00 00 17 01 00 00 00 00 ........
00 00 17 01 00 00 00 00 ........
80 00 00 00 00 00 00 00 ........
0x1170000:      add     byte ptr [rax], al
0x1170002:      add     byte ptr [rax], al
0x1170004:      add     byte ptr [rax], al
0x1170006:      add     byte ptr [rax], al
0x1170008:      popfq
0x1170009:      mov     byte ptr [rbx], bh
0x117000b:      stosb   byte ptr [rdi], al
0x117000c:      pop     rdx
0x117000d:      add     byte ptr [rcx], r8b
0x1170010:      out     dx, al
2136    WmiPrvSE.exe    0x1850000       0x18cffff       VadS    PAGE_EXECUTE_READWRITE  2       1Disabled
00 00 00 00 00 00 00 00 ........
06 87 bd 8e 5d 19 00 01 ....]...
ee ff ee ff 00 00 00 00 ........
28 01 85 01 00 00 00 00 (.......
28 01 85 01 00 00 00 00 (.......
00 00 85 01 00 00 00 00 ........
00 00 85 01 00 00 00 00 ........
80 00 00 00 00 00 00 00 ........
0x1850000:      add     byte ptr [rax], al
0x1850002:      add     byte ptr [rax], al
0x1850004:      add     byte ptr [rax], al
0x1850006:      add     byte ptr [rax], al
2728    explorer.exe    0x1cb0000       0x1cbffff       VadS    PAGE_EXECUTE_READWRITE  16      1Disabled
41 ba 80 00 00 00 48 b8 A.....H.
38 a1 9c ff fe 07 00 00 8.......
48 ff 20 90 41 ba 81 00 H...A...
00 00 48 b8 38 a1 9c ff ..H.8...
fe 07 00 00 48 ff 20 90 ....H...
41 ba 82 00 00 00 48 b8 A.....H.
38 a1 9c ff fe 07 00 00 8.......
48 ff 20 90 41 ba 83 00 H...A...
0x1cb0000:      mov     r10d, 0x80
0x1cb0006:      movabs  rax, 0x7feff9ca138
0x1cb0010:      jmp     qword ptr [rax]
0x1cb0013:      nop
0x1cb0014:      mov     r10d, 0x81
0x1cb001a:      movabs  rax, 0x7feff9ca138
0x1cb0024:      jmp     qword ptr [rax]
0x1cb0027:      nop
0x1cb0028:      mov     r10d, 0x82
0x1cb002e:      movabs  rax, 0x7feff9ca138
0x1cb0038:      jmp     qword ptr [rax]
0x1cb003b:      nop
2728    explorer.exe    0x3c30000       0x3c30fff       VadS    PAGE_EXECUTE_READWRITE  1       1Disabled
00 00 00 00 00 00 00 00 ........
00 00 00 00 00 00 00 00 ........
00 00 00 00 00 00 00 00 ........
00 00 00 00 00 00 00 00 ........
00 00 c3 03 00 00 00 00 ........
00 00 00 00 00 00 00 00 ........
00 00 00 00 00 00 00 00 ........
00 00 00 00 00 00 00 00 ........
0x3c30000:      add     byte ptr [rax], al
0x3c30002:      add     byte ptr [rax], al
0x3c30004:      add     byte ptr [rax], al
0x3c30006:      add     byte ptr [rax], al
0x3c30008:      add     byte ptr [rax], al
0x3c3000a:      add     byte ptr [rax], al
0x3c3000c:      add     byte ptr [rax], al
0x3c3000e:      add     byte ptr [rax], al
0x3c30010:      add     byte ptr [rax], al
0x3c30012:      add     byte ptr [rax], al
0x3c30014:      add     byte ptr [rax], al
0x3c30016:      add     byte ptr [rax], al
0x3c30018:      add     byte ptr [rax], al
0x3c3001a:      add     byte ptr [rax], al
0x3c3001c:      add     byte ptr [rax], al
0x3c3001e:      add     byte ptr [rax], al
0x3c30020:      add     byte ptr [rax], al
0x3c30022:      ret
0x3c30023:      add     eax, dword ptr [rax]
0x3c30025:      add     byte ptr [rax], al
0x3c30027:      add     byte ptr [rax], al
0x3c30029:      add     byte ptr [rax], al
0x3c3002b:      add     byte ptr [rax], al
0x3c3002d:      add     byte ptr [rax], al
0x3c3002f:      add     byte ptr [rax], al
0x3c30031:      add     byte ptr [rax], al
0x3c30033:      add     byte ptr [rax], al
0x3c30035:      add     byte ptr [rax], al
0x3c30037:      add     byte ptr [rax], al
0x3c30039:      add     byte ptr [rax], al
0x3c3003b:      add     byte ptr [rax], al
0x3c3003d:      add     byte ptr [rax], al
2836    BitTorrent.exe  0x5730000       0x5730fff       VadS    PAGE_EXECUTE_READWRITE  1       1Disabled
00 00 00 00 00 00 00 00 ........
00 00 00 00 00 00 00 00 ........
00 00 73 05 00 00 00 00 ..s.....
00 00 00 00 00 00 00 00 ........
10 00 73 05 00 00 00 00 ..s.....
00 00 00 00 00 00 00 00 ........
20 00 73 05 00 00 00 00 ..s.....
00 00 00 00 00 00 00 00 ........
0x5730000:      add     byte ptr [eax], al
0x5730002:      add     byte ptr [eax], al
0x5730004:      add     byte ptr [eax], al
0x5730006:      add     byte ptr [eax], al
0x5730008:      add     byte ptr [eax], al
0x573000a:      add     byte ptr [eax], al
0x573000c:      add     byte ptr [eax], al
0x573000e:      add     byte ptr [eax], al
0x5730010:      add     byte ptr [eax], al
0x5730012:      jae     0x5730019
0x5730014:      add     byte ptr [eax], al
0x5730016:      add     byte ptr [eax], al
0x5730018:      add     byte ptr [eax], al
0x573001a:      add     byte ptr [eax], al
0x573001c:      add     byte ptr [eax], al
0x573001e:      add     byte ptr [eax], al
0x5730020:      adc     byte ptr [eax], al
0x5730022:      jae     0x5730029
0x5730024:      add     byte ptr [eax], al
0x5730026:      add     byte ptr [eax], al
0x5730028:      add     byte ptr [eax], al
0x573002a:      add     byte ptr [eax], al
0x573002c:      add     byte ptr [eax], al
0x573002e:      add     byte ptr [eax], al
0x5730030:      and     byte ptr [eax], al
0x5730032:      jae     0x5730039
0x5730034:      add     byte ptr [eax], al
0x5730036:      add     byte ptr [eax], al
0x5730038:      add     byte ptr [eax], al
0x573003a:      add     byte ptr [eax], al
0x573003c:      add     byte ptr [eax], al
0x573003e:      add     byte ptr [eax], al
724     PresentationFo  0x5c0000        0x63ffff        VadS    PAGE_EXECUTE_READWRITE  2       1Disabled
00 00 00 00 00 00 00 00 ........
95 a4 16 c2 d2 96 00 01 ........
ee ff ee ff 00 00 00 00 ........
28 01 5c 00 00 00 00 00 (.\.....
28 01 5c 00 00 00 00 00 (.\.....
00 00 5c 00 00 00 00 00 ..\.....
00 00 5c 00 00 00 00 00 ..\.....
80 00 00 00 00 00 00 00 ........
0x5c0000:       add     byte ptr [rax], al
0x5c0002:       add     byte ptr [rax], al
0x5c0004:       add     byte ptr [rax], al
0x5c0006:       add     byte ptr [rax], al
0x5c0008:       xchg    ebp, eax
0x5c0009:       movsb   byte ptr [rdi], byte ptr [rsi]
724     PresentationFo  0xa10000        0xa8ffff        VadS    PAGE_EXECUTE_READWRITE  37      1Disabled
00 00 00 00 00 00 00 00 ........
1f 9a 5b bc e5 93 00 01 ..[.....
ee ff ee ff 00 00 00 00 ........
28 01 a1 00 00 00 00 00 (.......
28 01 a1 00 00 00 00 00 (.......
00 00 a1 00 00 00 00 00 ........
00 00 a1 00 00 00 00 00 ........
80 00 00 00 00 00 00 00 ........
0xa10000:       add     byte ptr [rax], al
0xa10002:       add     byte ptr [rax], al
0xa10004:       add     byte ptr [rax], al
0xa10006:       add     byte ptr [rax], al
724     PresentationFo  0x7fffff10000   0x7fffff1ffff   VadS    PAGE_EXECUTE_READWRITE  1       1Disabled
00 00 00 00 00 00 00 00 ........
78 0d 00 00 00 00 00 00 x.......
0e 00 00 00 49 c7 c2 00 ....I...
00 00 00 48 b8 e0 19 14 ...H....
f9 fe 07 00 00 ff e0 49 .......I
c7 c2 01 00 00 00 48 b8 ......H.
e0 19 14 f9 fe 07 00 00 ........
ff e0 49 c7 c2 02 00 00 ..I.....
0x7fffff10000:  add     byte ptr [rax], al
0x7fffff10002:  add     byte ptr [rax], al
0x7fffff10004:  add     byte ptr [rax], al
0x7fffff10006:  add     byte ptr [rax], al
0x7fffff10008:  js      0x7fffff10017
0x7fffff1000a:  add     byte ptr [rax], al
0x7fffff1000c:  add     byte ptr [rax], al
0x7fffff1000e:  add     byte ptr [rax], al
724     PresentationFo  0x7fffff20000   0x7fffffaffff   VadS    PAGE_EXECUTE_READWRITE  1       1Disabled
d8 ff ff ff ff ff ff ff ........
08 00 00 00 00 00 00 00 ........
01 00 00 00 00 00 00 00 ........
00 00 08 01 38 00 00 00 ....8...
15 00 0e 00 0e 00 00 00 ........
f8 73 f3 f7 fe 07 00 00 .s......
00 10 b0 f7 fe 07 00 00 ........
a8 ed b3 f7 fe 07 00 00 ........
0x7fffff20000:  fdivr   st(7)
412     mscorsvw.exe    0xba0000        0xbdffff        VadS    PAGE_EXECUTE_READWRITE  1       1Disabled
9e 17 1d ae b0 f0 00 01 ........
ee ff ee ff 00 00 00 00 ........
a8 00 ba 00 a8 00 ba 00 ........
00 00 ba 00 00 00 ba 00 ........
40 00 00 00 88 05 ba 00 @.......
00 00 be 00 3f 00 00 00 ....?...
01 00 00 00 00 00 00 00 ........
f0 0f ba 00 f0 0f ba 00 ........
0xba0000:       sahf
0xba0001:       pop     ss
0xba0002:       sbb     eax, 0xf0b0ae
0xba0007:       add     esi, ebp
412     mscorsvw.exe    0x16a0000       0x16dffff       VadS    PAGE_EXECUTE_READWRITE  1       1Disabled
87 79 5b b7 e7 b6 00 01 .y[.....
ee ff ee ff 00 00 00 00 ........
a8 00 6a 01 a8 00 6a 01 ..j...j.
00 00 6a 01 00 00 6a 01 ..j...j.
40 00 00 00 88 05 6a 01 @.....j.
00 00 6e 01 3f 00 00 00 ..n.?...
01 00 00 00 00 00 00 00 ........
f0 0f 6a 01 f0 0f 6a 01 ..j...j.
0x16a0000:      xchg    dword ptr [ecx + 0x5b], edi
0x16a0003:      mov     bh, 0xe7
0x16a0005:      mov     dh, 0
0x16a0007:      add     esi, ebp
3124    mscorsvw.exe    0xaf0000        0xb6ffff        VadS    PAGE_EXECUTE_READWRITE  2       1Disabled
00 00 00 00 00 00 00 00 ........
79 38 fd bf bb 0c 00 01 y8......
ee ff ee ff 00 00 00 00 ........
28 01 af 00 00 00 00 00 (.......
28 01 af 00 00 00 00 00 (.......
00 00 af 00 00 00 00 00 ........
00 00 af 00 00 00 00 00 ........
80 00 00 00 00 00 00 00 ........
0xaf0000:       add     byte ptr [rax], al
0xaf0002:       add     byte ptr [rax], al
0xaf0004:       add     byte ptr [rax], al
0xaf0006:       add     byte ptr [rax], al
0xaf0008:       jns     0xaf0042
0xaf000a:       std
0xaf000b:       mov     edi, 0x1000cbb
0xaf0010:       out     dx, al
3124    mscorsvw.exe    0x1330000       0x13affff       VadS    PAGE_EXECUTE_READWRITE  2       1Disabled
00 00 00 00 00 00 00 00 ........
22 0a 9a cc 73 9b 00 01 "...s...
ee ff ee ff 00 00 00 00 ........
28 01 33 01 00 00 00 00 (.3.....
28 01 33 01 00 00 00 00 (.3.....
00 00 33 01 00 00 00 00 ..3.....
00 00 33 01 00 00 00 00 ..3.....
80 00 00 00 00 00 00 00 ........
0x1330000:      add     byte ptr [rax], al
0x1330002:      add     byte ptr [rax], al
0x1330004:      add     byte ptr [rax], al
0x1330006:      add     byte ptr [rax], al
0x1330008:      and     cl, byte ptr [rdx]
3196    svchost.exe     0x5d0000        0x60ffff        VadS    PAGE_EXECUTE_READWRITE  64      1Disabled
56 57 53 55 48 83 ec 28 VWSUH..(
48 8b e9 ff e2 48 83 c4 H....H..
28 5d 5b 5f 5e c3 00 00 (][_^...
00 00 00 00 00 00 00 00 ........
00 00 00 00 00 00 00 00 ........
00 00 00 00 00 00 00 00 ........
00 00 00 00 00 00 00 00 ........
00 00 00 00 00 00 00 00 ........
0x5d0000:       push    rsi
0x5d0001:       push    rdi
0x5d0002:       push    rbx
0x5d0003:       push    rbp
0x5d0004:       sub     rsp, 0x28
0x5d0008:       mov     rbp, rcx
0x5d000b:       jmp     rdx
0x5d000d:       add     rsp, 0x28
0x5d0011:       pop     rbp
0x5d0012:       pop     rbx
0x5d0013:       pop     rdi
0x5d0014:       pop     rsi
0x5d0015:       ret
0x5d0016:       add     byte ptr [rax], al
0x5d0018:       add     byte ptr [rax], al
0x5d001a:       add     byte ptr [rax], al
0x5d001c:       add     byte ptr [rax], al
0x5d001e:       add     byte ptr [rax], al
0x5d0020:       add     byte ptr [rax], al
0x5d0022:       add     byte ptr [rax], al
0x5d0024:       add     byte ptr [rax], al
0x5d0026:       add     byte ptr [rax], al
0x5d0028:       add     byte ptr [rax], al
0x5d002a:       add     byte ptr [rax], al
0x5d002c:       add     byte ptr [rax], al
0x5d002e:       add     byte ptr [rax], al
0x5d0030:       add     byte ptr [rax], al
0x5d0032:       add     byte ptr [rax], al
0x5d0034:       add     byte ptr [rax], al
0x5d0036:       add     byte ptr [rax], al
0x5d0038:       add     byte ptr [rax], al
0x5d003a:       add     byte ptr [rax], al
0x5d003c:       add     byte ptr [rax], al
0x5d003e:       add     byte ptr [rax], al
3196    svchost.exe     0x2440000       0x24bffff       VadS    PAGE_EXECUTE_READWRITE  128     1Disabled
20 00 00 00 e0 ff 07 00 ........
0c 00 00 00 01 00 05 00 ........
00 42 00 50 00 30 00 70 .B.P.0.p
00 60 00 00 00 00 00 00 .`......
48 8b 45 28 c7 00 00 00 H.E(....
00 00 c7 40 04 00 00 00 ...@....
00 48 8b 45 28 48 8d 40 .H.E(H.@
08 48 89 c2 48 8b 45 20 .H..H.E.
0x2440000:      and     byte ptr [rax], al
0x2440002:      add     byte ptr [rax], al
0x2440004:      loopne  0x2440005
3196    svchost.exe     0x4ce0000       0x4ddffff       VadS    PAGE_EXECUTE_READWRITE  256     1Disabled
20 00 00 00 e0 ff 0f 00 ........
0c 00 00 00 01 00 05 00 ........
00 42 00 50 00 30 00 70 .B.P.0.p
00 60 00 00 00 00 00 00 .`......
ba fc ff ff ff 03 55 20 ......U.
03 55 5c b9 04 00 1a 00 .U\.....
4c 8b c5 ff 95 e0 37 00 L.....7.
00 8b 4d 24 89 08 48 8d ..M$..H.
0x4ce0000:      and     byte ptr [rax], al
0x4ce0002:      add     byte ptr [rax], al
0x4ce0004:      loopne  0x4ce0005
0x4ce0006:      str     word ptr [rax + rax]
0x4ce000a:      add     byte ptr [rax], al
0x4ce000c:      add     dword ptr [rax], eax
0x4ce000e:      add     eax, 0x420000
0x4ce0013:      push    rax
0x4ce0014:      add     byte ptr [rax], dh
0x4ce0016:      add     byte ptr [rax], dh
3196    svchost.exe     0x4de0000       0x4edffff       VadS    PAGE_EXECUTE_READWRITE  256     1Disabled
00 00 00 00 00 00 00 00 ........
00 00 00 00 00 00 00 00 ........
00 00 00 00 00 00 00 00 ........
00 00 00 00 00 00 00 00 ........
00 00 00 00 00 00 00 00 ........
00 00 00 00 00 00 00 00 ........
00 00 00 00 00 00 00 00 ........
00 00 00 00 00 00 00 00 ........
0x4de0000:      add     byte ptr [rax], al
0x4de0002:      add     byte ptr [rax], al
0x4de0004:      add     byte ptr [rax], al
0x4de0006:      add     byte ptr [rax], al
0x4de0008:      add     byte ptr [rax], al
0x4de000a:      add     byte ptr [rax], al
0x4de000c:      add     byte ptr [rax], al
0x4de000e:      add     byte ptr [rax], al
0x4de0010:      add     byte ptr [rax], al
0x4de0012:      add     byte ptr [rax], al
0x4de0014:      add     byte ptr [rax], al
0x4de0016:      add     byte ptr [rax], al
0x4de0018:      add     byte ptr [rax], al
0x4de001a:      add     byte ptr [rax], al
0x4de001c:      add     byte ptr [rax], al
0x4de001e:      add     byte ptr [rax], al
0x4de0020:      add     byte ptr [rax], al
0x4de0022:      add     byte ptr [rax], al
0x4de0024:      add     byte ptr [rax], al
0x4de0026:      add     byte ptr [rax], al
0x4de0028:      add     byte ptr [rax], al
0x4de002a:      add     byte ptr [rax], al
0x4de002c:      add     byte ptr [rax], al
0x4de002e:      add     byte ptr [rax], al
0x4de0030:      add     byte ptr [rax], al
0x4de0032:      add     byte ptr [rax], al
0x4de0034:      add     byte ptr [rax], al
0x4de0036:      add     byte ptr [rax], al
0x4de0038:      add     byte ptr [rax], al
0x4de003a:      add     byte ptr [rax], al
0x4de003c:      add     byte ptr [rax], al
0x4de003e:      add     byte ptr [rax], al
4076    chrome.exe      0x47d0000       0x47d0fff       VadS    PAGE_EXECUTE_READWRITE  1       1Disabled
00 00 00 00 00 00 00 00 ........
00 00 00 00 00 00 00 00 ........
00 00 00 00 00 00 00 00 ........
00 00 00 00 00 00 00 00 ........
00 00 7d 04 00 00 00 00 ..}.....
00 00 00 00 00 00 00 00 ........
00 00 00 00 00 00 00 00 ........
00 00 00 00 00 00 00 00 ........
0x47d0000:      add     byte ptr [rax], al
0x47d0002:      add     byte ptr [rax], al
0x47d0004:      add     byte ptr [rax], al
0x47d0006:      add     byte ptr [rax], al
0x47d0008:      add     byte ptr [rax], al
0x47d000a:      add     byte ptr [rax], al
0x47d000c:      add     byte ptr [rax], al
0x47d000e:      add     byte ptr [rax], al
0x47d0010:      add     byte ptr [rax], al
0x47d0012:      add     byte ptr [rax], al
0x47d0014:      add     byte ptr [rax], al
0x47d0016:      add     byte ptr [rax], al
0x47d0018:      add     byte ptr [rax], al
0x47d001a:      add     byte ptr [rax], al
0x47d001c:      add     byte ptr [rax], al
0x47d001e:      add     byte ptr [rax], al
0x47d0020:      add     byte ptr [rax], al
0x47d0022:      jge     0x47d0028
0x47d0024:      add     byte ptr [rax], al
0x47d0026:      add     byte ptr [rax], al
0x47d0028:      add     byte ptr [rax], al
0x47d002a:      add     byte ptr [rax], al
0x47d002c:      add     byte ptr [rax], al
0x47d002e:      add     byte ptr [rax], al
0x47d0030:      add     byte ptr [rax], al
0x47d0032:      add     byte ptr [rax], al
0x47d0034:      add     byte ptr [rax], al
0x47d0036:      add     byte ptr [rax], al
0x47d0038:      add     byte ptr [rax], al
0x47d003a:      add     byte ptr [rax], al
0x47d003c:      add     byte ptr [rax], al
0x47d003e:      add     byte ptr [rax], al
3720    vmware-tray.ex  0x670000        0x6affff        VadS    PAGE_EXECUTE_READWRITE  1       1Disabled
9c 4c 5b ae 8c 8a 00 01 .L[.....
ee ff ee ff 00 00 00 00 ........
a8 00 67 00 a8 00 67 00 ..g...g.
00 00 67 00 00 00 67 00 ..g...g.
40 00 00 00 88 05 67 00 @.....g.
00 00 6b 00 3f 00 00 00 ..k.?...
01 00 00 00 00 00 00 00 ........
f0 0f 67 00 f0 0f 67 00 ..g...g.
0x670000:       pushfd
0x670001:       dec     esp
0x670002:       pop     ebx
0x670003:       scasb   al, byte ptr es:[edi]
0x670004:       mov     word ptr [edx - 0x11ff00], cs
0x67000a:       out     dx, al
0x67000b:       inc     dword ptr [eax]
0x67000d:       add     byte ptr [eax], al
0x67000f:       add     byte ptr [eax - 0x57ff9900], ch
0x670015:       add     byte ptr [edi], ah
0x670018:       add     byte ptr [eax], al
0x67001a:       add     byte ptr [bx + si], al
0x67001d:       add     byte ptr [edi], ah
0x670020:       inc     eax
0x670021:       add     byte ptr [eax], al
0x670023:       add     byte ptr [eax + 0x6705], cl
0x670029:       add     byte ptr [ebx], ch
0x67002c:       aas
0x67002d:       add     byte ptr [eax], al
0x67002f:       add     byte ptr [ecx], al
0x670031:       add     byte ptr [eax], al
0x670033:       add     byte ptr [eax], al
0x670035:       add     byte ptr [eax], al
0x670037:       add     al, dh
0x670039:       packuswb        mm0, qword ptr [eax]
3720    vmware-tray.ex  0x510000        0x54ffff        VadS    PAGE_EXECUTE_READWRITE  23      1Disabled
f0 26 16 8e 6a 2f 00 01 .&..j/..
ee ff ee ff 00 00 00 00 ........
a8 00 51 00 a8 00 51 00 ..Q...Q.
00 00 51 00 00 00 51 00 ..Q...Q.
40 00 00 00 88 05 51 00 @.....Q.
00 00 55 00 29 00 00 00 ..U.)...
01 00 00 00 00 00 00 00 ........
f0 6f 52 00 f0 6f 52 00 .oR..oR.
3720    vmware-tray.ex  0xc00000        0xc3ffff        VadS    PAGE_EXECUTE_READWRITE  1       1Disabled
33 d2 3c f0 3c cf 00 01 3.<.<...
ee ff ee ff 00 00 00 00 ........
a8 00 c0 00 a8 00 c0 00 ........
00 00 c0 00 00 00 c0 00 ........
40 00 00 00 88 05 c0 00 @.......
00 00 c4 00 3f 00 00 00 ....?...
01 00 00 00 00 00 00 00 ........
f0 0f c0 00 f0 0f c0 00 ........
0xc00000:       xor     edx, edx
0xc00002:       cmp     al, 0xf0
0xc00004:       cmp     al, 0xcf
0xc00006:       add     byte ptr [ecx], al
0xc00008:       out     dx, al
3720    vmware-tray.ex  0xa10000        0xa4ffff        VadS    PAGE_EXECUTE_READWRITE  1       1Disabled
12 d2 1f 89 e6 fd 00 01 ........
ee ff ee ff 00 00 00 00 ........
a8 00 a1 00 a8 00 a1 00 ........
00 00 a1 00 00 00 a1 00 ........
40 00 00 00 88 05 a1 00 @.......
00 00 a5 00 3f 00 00 00 ....?...
01 00 00 00 00 00 00 00 ........
f0 0f a1 00 f0 0f a1 00 ........
0xa10000:       adc     dl, dl
0xa10002:       pop     ds
0xa10003:       mov     esi, esp
0xa10005:       std
0xa10006:       add     byte ptr [ecx], al
0xa10008:       out     dx, al
3880    WebCompanionIn  0x1a0000        0x1dffff        VadS    PAGE_EXECUTE_READWRITE  1       1Disabled
1e 31 9d e7 c5 1d 00 01 .1......
ee ff ee ff 00 00 00 00 ........
a8 00 1a 00 a8 00 1a 00 ........
00 00 1a 00 00 00 1a 00 ........
40 00 00 00 88 05 1a 00 @.......
00 00 1e 00 3f 00 00 00 ....?...
01 00 00 00 00 00 00 00 ........
f0 0f 1a 00 f0 0f 1a 00 ........
0x1a0000:       push    ds
0x1a0001:       xor     dword ptr [ebp + 0x1dc5e7], ebx
0x1a0007:       add     esi, ebp
3880    WebCompanionIn  0x7c0000        0x7fffff        VadS    PAGE_EXECUTE_READWRITE  1       1Disabled
78 a5 7c 82 a4 72 00 01 x.|..r..
ee ff ee ff 00 00 00 00 ........
a8 00 7c 00 a8 00 7c 00 ..|...|.
00 00 7c 00 00 00 7c 00 ..|...|.
40 00 00 00 88 05 7c 00 @.....|.
00 00 80 00 3f 00 00 00 ....?...
01 00 00 00 00 00 00 00 ........
f0 0f 7c 00 f0 0f 7c 00 ..|...|.
0x7c0000:       js      0x7bffa7
0x7c0002:       jl      0x7bff86
0x7c0004:       movsb   byte ptr es:[edi], byte ptr [esi]
0x7c0005:       jb      0x7c0007
0x7c0007:       add     esi, ebp
3880    WebCompanionIn  0x7ef40000      0x7ef8ffff      VadS    PAGE_EXECUTE_READWRITE  1       1Disabled
ec ff ff ff 04 00 00 00 ........
01 00 00 00 00 00 08 01 ........
1c 00 00 00 15 00 0e 00 ........
0e 00 00 00 8c 07 24 73 ......$s
00 10 fd 72 5c 70 ff 72 ...r\p.r
2c 30 fd 72 00 00 00 00 ,0.r....
00 00 00 00 10 00 f3 7e .......~
1a 00 f3 7e 24 00 f3 7e ...~$..~
0x7ef40000:     in      al, dx
3880    WebCompanionIn  0x7ef30000      0x7ef3ffff      VadS    PAGE_EXECUTE_READWRITE  1       1Disabled
00 00 00 00 97 19 00 00 ........
00 00 00 00 0e 00 00 00 ........
68 00 00 00 00 e9 4a 09 h.....J.
89 81 68 01 00 00 00 e9 ..h.....
40 09 89 81 68 02 00 00 @...h...
00 e9 36 09 89 81 68 03 ..6...h.
00 00 00 e9 2c 09 89 81 ....,...
68 04 00 00 00 e9 22 09 h.....".
0x7ef30000:     add     byte ptr [eax], al
0x7ef30002:     add     byte ptr [eax], al
0x7ef30004:     xchg    edi, eax
0x7ef30005:     sbb     dword ptr [eax], eax
0x7ef30007:     add     byte ptr [eax], al
0x7ef30009:     add     byte ptr [eax], al
0x7ef3000b:     add     byte ptr [esi], cl
0x7ef3000d:     add     byte ptr [eax], al
0x7ef3000f:     add     byte ptr [eax], ch
0x7ef30012:     add     byte ptr [eax], al
0x7ef30014:     add     cl, ch
0x7ef30016:     dec     edx
0x7ef30017:     or      dword ptr [ecx + 0x16881], ecx
0x7ef3001d:     add     byte ptr [eax], al
0x7ef3001f:     jmp     0x7c0964
0x7ef30024:     push    2
0x7ef30029:     jmp     0x7c0964
0x7ef3002e:     push    3
0x7ef30033:     jmp     0x7c0964
0x7ef30038:     push    4
3496    Lavasoft.WCAss  0x580000        0x5fffff        VadS    PAGE_EXECUTE_READWRITE  2       1Disabled
00 00 00 00 00 00 00 00 ........
50 d6 10 d6 57 0e 00 01 P...W...
ee ff ee ff 00 00 00 00 ........
28 01 58 00 00 00 00 00 (.X.....
28 01 58 00 00 00 00 00 (.X.....
00 00 58 00 00 00 00 00 ..X.....
00 00 58 00 00 00 00 00 ..X.....
80 00 00 00 00 00 00 00 ........
0x580000:       add     byte ptr [rax], al
0x580002:       add     byte ptr [rax], al
0x580004:       add     byte ptr [rax], al
0x580006:       add     byte ptr [rax], al
0x580008:       push    rax
3496    Lavasoft.WCAss  0x660000        0x6dffff        VadS    PAGE_EXECUTE_READWRITE  50      1Disabled
00 00 00 00 00 00 00 00 ........
aa 32 b3 a9 8f 81 00 01 .2......
ee ff ee ff 00 00 00 00 ........
28 01 66 00 00 00 00 00 (.f.....
28 01 66 00 00 00 00 00 (.f.....
00 00 66 00 00 00 00 00 ..f.....
00 00 66 00 00 00 00 00 ..f.....
80 00 00 00 00 00 00 00 ........
0x660000:       add     byte ptr [rax], al
0x660002:       add     byte ptr [rax], al
0x660004:       add     byte ptr [rax], al
0x660006:       add     byte ptr [rax], al
0x660008:       stosb   byte ptr [rdi], al
0x660009:       xor     dh, byte ptr [rbx + 0x818fa9]
0x66000f:       add     esi, ebp
3496    Lavasoft.WCAss  0x7fffff10000   0x7fffff9ffff   VadS    PAGE_EXECUTE_READWRITE  1       1Disabled
d8 ff ff ff ff ff ff ff ........
08 00 00 00 00 00 00 00 ........
01 00 00 00 00 00 00 00 ........
00 00 08 01 38 00 00 00 ....8...
15 00 0e 00 0e 00 00 00 ........
f8 73 f3 f7 fe 07 00 00 .s......
00 10 b0 f7 fe 07 00 00 ........
a8 ed b3 f7 fe 07 00 00 ........
0x7fffff10000:  fdivr   st(7)
3496    Lavasoft.WCAss  0x7fffff00000   0x7fffff0ffff   VadS    PAGE_EXECUTE_READWRITE  1       1Disabled
00 00 00 00 00 00 00 00 ........
78 0d 00 00 00 00 00 00 x.......
0e 00 00 00 49 c7 c2 00 ....I...
00 00 00 48 b8 e0 19 14 ...H....
f9 fe 07 00 00 ff e0 49 .......I
c7 c2 01 00 00 00 48 b8 ......H.
e0 19 14 f9 fe 07 00 00 ........
ff e0 49 c7 c2 02 00 00 ..I.....
0x7fffff00000:  add     byte ptr [rax], al
0x7fffff00002:  add     byte ptr [rax], al
0x7fffff00004:  add     byte ptr [rax], al
0x7fffff00006:  add     byte ptr [rax], al
0x7fffff00008:  js      0x7fffff00017
0x7fffff0000a:  add     byte ptr [rax], al
0x7fffff0000c:  add     byte ptr [rax], al
0x7fffff0000e:  add     byte ptr [rax], al
3856    WebCompanion.e  0x1f0000        0x22ffff        VadS    PAGE_EXECUTE_READWRITE  1       1Disabled
2e 7f f0 8b 0a 71 00 01 .....q..
ee ff ee ff 00 00 00 00 ........
a8 00 1f 00 a8 00 1f 00 ........
00 00 1f 00 00 00 1f 00 ........
40 00 00 00 88 05 1f 00 @.......
00 00 23 00 3f 00 00 00 ..#.?...
01 00 00 00 00 00 00 00 ........
f0 0f 1f 00 f0 0f 1f 00 ........
0x1f0000:       jg      0x1efff3
0x1f0003:       mov     ecx, dword ptr [edx]
0x1f0005:       jno     0x1f0007
0x1f0007:       add     esi, ebp
3856    WebCompanion.e  0x7d0000        0x80ffff        VadS    PAGE_EXECUTE_READWRITE  1       1Disabled
01 a0 33 b8 02 5c 00 01 ..3..\..
ee ff ee ff 00 00 00 00 ........
a8 00 7d 00 a8 00 7d 00 ..}...}.
00 00 7d 00 00 00 7d 00 ..}...}.
40 00 00 00 88 05 7d 00 @.....}.
00 00 81 00 3f 00 00 00 ....?...
01 00 00 00 00 00 00 00 ........
f0 0f 7d 00 f0 0f 7d 00 ..}...}.
0x7d0000:       add     dword ptr [eax + 0x5c02b833], esp
0x7d0006:       add     byte ptr [ecx], al
0x7d0008:       out     dx, al
3856    WebCompanion.e  0x4990000       0x49cffff       VadS    PAGE_EXECUTE_READWRITE  27      1Disabled
13 e6 17 8b 1b 43 00 01 .....C..
ee ff ee ff 00 00 00 00 ........
a8 00 99 04 a8 00 99 04 ........
00 00 99 04 00 00 99 04 ........
40 00 00 00 88 05 99 04 @.......
00 00 9d 04 25 00 00 00 ....%...
01 00 00 00 00 00 00 00 ........
f0 af 9a 04 f0 af 9a 04 ........
0x4990000:      adc     esp, esi
0x4990002:      pop     ss
0x4990003:      mov     ebx, dword ptr [ebx]
0x4990005:      inc     ebx
0x4990006:      add     byte ptr [ecx], al
0x4990008:      out     dx, al
```


# windows.malfind.Malfind 分析

## 1. Plugin 功能說明

`windows.malfind.Malfind` 用來掃描行程記憶體中可疑的 VAD 區塊。

Malfind 主要會尋找具有可疑權限的記憶體區域，例如：

```text
PAGE_EXECUTE_READWRITE
PAGE_EXECUTE_WRITECOPY
```

這類記憶體區塊可能代表程式有注入程式碼、Shellcode、解殼後程式碼或惡意程式在記憶體中動態產生可執行內容。

---

## 2. 執行指令

本次執行指令如下：

```bash
.\vol.exe -f .\OtterCTF.vmem windows.malfind.Malfind
```

此指令會掃描所有 Process，而不是只掃描單一 PID。

---

## 3. 欄位說明

| 欄位              | 說明                 |
| --------------- | ------------------ |
| `PID`           | 行程編號               |
| `Process`       | 行程名稱               |
| `Start VPN`     | 可疑記憶體區塊起始位址        |
| `End VPN`       | 可疑記憶體區塊結束位址        |
| `Tag`           | VAD 標籤             |
| `Protection`    | 記憶體保護權限            |
| `CommitCharge`  | 記憶體配置大小            |
| `PrivateMemory` | 是否為 private memory |
| `File output`   | 是否有 dump 出檔案       |
| `Hexdump`       | 可疑記憶體區塊的十六進位內容     |
| `Disasm`        | 反組譯結果              |

---

## 4. 本次掃描結果重點

本次 Malfind 發現多個具有 `PAGE_EXECUTE_READWRITE` 權限的記憶體區塊，包含：

```text
WmiPrvSE.exe
explorer.exe
BitTorrent.exe
PresentationFontCache.exe
mscorsvw.exe
svchost.exe
chrome.exe
vmware-tray.exe
WebCompanionInstaller
WebCompanion.exe
Lavasoft.WCAssistant
```

其中最需要注意的是：

```text
PID 3720  vmware-tray.ex
```

因為前面已經發現此行程路徑為：

```text
C:\Users\Rick\AppData\Local\Temp\RarSFX0\vmware-tray.exe
```

該路徑位於使用者 Temp 目錄中的 `RarSFX0`，不符合正常 VMware 程式位置，因此具有高度可疑性。

---

## 5. PID 3720 vmware-tray.exe 分析

Malfind 在 PID 3720 中發現多個可疑記憶體區塊：

```text
PID 3720  vmware-tray.ex  0x670000  0x6affff  VadS  PAGE_EXECUTE_READWRITE
PID 3720  vmware-tray.ex  0x510000  0x54ffff  VadS  PAGE_EXECUTE_READWRITE
PID 3720  vmware-tray.ex  0xc00000  0xc3ffff  VadS  PAGE_EXECUTE_READWRITE
PID 3720  vmware-tray.ex  0xa10000  0xa4ffff  VadS  PAGE_EXECUTE_READWRITE
```

```
D:\Forensic\G140A006\VolatilityWorkbench>.\vol.exe -f .\OtterCTF.vmem windows.malfind.Malfind | findstr 3720
3720ressvmware-tray.ex  0x670000PDB scan0x6affffished   VadS    PAGE_EXECUTE_READWRITE  1       1Disabled
3720    vmware-tray.ex  0x510000        0x54ffff        VadS    PAGE_EXECUTE_READWRITE  23      1Disabled
3720    vmware-tray.ex  0xc00000        0xc3ffff        VadS    PAGE_EXECUTE_READWRITE  1       1Disabled
3720    vmware-tray.ex  0xa10000        0xa4ffff        VadS    PAGE_EXECUTE_READWRITE  1       1Disabled
```

這代表 `vmware-tray.exe` 行程中存在多個同時具有「可寫入」與「可執行」權限的記憶體區塊。

這種權限組合在惡意程式分析中需要特別注意，因為它可能被用來執行動態產生的程式碼。

---

## 6. 與前面證據的關聯

前面分析已經發現：

```text
CmdLine:
C:\Users\Rick\AppData\Local\Temp\RarSFX0\vmware-tray.exe

Pstree:
Rick And Morty season 1 download.exe
↓
vmware-tray.exe

UserAssist:
C:\Users\Rick\AppData\Local\Temp\RarSFX0\vmware-tray.exe

DumpFiles:
成功 dump 出 vmware-tray.exe

READ_IT.txt:
Your files have been encrypted.
```

因此，Malfind 發現 PID 3720 有可疑可執行記憶體區塊，可進一步補強 `vmware-tray.exe` 的可疑性。

---

## 7. PID 3820 Rick And Morty 結果說明

本次完整 Malfind 結果中沒有看到 PID 3820 `Rick And Morty` 的項目。

這代表 Malfind 沒有在 PID 3820 中偵測到明顯符合條件的可疑 VAD 區塊。

但這不代表 `Rick And Morty season 1 download.exe` 是正常檔案。

原因是前面已有多項證據顯示它具有高度可疑性：

```text
1. 位於 C:\Torrents\
2. 檔名偽裝成影片下載
3. 實際副檔名為 .exe
4. UserAssist 顯示 Rick 使用者曾執行
5. Pstree 顯示其啟動 vmware-tray.exe
6. READ_IT.txt 顯示檔案遭加密
```

因此，`Rick And Morty season 1 download.exe` 仍可判定為主要可疑執行檔。

---

## 8. 其他行程說明

Malfind 也在 `BitTorrent.exe`、`WebCompanion`、`Lavasoft.WCAssistant`、`svchost.exe` 等行程中發現 `PAGE_EXECUTE_READWRITE` 區塊。

不過，單純出現 `PAGE_EXECUTE_READWRITE` 不一定代表惡意，部分正常程式、JIT、.NET 或瀏覽器相關程式也可能產生這類記憶體區塊。

因此，本案分析重點仍放在與事件鏈高度相關的 PID 3720 `vmware-tray.exe`。
