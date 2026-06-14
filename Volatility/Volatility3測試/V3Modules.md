# 測試內容
- vol.exe -f .\OtterCTF.vmem windows.modules.Modules

```
D:\Forensic\G140A006\VolatilityWorkbench>.\vol.exe -f .\OtterCTF.vmem windows.modules.Modules
Volatility 3 Framework 2.5.0
Progress:  100.00               PDB scanning finished
Offset  Base    Size    Name    Path    File output

0xfa8018d36e70  0xf80002a52000  0x5ea000        ntoskrnl.exe    \SystemRoot\system32\ntoskrnl.exeDisabled
0xfa8018d30100  0xf80002a09000  0x49000 hal.dll \SystemRoot\system32\hal.dll    Disabled
0xfa8018d36d90  0xf80000bb6000  0xa000  kdcom.dll       \SystemRoot\system32\kdcom.dll  Disabled
0xfa8018d36ca0  0xf88000c1f000  0x4f000 mcupdate.dll    \SystemRoot\system32\mcupdate_GenuineIntel.dll   Disabled
0xfa8018d36bc0  0xf88000c6e000  0x14000 PSHED.dll       \SystemRoot\system32\PSHED.dll  Disabled
0xfa8018d36ad0  0xf88000c82000  0x5e000 CLFS.SYS        \SystemRoot\system32\CLFS.SYS   Disabled
0xfa8018d369e0  0xf88000ce0000  0xc0000 CI.dll  \SystemRoot\system32\CI.dll     Disabled
0xfa8018d368e0  0xf88000efa000  0xa4000 Wdf01000.sys    \SystemRoot\system32\drivers\Wdf01000.sysDisabled
0xfa8018d36800  0xf88000f9e000  0xf000  WDFLDR.SYS      \SystemRoot\system32\drivers\WDFLDR.SYS Disabled
0xfa8018d36710  0xf88000e00000  0x57000 ACPI.sys        \SystemRoot\system32\drivers\ACPI.sys   Disabled
0xfa8018d37010  0xf88000e57000  0x9000  WMILIB.SYS      \SystemRoot\system32\drivers\WMILIB.SYS Disabled
0xfa8018d37f20  0xf88000e60000  0xa000  msisadrv.sys    \SystemRoot\system32\drivers\msisadrv.sysDisabled
0xfa8018d37e40  0xf88000e6a000  0x33000 pci.sys \SystemRoot\system32\drivers\pci.sys    Disabled
0xfa8018d37d50  0xf88000e9d000  0xd000  vdrvroot.sys    \SystemRoot\system32\drivers\vdrvroot.sysDisabled
0xfa8018d37c60  0xf88000eaa000  0x15000 partmgr.sys     \SystemRoot\System32\drivers\partmgr.sysDisabled
0xfa8018d37b70  0xf88000ebf000  0x9000  compbatt.sys    \SystemRoot\system32\DRIVERS\compbatt.sysDisabled
0xfa8018d37a90  0xf88000ec8000  0xc000  BATTC.SYS       \SystemRoot\system32\DRIVERS\BATTC.SYS  Disabled
0xfa8018d379b0  0xf88000ed4000  0x15000 volmgr.sys      \SystemRoot\system32\drivers\volmgr.sys Disabled
0xfa8018d378c0  0xf88000da0000  0x5c000 volmgrx.sys     \SystemRoot\System32\drivers\volmgrx.sysDisabled
0xfa8018d377d0  0xf88000ee9000  0x8000  intelide.sys    \SystemRoot\system32\drivers\intelide.sysDisabled
0xfa8018d376e0  0xf88000fad000  0x10000 PCIIDEX.SYS     \SystemRoot\system32\drivers\PCIIDEX.SYSDisabled
0xfa8018d37600  0xf88000fbd000  0x19000 vmci.sys        \SystemRoot\system32\DRIVERS\vmci.sys   Disabled
0xfa8018d37510  0xf88000fd6000  0x1a000 mountmgr.sys    \SystemRoot\System32\drivers\mountmgr.sysDisabled
0xfa8018d37430  0xf88000c00000  0x17000 vsock.sys       \SystemRoot\system32\drivers\vsock.sys  Disabled
0xfa8018d37350  0xf88000ff0000  0x9000  atapi.sys       \SystemRoot\system32\drivers\atapi.sys  Disabled
0xfa8018d37260  0xf880010ae000  0x2a000 ataport.SYS     \SystemRoot\system32\drivers\ataport.SYSDisabled
0xfa8018d37170  0xf880010d8000  0x1d000 lsi_sas.sys     \SystemRoot\system32\drivers\lsi_sas.sysDisabled
0xfa8018d38010  0xf880010f5000  0x63000 storport.sys    \SystemRoot\system32\drivers\storport.sysDisabled
0xfa8018d38f30  0xf88001158000  0xb000  msahci.sys      \SystemRoot\system32\drivers\msahci.sys Disabled
0xfa8018d38e40  0xf88001163000  0xb000  amdxata.sys     \SystemRoot\system32\drivers\amdxata.sysDisabled
0xfa8018d38d50  0xf8800116e000  0x4c000 fltmgr.sys      \SystemRoot\system32\drivers\fltmgr.sys Disabled
0xfa8018d38c60  0xf880011ba000  0x14000 fileinfo.sys    \SystemRoot\system32\drivers\fileinfo.sysDisabled
0xfa8018d38b50  0xf8800125d000  0x1a3000        Ntfs.sys        \SystemRoot\System32\Drivers\Ntfs.sys    Disabled
0xfa8018d38a60  0xf88001000000  0x5e000 msrpc.sys       \SystemRoot\System32\Drivers\msrpc.sys  Disabled
0xfa8018d38980  0xf88001200000  0x1b000 ksecdd.sys      \SystemRoot\System32\Drivers\ksecdd.sys Disabled
0xfa8018d38890  0xf88001474000  0x72000 cng.sys \SystemRoot\System32\Drivers\cng.sys    Disabled
0xfa8018d387b0  0xf880014e6000  0x11000 pcw.sys \SystemRoot\System32\drivers\pcw.sys    Disabled
0xfa8018d386d0  0xf880014f7000  0xa000  Fs_Rec.sys      \SystemRoot\System32\Drivers\Fs_Rec.sys Disabled
0xfa8018d385d0  0xf88001501000  0xf3000 ndis.sys        \SystemRoot\system32\drivers\ndis.sys   Disabled
0xfa8018d384e0  0xf88001400000  0x60000 NETIO.SYS       \SystemRoot\system32\drivers\NETIO.SYS  Disabled
0xfa8018d383f0  0xf8800121b000  0x2b000 ksecpkg.sys     \SystemRoot\System32\Drivers\ksecpkg.sysDisabled
0xfa8018d382d0  0xf88001637000  0x204000        tcpip.sys       \SystemRoot\System32\drivers\tcpip.sys   Disabled
0xfa8018d381e0  0xf8800183b000  0x4a000 fwpkclnt.sys    \SystemRoot\System32\drivers\fwpkclnt.sysDisabled
0xfa8018d39010  0xf88001885000  0x10000 vmstorfl.sys    \SystemRoot\system32\drivers\vmstorfl.sysDisabled
0xfa8018d39f20  0xf88001895000  0x4c000 volsnap.sys     \SystemRoot\system32\drivers\volsnap.sysDisabled
0xfa8018d38100  0xf880018e1000  0x8000  spldr.sys       \SystemRoot\System32\Drivers\spldr.sys  Disabled
0xfa8018d39e30  0xf880018e9000  0x3a000 rdyboost.sys    \SystemRoot\System32\drivers\rdyboost.sysDisabled
0xfa8018d39d50  0xf88001923000  0x12000 mup.sys \SystemRoot\System32\Drivers\mup.sys    Disabled
0xfa8018d39c60  0xf88001935000  0x9000  hwpolicy.sys    \SystemRoot\System32\drivers\hwpolicy.sysDisabled
0xfa8018d39b80  0xf8800193e000  0x3a000 fvevol.sys      \SystemRoot\System32\DRIVERS\fvevol.sys Disabled
0xfa8018d39aa0  0xf88001978000  0x16000 disk.sys        \SystemRoot\system32\drivers\disk.sys   Disabled
0xfa8018d399b0  0xf8800198e000  0x30000 CLASSPNP.SYS    \SystemRoot\system32\drivers\CLASSPNP.SYSDisabled
0xfa80193a9290  0xf8800105e000  0x2a000 cdrom.sys       \SystemRoot\system32\DRIVERS\cdrom.sys  Disabled
0xfa80193adc20  0xf88001613000  0x9000  Null.SYS        \SystemRoot\System32\Drivers\Null.SYS   Disabled
0xfa80193add50  0xf8800161c000  0x7000  Beep.SYS        \SystemRoot\System32\Drivers\Beep.SYS   Disabled
0xfa80193adf20  0xf88001623000  0xf000  vmrawdsk.sys    \??\C:\Program Files\VMware\VMware Tools\vmrawdsk.sys    Disabled
0xfa80193b5b50  0xf88001460000  0xe000  vga.sys \SystemRoot\System32\drivers\vga.sys    Disabled
0xfa80193b72d0  0xf88001088000  0x25000 VIDEOPRT.SYS    \SystemRoot\System32\drivers\VIDEOPRT.SYSDisabled
0xfa80193b9820  0xf88001246000  0x10000 watchdog.sys    \SystemRoot\System32\drivers\watchdog.sysDisabled
0xfa80193b37a0  0xf880019f3000  0x9000  RDPCDD.sys      \SystemRoot\System32\DRIVERS\RDPCDD.sys Disabled
0xfa80193bbe90  0xf880015f4000  0x9000  rdpencdd.sys    \SystemRoot\system32\drivers\rdpencdd.sysDisabled
0xfa80193bb7f0  0xf880011ce000  0x9000  rdprefmp.sys    \SystemRoot\system32\drivers\rdprefmp.sysDisabled
0xfa80193c1640  0xf880011d7000  0xb000  Msfs.SYS        \SystemRoot\System32\Drivers\Msfs.SYS   Disabled
0xfa80193c3690  0xf880011e2000  0x11000 Npfs.SYS        \SystemRoot\System32\Drivers\Npfs.SYS   Disabled
0xfa80193c3770  0xf88002cda000  0x22000 tdx.sys \SystemRoot\system32\DRIVERS\tdx.sys    Disabled
0xfa80193c9bb0  0xf88002cfc000  0xd000  TDI.SYS \SystemRoot\system32\DRIVERS\TDI.SYS    Disabled
0xfa80193d1310  0xf88002d09000  0x89000 afd.sys \SystemRoot\system32\drivers\afd.sys    Disabled
0xfa80193c52d0  0xf88002d92000  0x45000 netbt.sys       \SystemRoot\System32\DRIVERS\netbt.sys  Disabled
0xfa80193dba60  0xf88002dd7000  0xb000  ws2ifsl.sys     \SystemRoot\system32\drivers\ws2ifsl.sysDisabled
0xfa80193d1910  0xf88002de2000  0x9000  wfplwf.sys      \SystemRoot\system32\DRIVERS\wfplwf.sys Disabled
0xfa80193ddda0  0xf88002c00000  0x26000 pacer.sys       \SystemRoot\system32\DRIVERS\pacer.sys  Disabled
0xfa80193e5af0  0xf88002c26000  0xf000  netbios.sys     \SystemRoot\system32\DRIVERS\netbios.sysDisabled
0xfa80193e7f30  0xf88002c35000  0x28000 vmhgfs.sys      \SystemRoot\system32\drivers\vmhgfs.sys Disabled
0xfa80193efe10  0xf88002c5d000  0x1d000 serial.sys      \SystemRoot\system32\DRIVERS\serial.sys Disabled
0xfa80193ed7c0  0xf88002c7a000  0x1b000 wanarp.sys      \SystemRoot\system32\DRIVERS\wanarp.sys Disabled
0xfa80193f37f0  0xf88002c95000  0x14000 termdd.sys      \SystemRoot\system32\DRIVERS\termdd.sys Disabled
0xfa80193fb800  0xf88003a13000  0x51000 rdbss.sys       \SystemRoot\system32\DRIVERS\rdbss.sys  Disabled
0xfa8019406280  0xf88003a64000  0xc000  nsiproxy.sys    \SystemRoot\system32\drivers\nsiproxy.sysDisabled
0xfa801940cad0  0xf88003a70000  0xb000  mssmbios.sys    \SystemRoot\system32\DRIVERS\mssmbios.sysDisabled
0xfa801940cbd0  0xf88003a7b000  0xf000  discache.sys    \SystemRoot\System32\drivers\discache.sysDisabled
0xfa801940e280  0xf88003a8a000  0x83000 csc.sys \SystemRoot\system32\drivers\csc.sys    Disabled
0xfa8019412dd0  0xf88003b0d000  0x1e000 dfsc.sys        \SystemRoot\System32\Drivers\dfsc.sys   Disabled
0xfa8019414c90  0xf88003b2b000  0x11000 blbdrive.sys    \SystemRoot\system32\DRIVERS\blbdrive.sysDisabled
0xfa801941ac30  0xf88003b3c000  0x26000 tunnel.sys      \SystemRoot\system32\DRIVERS\tunnel.sys Disabled
0xfa801980b670  0xf88003b62000  0x1e000 i8042prt.sys    \SystemRoot\system32\DRIVERS\i8042prt.sysDisabled
0xfa801944c3e0  0xf88003b80000  0xf000  kbdclass.sys    \SystemRoot\system32\DRIVERS\kbdclass.sysDisabled
0xfa8019416430  0xf88003b8f000  0x8000  vmmouse.sys     \SystemRoot\system32\DRIVERS\vmmouse.sysDisabled
0xfa801944c500  0xf88003b97000  0xf000  mouclass.sys    \SystemRoot\system32\DRIVERS\mouclass.sysDisabled
0xfa8019474210  0xf88003ba6000  0xc000  serenum.sys     \SystemRoot\system32\DRIVERS\serenum.sysDisabled
0xfa8019474330  0xf88003bb2000  0x36000 vm3dmp.sys      \SystemRoot\system32\DRIVERS\vm3dmp.sys Disabled
0xfa8019532450  0xf88003cf6000  0xf4000 dxgkrnl.sys     \SystemRoot\System32\drivers\dxgkrnl.sysDisabled
0xfa80198388e0  0xf88003c00000  0x46000 dxgmms1.sys     \SystemRoot\System32\drivers\dxgmms1.sysDisabled
0xfa80198b4b90  0xf88003c46000  0xd000  usbuhci.sys     \SystemRoot\system32\DRIVERS\usbuhci.sysDisabled
0xfa80198bf860  0xf88003c53000  0x56000 USBPORT.SYS     \SystemRoot\system32\DRIVERS\USBPORT.SYSDisabled
0xfa801935f760  0xf88003ca9000  0x24000 E1G6032E.sys    \SystemRoot\system32\DRIVERS\E1G6032E.sysDisabled
0xfa8019395410  0xf88003ccd000  0x24000 HDAudBus.sys    \SystemRoot\system32\DRIVERS\HDAudBus.sysDisabled
0xfa80198c3950  0xf88003dea000  0x11000 usbehci.sys     \SystemRoot\system32\DRIVERS\usbehci.sysDisabled
0xfa8019854530  0xf88003dfb000  0x5000  CmBatt.sys      \SystemRoot\system32\DRIVERS\CmBatt.sys Disabled
0xfa8019855830  0xf88003be8000  0x16000 intelppm.sys    \SystemRoot\system32\DRIVERS\intelppm.sysDisabled
0xfa80198626e0  0xf88003a00000  0xa000  pnpmem.sys      \SystemRoot\system32\DRIVERS\pnpmem.sys Disabled
0xfa8019865750  0xf88002ca9000  0x10000 CompositeBus.sys        \SystemRoot\system32\DRIVERS\CompositeBus.sys    Disabled
0xfa8019166760  0xf88002cb9000  0x16000 AgileVpn.sys    \SystemRoot\system32\DRIVERS\AgileVpn.sysDisabled
0xfa801986a3f0  0xf88003e81000  0x24000 rasl2tp.sys     \SystemRoot\system32\DRIVERS\rasl2tp.sysDisabled
0xfa801986e730  0xf88003ea5000  0xc000  ndistapi.sys    \SystemRoot\system32\DRIVERS\ndistapi.sysDisabled
0xfa801986c0f0  0xf88003eb1000  0x2f000 ndiswan.sys     \SystemRoot\system32\DRIVERS\ndiswan.sysDisabled
0xfa801987ac10  0xf88003ee0000  0x1b000 raspppoe.sys    \SystemRoot\system32\DRIVERS\raspppoe.sysDisabled
0xfa801987bea0  0xf88003efb000  0x21000 raspptp.sys     \SystemRoot\system32\DRIVERS\raspptp.sysDisabled
0xfa801987ca80  0xf88003f1c000  0x1a000 rassstp.sys     \SystemRoot\system32\DRIVERS\rassstp.sysDisabled
0xfa8019886010  0xf88003f36000  0xb000  rdpbus.sys      \SystemRoot\system32\DRIVERS\rdpbus.sys Disabled
0xfa80198877d0  0xf88003f41000  0x2000  swenum.sys      \SystemRoot\system32\DRIVERS\swenum.sys Disabled
0xfa80198862e0  0xf88003f43000  0x43000 ks.sys  \SystemRoot\system32\DRIVERS\ks.sys     Disabled
0xfa801988a2b0  0xf88003f86000  0x12000 umbus.sys       \SystemRoot\system32\DRIVERS\umbus.sys  Disabled
0xfa80198dcb20  0xf88003f98000  0x5a000 usbhub.sys      \SystemRoot\system32\DRIVERS\usbhub.sys Disabled
0xfa8019822b60  0xf88003e00000  0x15000 NDProxy.SYS     \SystemRoot\System32\Drivers\NDProxy.SYSDisabled
0xfa8019f93970  0xf88003e15000  0x5c000 HdAudio.sys     \SystemRoot\system32\drivers\HdAudio.sysDisabled
0xfa8019f8ee40  0xf88004271000  0x3d000 portcls.sys     \SystemRoot\system32\drivers\portcls.sysDisabled
0xfa8019f9e420  0xf880042ae000  0x22000 drmk.sys        \SystemRoot\system32\drivers\drmk.sys   Disabled
0xfa8019fa3780  0xf880042d0000  0x6000  ksthunk.sys     \SystemRoot\system32\drivers\ksthunk.sysDisabled
0xfa8019744010  0xf880042d6000  0xe000  crashdmp.sys    \SystemRoot\System32\Drivers\crashdmp.sysDisabled
0xfa801978a010  0xf880042e4000  0xa000  dump_storport.sys       \SystemRoot\System32\Drivers\dump_diskdump.sys   Disabled
0xfa801978a950  0xf880042ee000  0x1d000 dump_LSI_SAS.sys        \SystemRoot\System32\Drivers\dump_LSI_SAS.sys    Disabled
0xfa80194baf20  0xf8800430b000  0x13000 dump_dumpfve.sys        \SystemRoot\System32\Drivers\dump_dumpfve.sys    Disabled
0xfa8019fde4a0  0xf8800431e000  0x1d000 usbccgp.sys     \SystemRoot\system32\DRIVERS\usbccgp.sysDisabled
0xfa8019fde780  0xf8800433b000  0x2000  USBD.SYS        \SystemRoot\system32\DRIVERS\USBD.SYS   Disabled
0xfa801a06fb80  0xf8800433d000  0xe000  hidusb.sys      \SystemRoot\system32\DRIVERS\hidusb.sys Disabled
0xfa801a06fc60  0xf8800434b000  0x19000 HIDCLASS.SYS    \SystemRoot\system32\DRIVERS\HIDCLASS.SYSDisabled
0xfa801a07c860  0xf88004364000  0x9000  HIDPARSE.SYS    \SystemRoot\system32\DRIVERS\HIDPARSE.SYSDisabled
0xfa801a07c3f0  0xf8800436d000  0xd000  mouhid.sys      \SystemRoot\system32\DRIVERS\mouhid.sys Disabled
0xfa801a0862c0  0xf8800437a000  0x9000  vmusbmouse.sys  \SystemRoot\system32\DRIVERS\vmusbmouse.sys      Disabled
0xfa801a08ae70  0xf88004383000  0x18000 BTHUSB.sys      \SystemRoot\System32\Drivers\BTHUSB.sys Disabled
0xfa801a08b4b0  0xf88004475000  0x8c000 bthport.sys     \SystemRoot\System32\Drivers\bthport.sysDisabled
0xfa801a0ac010  0xf88004501000  0x2c000 rfcomm.sys      \SystemRoot\system32\DRIVERS\rfcomm.sys Disabled
0xfa801a0a95f0  0xf8800452d000  0x10000 BthEnum.sys     \SystemRoot\system32\DRIVERS\BthEnum.sysDisabled
0xfa801a0afa30  0xf960000e0000  0x310000        win32k.sys      \SystemRoot\System32\win32k.sys Disabled
0xfa801a0a3320  0xf8800453d000  0xc000  Dxapi.sys       \SystemRoot\System32\drivers\Dxapi.sys  Disabled
0xfa801a0ba6c0  0xf88004549000  0x20000 bthpan.sys      \SystemRoot\system32\DRIVERS\bthpan.sys Disabled
0xfa8018da97b0  0xf88004569000  0xe000  monitor.sys     \SystemRoot\system32\DRIVERS\monitor.sysDisabled
0xfa801969e870  0xf96000440000  0xa000  TSDDD.dll       \SystemRoot\System32\TSDDD.dll  Disabled
0xfa801a0aad50  0xf960007b0000  0x27000 cdd.dll \SystemRoot\System32\cdd.dll    Disabled
0xfa801abacc00  0xf88004577000  0x23000 luafv.sys       \SystemRoot\system32\drivers\luafv.sys  Disabled
0xfa801acc3010  0xf8800459a000  0x15000 lltdio.sys      \SystemRoot\system32\DRIVERS\lltdio.sys Disabled
0xfa801acc9790  0xf880045af000  0x18000 rspndr.sys      \SystemRoot\system32\DRIVERS\rspndr.sys Disabled
0xfa801ad46660  0xf88002a33000  0xc9000 HTTP.sys        \SystemRoot\system32\drivers\HTTP.sys   Disabled
0xfa801ad8e540  0xf88002afc000  0x1e000 bowser.sys      \SystemRoot\system32\DRIVERS\bowser.sys Disabled
0xfa801ad92970  0xf88002b1a000  0x18000 mpsdrv.sys      \SystemRoot\System32\drivers\mpsdrv.sys Disabled
0xfa801ad95c70  0xf88002b32000  0x2d000 mrxsmb.sys      \SystemRoot\system32\DRIVERS\mrxsmb.sys Disabled
0xfa801ada7270  0xf88002b5f000  0x4d000 mrxsmb10.sys    \SystemRoot\system32\DRIVERS\mrxsmb10.sysDisabled
0xfa801ac65520  0xf88002bac000  0x24000 mrxsmb20.sys    \SystemRoot\system32\DRIVERS\mrxsmb20.sysDisabled
0xfa801adcb510  0xf88002bd0000  0xa000  vmmemctl.sys    \??\C:\Program Files\Common Files\VMware\Drivers\memctl\vmmemctl.sys     Disabled
0xfa801adcf210  0xf880034ab000  0xa6000 peauth.sys      \SystemRoot\system32\drivers\peauth.sys Disabled
0xfa801add5ce0  0xf88003551000  0xb000  secdrv.SYS      \SystemRoot\System32\Drivers\secdrv.SYS Disabled
0xfa8018d72cc0  0xf8800355c000  0x31000 srvnet.sys      \SystemRoot\System32\DRIVERS\srvnet.sys Disabled
0xfa801add1760  0xf8800358d000  0x12000 tcpipreg.sys    \SystemRoot\System32\drivers\tcpipreg.sysDisabled
0xfa801af3dbc0  0xf88003400000  0x6b000 srv2.sys        \SystemRoot\System32\DRIVERS\srv2.sys   Disabled
0xfa801af3ef20  0xf88004a0d000  0x99000 srv.sys \SystemRoot\System32\DRIVERS\srv.sys    Disabled
0xfa801aed8160  0xf88004aa6000  0x71000 spsys.sys       \SystemRoot\system32\drivers\spsys.sys  Disabled
```
