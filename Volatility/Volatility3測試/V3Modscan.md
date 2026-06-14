# 測試內容
- vol.exe -f .\OtterCTF.vmem windows.modscan.ModScan


```
D:\Forensic\G140A006\VolatilityWorkbench>.\vol.exe -f .\OtterCTF.vmem windows.modscan.ModScan
Volatility 3 Framework 2.5.0
Progress:  100.00               PDB scanning finished
Offset  Base    Size    Name    Path    File output

0x2b20891       0x24748b483024  0x48909090                      Disabled
0x2e662a7       0x6840c70772    0x48206848                      Disabled
0x2eb4145       0x24548d48ffbe  0x448b48ff                      Disabled
0x2d581088      0xf8800312ba50  0x312ba18                       Disabled
0x7dcd8160      0xf88004aa6000  0x71000 spsys.sys       \SystemRoot\system32\drivers\spsys.sys  Disabled
0x7dd3dbc0      0xf88003400000  0x6b000 srv2.sys        \SystemRoot\System32\DRIVERS\srv2.sys   Disabled
0x7dd3ef20      0xf88004a0d000  0x99000 srv.sys \SystemRoot\System32\DRIVERS\srv.sys    Disabled
0x7de65520      0xf88002bac000  0x24000 mrxsmb20.sys    \SystemRoot\system32\DRIVERS\mrxsmb20.sysDisabled
0x7dec3010      0xf8800459a000  0x15000 lltdio.sys      \SystemRoot\system32\DRIVERS\lltdio.sys Disabled
0x7dec9790      0xf880045af000  0x18000 rspndr.sys      \SystemRoot\system32\DRIVERS\rspndr.sys Disabled
0x7df46660      0xf88002a33000  0xc9000 HTTP.sys        \SystemRoot\system32\drivers\HTTP.sys   Disabled
0x7df8e540      0xf88002afc000  0x1e000 bowser.sys      \SystemRoot\system32\DRIVERS\bowser.sys Disabled
0x7df92970      0xf88002b1a000  0x18000 mpsdrv.sys      \SystemRoot\System32\drivers\mpsdrv.sys Disabled
0x7df95c70      0xf88002b32000  0x2d000 mrxsmb.sys      \SystemRoot\system32\DRIVERS\mrxsmb.sys Disabled
0x7dfa7270      0xf88002b5f000  0x4d000 mrxsmb10.sys    \SystemRoot\system32\DRIVERS\mrxsmb10.sysDisabled
0x7dfcb510      0xf88002bd0000  0xa000  vmmemctl.sys    \??\C:\Program Files\Common Files\VMware\Drivers\memctl\vmmemctl.sys     Disabled
0x7dfcf210      0xf880034ab000  0xa6000 peauth.sys      \SystemRoot\system32\drivers\peauth.sys Disabled
0x7dfd1760      0xf8800358d000  0x12000 tcpipreg.sys    \SystemRoot\System32\drivers\tcpipreg.sysDisabled
0x7dfd5ce0      0xf88003551000  0xb000  secdrv.SYS      \SystemRoot\System32\Drivers\secdrv.SYS Disabled
0x7e1acc00      0xf88004577000  0x23000 luafv.sys       \SystemRoot\system32\drivers\luafv.sys  Disabled
0x7ea6fb80      0xf8800433d000  0xe000  hidusb.sys      \SystemRoot\system32\DRIVERS\hidusb.sys Disabled
0x7ea6fc60      0xf8800434b000  0x19000 HIDCLASS.SYS    \SystemRoot\system32\DRIVERS\HIDCLASS.SYSDisabled
0x7ea7c3f0      0xf8800436d000  0xd000  mouhid.sys      \SystemRoot\system32\DRIVERS\mouhid.sys Disabled
0x7ea7c860      0xf88004364000  0x9000  HIDPARSE.SYS    \SystemRoot\system32\DRIVERS\HIDPARSE.SYSDisabled
0x7ea862c0      0xf8800437a000  0x9000  vmusbmouse.sys  \SystemRoot\system32\DRIVERS\vmusbmouse.sys      Disabled
0x7ea8ae70      0xf88004383000  0x18000 BTHUSB.sys      \SystemRoot\System32\Drivers\BTHUSB.sys Disabled
0x7ea8b4b0      0xf88004475000  0x8c000 bthport.sys     \SystemRoot\System32\Drivers\bthport.sysDisabled
0x7eaa3320      0xf8800453d000  0xc000  Dxapi.sys       \SystemRoot\System32\drivers\Dxapi.sys  Disabled
0x7eaa95f0      0xf8800452d000  0x10000 BthEnum.sys     \SystemRoot\system32\DRIVERS\BthEnum.sysDisabled
0x7eaaad50      0xf960007b0000  0x27000 cdd.dll \SystemRoot\System32\cdd.dll    Disabled
0x7eaac010      0xf88004501000  0x2c000 rfcomm.sys      \SystemRoot\system32\DRIVERS\rfcomm.sys Disabled
0x7eaafa30      0xf960000e0000  0x310000        win32k.sys      \SystemRoot\System32\win32k.sys Disabled
0x7eaba6c0      0xf88004549000  0x20000 bthpan.sys      \SystemRoot\system32\DRIVERS\bthpan.sys Disabled
0x7ed8ee40      0xf88004271000  0x3d000 portcls.sys     \SystemRoot\system32\drivers\portcls.sysDisabled
0x7ed93970      0xf88003e15000  0x5c000 HdAudio.sys     \SystemRoot\system32\drivers\HdAudio.sysDisabled
0x7ed9e420      0xf880042ae000  0x22000 drmk.sys        \SystemRoot\system32\drivers\drmk.sys   Disabled
0x7eda3780      0xf880042d0000  0x6000  ksthunk.sys     \SystemRoot\system32\drivers\ksthunk.sysDisabled
0x7edde4a0      0xf8800431e000  0x1d000 usbccgp.sys     \SystemRoot\system32\DRIVERS\usbccgp.sysDisabled
0x7edde780      0xf8800433b000  0x2000  USBD.SYS        \SystemRoot\system32\DRIVERS\USBD.SYS   Disabled
0x7f20b670      0xf88003b62000  0x1e000 i8042prt.sys    \SystemRoot\system32\DRIVERS\i8042prt.sysDisabled
0x7f222b60      0xf88003e00000  0x15000 NDProxy.SYS     \SystemRoot\System32\Drivers\NDProxy.SYSDisabled
0x7f2388e0      0xf88003c00000  0x46000 dxgmms1.sys     \SystemRoot\System32\drivers\dxgmms1.sysDisabled
0x7f254530      0xf88003dfb000  0x5000  CmBatt.sys      \SystemRoot\system32\DRIVERS\CmBatt.sys Disabled
0x7f255830      0xf88003be8000  0x16000 intelppm.sys    \SystemRoot\system32\DRIVERS\intelppm.sysDisabled
0x7f2626e0      0xf88003a00000  0xa000  pnpmem.sys      \SystemRoot\system32\DRIVERS\pnpmem.sys Disabled
0x7f265750      0xf88002ca9000  0x10000 CompositeBus.sys        \SystemRoot\system32\DRIVERS\CompositeBus.sys    Disabled
0x7f26a3f0      0xf88003e81000  0x24000 rasl2tp.sys     \SystemRoot\system32\DRIVERS\rasl2tp.sysDisabled
0x7f26c0f0      0xf88003eb1000  0x2f000 ndiswan.sys     \SystemRoot\system32\DRIVERS\ndiswan.sysDisabled
0x7f26e730      0xf88003ea5000  0xc000  ndistapi.sys    \SystemRoot\system32\DRIVERS\ndistapi.sysDisabled
0x7f27ac10      0xf88003ee0000  0x1b000 raspppoe.sys    \SystemRoot\system32\DRIVERS\raspppoe.sysDisabled
0x7f27bea0      0xf88003efb000  0x21000 raspptp.sys     \SystemRoot\system32\DRIVERS\raspptp.sysDisabled
0x7f27ca80      0xf88003f1c000  0x1a000 rassstp.sys     \SystemRoot\system32\DRIVERS\rassstp.sysDisabled
0x7f286010      0xf88003f36000  0xb000  rdpbus.sys      \SystemRoot\system32\DRIVERS\rdpbus.sys Disabled
0x7f2862e0      0xf88003f43000  0x43000 ks.sys  \SystemRoot\system32\DRIVERS\ks.sys     Disabled
0x7f2877d0      0xf88003f41000  0x2000  swenum.sys      \SystemRoot\system32\DRIVERS\swenum.sys Disabled
0x7f28a2b0      0xf88003f86000  0x12000 umbus.sys       \SystemRoot\system32\DRIVERS\umbus.sys  Disabled
0x7f2b4b90      0xf88003c46000  0xd000  usbuhci.sys     \SystemRoot\system32\DRIVERS\usbuhci.sysDisabled
0x7f2bf860      0xf88003c53000  0x56000 USBPORT.SYS     \SystemRoot\system32\DRIVERS\USBPORT.SYSDisabled
0x7f2c3950      0xf88003dea000  0x11000 usbehci.sys     \SystemRoot\system32\DRIVERS\usbehci.sysDisabled
0x7f2dcb20      0xf88003f98000  0x5a000 usbhub.sys      \SystemRoot\system32\DRIVERS\usbhub.sys Disabled
0x7f49e870      0xf96000440000  0xa000  TSDDD.dll       \SystemRoot\System32\TSDDD.dll  Disabled
0x7f544010      0xf880042d6000  0xe000  crashdmp.sys    \SystemRoot\System32\Drivers\crashdmp.sysDisabled
0x7f58a010      0xf880042e4000  0xa000  dump_storport.sys       \SystemRoot\System32\Drivers\dump_diskdump.sys   Disabled
0x7f58a950      0xf880042ee000  0x1d000 dump_LSI_SAS.sys        \SystemRoot\System32\Drivers\dump_LSI_SAS.sys    Disabled
0x7f606280      0xf88003a64000  0xc000  nsiproxy.sys    \SystemRoot\system32\drivers\nsiproxy.sysDisabled
0x7f60cad0      0xf88003a70000  0xb000  mssmbios.sys    \SystemRoot\system32\DRIVERS\mssmbios.sysDisabled
0x7f60cbd0      0xf88003a7b000  0xf000  discache.sys    \SystemRoot\System32\drivers\discache.sysDisabled
0x7f60e280      0xf88003a8a000  0x83000 csc.sys \SystemRoot\system32\drivers\csc.sys    Disabled
0x7f612dd0      0xf88003b0d000  0x1e000 dfsc.sys        \SystemRoot\System32\Drivers\dfsc.sys   Disabled
0x7f614c90      0xf88003b2b000  0x11000 blbdrive.sys    \SystemRoot\system32\DRIVERS\blbdrive.sysDisabled
0x7f616430      0xf88003b8f000  0x8000  vmmouse.sys     \SystemRoot\system32\DRIVERS\vmmouse.sysDisabled
0x7f61ac30      0xf88003b3c000  0x26000 tunnel.sys      \SystemRoot\system32\DRIVERS\tunnel.sys Disabled
0x7f64c3e0      0xf88003b80000  0xf000  kbdclass.sys    \SystemRoot\system32\DRIVERS\kbdclass.sysDisabled
0x7f64c500      0xf88003b97000  0xf000  mouclass.sys    \SystemRoot\system32\DRIVERS\mouclass.sysDisabled
0x7f674210      0xf88003ba6000  0xc000  serenum.sys     \SystemRoot\system32\DRIVERS\serenum.sysDisabled
0x7f674330      0xf88003bb2000  0x36000 vm3dmp.sys      \SystemRoot\system32\DRIVERS\vm3dmp.sys Disabled
0x7f6baf20      0xf8800430b000  0x13000 dump_dumpfve.sys        \SystemRoot\System32\Drivers\dump_dumpfve.sys    Disabled
0x7f732450      0xf88003cf6000  0xf4000 dxgkrnl.sys     \SystemRoot\System32\drivers\dxgkrnl.sysDisabled
0x7f95f760      0xf88003ca9000  0x24000 E1G6032E.sys    \SystemRoot\system32\DRIVERS\E1G6032E.sysDisabled
0x7f995410      0xf88003ccd000  0x24000 HDAudBus.sys    \SystemRoot\system32\DRIVERS\HDAudBus.sysDisabled
0x7f9a9290      0xf8800105e000  0x2a000 cdrom.sys       \SystemRoot\system32\DRIVERS\cdrom.sys  Disabled
0x7f9adc20      0xf88001613000  0x9000  Null.SYS        \SystemRoot\System32\Drivers\Null.SYS   Disabled
0x7f9add50      0xf8800161c000  0x7000  Beep.SYS        \SystemRoot\System32\Drivers\Beep.SYS   Disabled
0x7f9adf20      0xf88001623000  0xf000  vmrawdsk.sys    \??\C:\Program Files\VMware\VMware Tools\vmrawdsk.sys    Disabled
0x7f9b37a0      0xf880019f3000  0x9000  RDPCDD.sys      \SystemRoot\System32\DRIVERS\RDPCDD.sys Disabled
0x7f9b5b50      0xf88001460000  0xe000  vga.sys \SystemRoot\System32\drivers\vga.sys    Disabled
0x7f9b72d0      0xf88001088000  0x25000 VIDEOPRT.SYS    \SystemRoot\System32\drivers\VIDEOPRT.SYSDisabled
0x7f9b9820      0xf88001246000  0x10000 watchdog.sys    \SystemRoot\System32\drivers\watchdog.sysDisabled
0x7f9bb7f0      0xf880011ce000  0x9000  rdprefmp.sys    \SystemRoot\system32\drivers\rdprefmp.sysDisabled
0x7f9bbe90      0xf880015f4000  0x9000  rdpencdd.sys    \SystemRoot\system32\drivers\rdpencdd.sysDisabled
0x7f9c1640      0xf880011d7000  0xb000  Msfs.SYS        \SystemRoot\System32\Drivers\Msfs.SYS   Disabled
0x7f9c3690      0xf880011e2000  0x11000 Npfs.SYS        \SystemRoot\System32\Drivers\Npfs.SYS   Disabled
0x7f9c3770      0xf88002cda000  0x22000 tdx.sys \SystemRoot\system32\DRIVERS\tdx.sys    Disabled
0x7f9c52d0      0xf88002d92000  0x45000 netbt.sys       \SystemRoot\System32\DRIVERS\netbt.sys  Disabled
0x7f9c9bb0      0xf88002cfc000  0xd000  TDI.SYS \SystemRoot\system32\DRIVERS\TDI.SYS    Disabled
0x7f9d1310      0xf88002d09000  0x89000 afd.sys \SystemRoot\system32\drivers\afd.sys    Disabled
0x7f9d1910      0xf88002de2000  0x9000  wfplwf.sys      \SystemRoot\system32\DRIVERS\wfplwf.sys Disabled
0x7f9dba60      0xf88002dd7000  0xb000  ws2ifsl.sys     \SystemRoot\system32\drivers\ws2ifsl.sysDisabled
0x7f9ddda0      0xf88002c00000  0x26000 pacer.sys       \SystemRoot\system32\DRIVERS\pacer.sys  Disabled
0x7f9e5af0      0xf88002c26000  0xf000  netbios.sys     \SystemRoot\system32\DRIVERS\netbios.sysDisabled
0x7f9e7f30      0xf88002c35000  0x28000 vmhgfs.sys      \SystemRoot\system32\drivers\vmhgfs.sys Disabled
0x7f9ed7c0      0xf88002c7a000  0x1b000 wanarp.sys      \SystemRoot\system32\DRIVERS\wanarp.sys Disabled
0x7f9efe10      0xf88002c5d000  0x1d000 serial.sys      \SystemRoot\system32\DRIVERS\serial.sys Disabled
0x7f9f37f0      0xf88002c95000  0x14000 termdd.sys      \SystemRoot\system32\DRIVERS\termdd.sys Disabled
0x7f9fb800      0xf88003a13000  0x51000 rdbss.sys       \SystemRoot\system32\DRIVERS\rdbss.sys  Disabled
0x7fb66760      0xf88002cb9000  0x16000 AgileVpn.sys    \SystemRoot\system32\DRIVERS\AgileVpn.sysDisabled
0x7fe287b0      0xf88004569000  0xe000  monitor.sys     \SystemRoot\system32\DRIVERS\monitor.sysDisabled
0x7fe71cc0      0xf8800355c000  0x31000 srvnet.sys      \SystemRoot\System32\DRIVERS\srvnet.sys Disabled
0x7feaf100      0xf80002a09000  0x49000 hal.dll \SystemRoot\system32\hal.dll    Disabled
0x7feb5710      0xf88000e00000  0x57000 ACPI.sys        \SystemRoot\system32\drivers\ACPI.sys   Disabled
0x7feb5800      0xf88000f9e000  0xf000  WDFLDR.SYS      \SystemRoot\system32\drivers\WDFLDR.SYS Disabled
0x7feb58e0      0xf88000efa000  0xa4000 Wdf01000.sys    \SystemRoot\system32\drivers\Wdf01000.sysDisabled
0x7feb59e0      0xf88000ce0000  0xc0000 CI.dll  \SystemRoot\system32\CI.dll     Disabled
0x7feb5ad0      0xf88000c82000  0x5e000 CLFS.SYS        \SystemRoot\system32\CLFS.SYS   Disabled
0x7feb5bc0      0xf88000c6e000  0x14000 PSHED.dll       \SystemRoot\system32\PSHED.dll  Disabled
0x7feb5ca0      0xf88000c1f000  0x4f000 mcupdate.dll    \SystemRoot\system32\mcupdate_GenuineIntel.dll   Disabled
0x7feb5d90      0xf80000bb6000  0xa000  kdcom.dll       \SystemRoot\system32\kdcom.dll  Disabled
0x7feb5e70      0xf80002a52000  0x5ea000        ntoskrnl.exe    \SystemRoot\system32\ntoskrnl.exeDisabled
0x7feb6010      0xf88000e57000  0x9000  WMILIB.SYS      \SystemRoot\system32\drivers\WMILIB.SYS Disabled
0x7feb6170      0xf880010d8000  0x1d000 lsi_sas.sys     \SystemRoot\system32\drivers\lsi_sas.sysDisabled
0x7feb6260      0xf880010ae000  0x2a000 ataport.SYS     \SystemRoot\system32\drivers\ataport.SYSDisabled
0x7feb6350      0xf88000ff0000  0x9000  atapi.sys       \SystemRoot\system32\drivers\atapi.sys  Disabled
0x7feb6430      0xf88000c00000  0x17000 vsock.sys       \SystemRoot\system32\drivers\vsock.sys  Disabled
0x7feb6510      0xf88000fd6000  0x1a000 mountmgr.sys    \SystemRoot\System32\drivers\mountmgr.sysDisabled
0x7feb6600      0xf88000fbd000  0x19000 vmci.sys        \SystemRoot\system32\DRIVERS\vmci.sys   Disabled
0x7feb66e0      0xf88000fad000  0x10000 PCIIDEX.SYS     \SystemRoot\system32\drivers\PCIIDEX.SYSDisabled
0x7feb67d0      0xf88000ee9000  0x8000  intelide.sys    \SystemRoot\system32\drivers\intelide.sysDisabled
0x7feb68c0      0xf88000da0000  0x5c000 volmgrx.sys     \SystemRoot\System32\drivers\volmgrx.sysDisabled
0x7feb69b0      0xf88000ed4000  0x15000 volmgr.sys      \SystemRoot\system32\drivers\volmgr.sys Disabled
0x7feb6a90      0xf88000ec8000  0xc000  BATTC.SYS       \SystemRoot\system32\DRIVERS\BATTC.SYS  Disabled
0x7feb6b70      0xf88000ebf000  0x9000  compbatt.sys    \SystemRoot\system32\DRIVERS\compbatt.sysDisabled
0x7feb6c60      0xf88000eaa000  0x15000 partmgr.sys     \SystemRoot\System32\drivers\partmgr.sysDisabled
0x7feb6d50      0xf88000e9d000  0xd000  vdrvroot.sys    \SystemRoot\system32\drivers\vdrvroot.sysDisabled
0x7feb6e40      0xf88000e6a000  0x33000 pci.sys \SystemRoot\system32\drivers\pci.sys    Disabled
0x7feb6f20      0xf88000e60000  0xa000  msisadrv.sys    \SystemRoot\system32\drivers\msisadrv.sysDisabled
0x7feb7010      0xf880010f5000  0x63000 storport.sys    \SystemRoot\system32\drivers\storport.sysDisabled
0x7feb7100      0xf880018e1000  0x8000  spldr.sys       \SystemRoot\System32\Drivers\spldr.sys  Disabled
0x7feb71e0      0xf8800183b000  0x4a000 fwpkclnt.sys    \SystemRoot\System32\drivers\fwpkclnt.sysDisabled
0x7feb72d0      0xf88001637000  0x204000        tcpip.sys       \SystemRoot\System32\drivers\tcpip.sys   Disabled
0x7feb73f0      0xf8800121b000  0x2b000 ksecpkg.sys     \SystemRoot\System32\Drivers\ksecpkg.sysDisabled
0x7feb74e0      0xf88001400000  0x60000 NETIO.SYS       \SystemRoot\system32\drivers\NETIO.SYS  Disabled
0x7feb75d0      0xf88001501000  0xf3000 ndis.sys        \SystemRoot\system32\drivers\ndis.sys   Disabled
0x7feb76d0      0xf880014f7000  0xa000  Fs_Rec.sys      \SystemRoot\System32\Drivers\Fs_Rec.sys Disabled
0x7feb77b0      0xf880014e6000  0x11000 pcw.sys \SystemRoot\System32\drivers\pcw.sys    Disabled
0x7feb7890      0xf88001474000  0x72000 cng.sys \SystemRoot\System32\Drivers\cng.sys    Disabled
0x7feb7980      0xf88001200000  0x1b000 ksecdd.sys      \SystemRoot\System32\Drivers\ksecdd.sys Disabled
0x7feb7a60      0xf88001000000  0x5e000 msrpc.sys       \SystemRoot\System32\Drivers\msrpc.sys  Disabled
0x7feb7b50      0xf8800125d000  0x1a3000        Ntfs.sys        \SystemRoot\System32\Drivers\Ntfs.sys    Disabled
0x7feb7c60      0xf880011ba000  0x14000 fileinfo.sys    \SystemRoot\system32\drivers\fileinfo.sysDisabled
0x7feb7d50      0xf8800116e000  0x4c000 fltmgr.sys      \SystemRoot\system32\drivers\fltmgr.sys Disabled
0x7feb7e40      0xf88001163000  0xb000  amdxata.sys     \SystemRoot\system32\drivers\amdxata.sysDisabled
0x7feb7f30      0xf88001158000  0xb000  msahci.sys      \SystemRoot\system32\drivers\msahci.sys Disabled
0x7feb8010      0xf88001885000  0x10000 vmstorfl.sys    \SystemRoot\system32\drivers\vmstorfl.sysDisabled
0x7feb89b0      0xf8800198e000  0x30000 CLASSPNP.SYS    \SystemRoot\system32\drivers\CLASSPNP.SYSDisabled
0x7feb8aa0      0xf88001978000  0x16000 disk.sys        \SystemRoot\system32\drivers\disk.sys   Disabled
0x7feb8b80      0xf8800193e000  0x3a000 fvevol.sys      \SystemRoot\System32\DRIVERS\fvevol.sys Disabled
0x7feb8c60      0xf88001935000  0x9000  hwpolicy.sys    \SystemRoot\System32\drivers\hwpolicy.sysDisabled
0x7feb8d50      0xf88001923000  0x12000 mup.sys \SystemRoot\System32\Drivers\mup.sys    Disabled
0x7feb8e30      0xf880018e9000  0x3a000 rdyboost.sys    \SystemRoot\System32\drivers\rdyboost.sysDisabled
0x7feb8f20      0xf88001895000  0x4c000 volsnap.sys     \SystemRoot\system32\drivers\volsnap.sysDisabled
```
