# 測試內容

.\vol.exe -f .\OtterCTF.vmem windows.devicetree.DeviceTree

```
D:\Forensic\G140A006\VolatilityWorkbench>.\vol.exe -f .\OtterCTF.vmem windows.devicetree.DeviceTree
Volatility 3 Framework 2.5.0
Progress:  100.00               PDB scanning finished
Offset  Type    DriverName      DeviceName      DriverNameOfAttDevice   DeviceType

0x5ded2e0       DRV     -       N/A     N/A     N/A
* 0x5ded2e0     DEV     -       00000044        N/A     FILE_DEVICE_BUS_EXTENDER
** 0x5ded2e0    ATT     -       -       \Driver\ACPI    FILE_DEVICE_ACPI
0x5df52e0       DRV     -       N/A     N/A     N/A
* 0x5df52e0     DEV     -       WMIAdminDevice  N/A     FILE_DEVICE_UNKNOWN
0x5dfe060       DRV     -       N/A     N/A     N/A
* 0x5dfe060     DEV     -       RawTape N/A     FILE_DEVICE_TAPE_FILE_SYSTEM
0x5dfe310       DRV     -       N/A     N/A     N/A
* 0x5dfe310     DEV     -       -       N/A     FILE_DEVICE_ACPI
** 0x5dfe310    ATT     -       RaidPort0       \Driver\LSI_SAS FILE_DEVICE_CONTROLLER
0x12ab0301      DRV     -       N/A     N/A     N/A
0x7ac546dc      DRV     -       N/A     N/A     N/A
0x7dd1a990      DRV     -       N/A     N/A     N/A
* 0x7dd1a990    DEV     -       -       N/A     FILE_DEVICE_BUS_EXTENDER
0x7dd3bb00      DRV     -       N/A     N/A     N/A
* 0x7dd3bb00    DEV     -       Srv2    N/A     FILE_DEVICE_NETWORK_FILE_SYSTEM
0x7dd3ce70      DRV     -       N/A     N/A     N/A
* 0x7dd3ce70    DEV     -       LanmanServer    N/A     FILE_DEVICE_NETWORK
0x7dec3240      DRV     -       N/A     N/A     N/A
* 0x7dec3240    DEV     -       lltdio  N/A     FILE_DEVICE_NETWORK
0x7decde70      DRV     -       N/A     N/A     N/A
* 0x7decde70    DEV     -       rspndr  N/A     FILE_DEVICE_NETWORK
0x7df46300      DRV     -       N/A     N/A     N/A
* 0x7df46300    DEV     -       ReqQueue        N/A     FILE_DEVICE_NETWORK
0x7df5b420      DRV     -       N/A     N/A     N/A
0x7df82b30      DRV     -       N/A     N/A     N/A
* 0x7df82b30    DEV     -       Secdrv  N/A     UNKNOWN
0x7df91060      DRV     -       N/A     N/A     N/A
* 0x7df91060    DEV     -       LanmanDatagramReceiver  N/A     FILE_DEVICE_NETWORK_BROWSER
0x7df94e70      DRV     -       N/A     N/A     N/A
* 0x7df94e70    DEV     -       MPS     N/A     UNKNOWN
0x7df99060      DRV     -       N/A     N/A     N/A
* 0x7df99060    DEV     -       -       N/A     FILE_DEVICE_NETWORK_FILE_SYSTEM
0x7df9e780      DRV     -       N/A     N/A     N/A
0x7dfaa060      DRV     -       N/A     N/A     N/A
0x7dfcf060      DRV     -       N/A     N/A     N/A
* 0x7dfcf060    DEV     -       vmmemctl        N/A     FILE_DEVICE_UNKNOWN
0x7dfd4aa0      DRV     -       N/A     N/A     N/A
* 0x7dfd4aa0    DEV     -       PEAuth  N/A     FILE_DEVICE_UNKNOWN
0x7e1ac8a0      DRV     -       N/A     N/A     N/A
0x7ea7b770      DRV     -       N/A     N/A     N/A
* 0x7ea7b770    DEV     -       000000ab        N/A     FILE_DEVICE_UNKNOWN
** 0x7ea7b770   ATT     -       -       \Driver\mouhid  FILE_DEVICE_MOUSE
*** 0x7ea7b770  ATT     -       -       \Driver\vmusbmouse      FILE_DEVICE_MOUSE
**** 0x7ea7b770 ATT     -       PointerClass3   \Driver\mouclass        FILE_DEVICE_MOUSE
0x7ea86d80      DRV     -       N/A     N/A     N/A
* 0x7ea86d80    DEV     -       -       N/A     FILE_DEVICE_MOUSE
** 0x7ea86d80   ATT     -       -       \Driver\vmusbmouse      FILE_DEVICE_MOUSE
*** 0x7ea86d80  ATT     -       PointerClass3   \Driver\mouclass        FILE_DEVICE_MOUSE
0x7ea8c060      DRV     -       N/A     N/A     N/A
* 0x7ea8c060    DEV     -       000000ae        N/A     FILE_DEVICE_UNKNOWN
** 0x7ea8c060   ATT     -       NDMP12  \Driver\BthPan  FILE_DEVICE_PHYSICAL_NETCARD
0x7eaab060      DRV     -       N/A     N/A     N/A
* 0x7eaab060    DEV     -       BTHMS_RFCOMM    N/A     FILE_DEVICE_NETWORK
0x7eaae630      DRV     -       N/A     N/A     N/A
* 0x7eaae630    DEV     -       BthEnum1        N/A     FILE_DEVICE_NULL
0x7eabb060      DRV     -       N/A     N/A     N/A
* 0x7eabb060    DEV     -       BthPan  N/A     FILE_DEVICE_NETWORK
0x7eac42a0      DRV     -       N/A     N/A     N/A
0x7eda4060      DRV     -       N/A     N/A     N/A
* 0x7eda4060    DEV     -       000000a4        N/A     FILE_DEVICE_KS
** 0x7eda4060   ATT     -       000000a5        \Driver\ksthunk FILE_DEVICE_KS
0x7eda4e70      DRV     -       N/A     N/A     N/A
* 0x7eda4e70    DEV     -       000000a5        N/A     FILE_DEVICE_KS
0x7f20b370      DRV     -       N/A     N/A     N/A
* 0x7f20b370    DEV     -       -       N/A     FILE_DEVICE_8042_PORT
** 0x7f20b370   ATT     -       -       \Driver\vmmouse FILE_DEVICE_MOUSE
*** 0x7f20b370  ATT     -       PointerClass0   \Driver\mouclass        FILE_DEVICE_MOUSE
0x7f222960      DRV     -       N/A     N/A     N/A
* 0x7f222960    DEV     -       NDProxy N/A     FILE_DEVICE_NETWORK
0x7f233260      DRV     -       N/A     N/A     N/A
* 0x7f233260    DEV     -       000000a9        N/A     FILE_DEVICE_UNKNOWN
** 0x7f233260   ATT     -       _HID00000001    \Driver\HidUsb  FILE_DEVICE_UNKNOWN
0x7f237e70      DRV     -       N/A     N/A     N/A
* 0x7f237e70    DEV     -       -       N/A     FILE_DEVICE_UNKNOWN
0x7f2542c0      DRV     -       N/A     N/A     N/A
* 0x7f2542c0    DEV     -       -       N/A     FILE_DEVICE_BATTERY
0x7f262060      DRV     -       N/A     N/A     N/A
* 0x7f262060    DEV     -       NDMP4   N/A     FILE_DEVICE_PHYSICAL_NETCARD
0x7f262470      DRV     -       N/A     N/A     N/A
* 0x7f262470    DEV     -       -       N/A     FILE_DEVICE_UNKNOWN
0x7f2655b0      DRV     -       N/A     N/A     N/A
* 0x7f2655b0    DEV     -       -       N/A     FILE_DEVICE_BUS_EXTENDER
0x7f26ccf0      DRV     -       N/A     N/A     N/A
* 0x7f26ccf0    DEV     -       NDMP5   N/A     FILE_DEVICE_PHYSICAL_NETCARD
0x7f26e590      DRV     -       N/A     N/A     N/A
* 0x7f26e590    DEV     -       NdisTapi        N/A     UNKNOWN
0x7f271a90      DRV     -       N/A     N/A     N/A
* 0x7f271a90    DEV     -       NdisWan N/A     FILE_DEVICE_NETWORK
0x7f27aa70      DRV     -       N/A     N/A     N/A
* 0x7f27aa70    DEV     -       NDMP9   N/A     FILE_DEVICE_PHYSICAL_NETCARD
0x7f27b060      DRV     -       N/A     N/A     N/A
* 0x7f27b060    DEV     -       NDMP10  N/A     FILE_DEVICE_PHYSICAL_NETCARD
0x7f27f8c0      DRV     -       N/A     N/A     N/A
* 0x7f27f8c0    DEV     -       NDMP11  N/A     FILE_DEVICE_PHYSICAL_NETCARD
0x7f286e70      DRV     -       N/A     N/A     N/A
* 0x7f286e70    DEV     -       RdpBus  N/A     FILE_DEVICE_UNKNOWN
0x7f289a40      DRV     -       N/A     N/A     N/A
* 0x7f289a40    DEV     -       -       N/A     FILE_DEVICE_BUS_EXTENDER
0x7f29be30      DRV     -       N/A     N/A     N/A
* 0x7f29be30    DEV     -       -       N/A     FILE_DEVICE_BUS_EXTENDER
0x7f2c1cb0      DRV     -       N/A     N/A     N/A
* 0x7f2c1cb0    DEV     -       USBPDO-0        N/A     FILE_DEVICE_BUS_EXTENDER
** 0x7f2c1cb0   ATT     -       000000a1        \Driver\usbhub  UNKNOWN
0x7f2dc980      DRV     -       N/A     N/A     N/A
* 0x7f2dc980    DEV     -       USBPDO-4        N/A     FILE_DEVICE_UNKNOWN
** 0x7f2dc980   ATT     -       -       \Driver\BTHUSB  UNKNOWN
0x7f304060      DRV     -       N/A     N/A     N/A
* 0x7f304060    DEV     -       USBPDO-1        N/A     FILE_DEVICE_BUS_EXTENDER
** 0x7f304060   ATT     -       000000a2        \Driver\usbhub  UNKNOWN
0x7f4ab4e0      DRV     -       N/A     N/A     N/A
* 0x7f4ab4e0    DEV     -       INTELPRO_{7F5B9219-B869-4AEA-84AF-CC6E4C2486FA} N/A     FILE_DEVICE_NETWORK
0x7f60a820      DRV     -       N/A     N/A     N/A
* 0x7f60a820    DEV     -       Nsi     N/A     FILE_DEVICE_NETWORK
0x7f60c930      DRV     -       N/A     N/A     N/A
* 0x7f60c930    DEV     -       -       N/A     FILE_DEVICE_UNKNOWN
0x7f60e9d0      DRV     -       N/A     N/A     N/A
* 0x7f60e9d0    DEV     -       DfsClient       N/A     FILE_DEVICE_DISK_FILE_SYSTEM
0x7f60ee70      DRV     -       N/A     N/A     N/A
0x7f610740      DRV     -       N/A     N/A     N/A
* 0x7f610740    DEV     -       -       N/A     FILE_DEVICE_NETWORK_FILE_SYSTEM
0x7f614a90      DRV     -       N/A     N/A     N/A
* 0x7f614a90    DEV     -       BlbControl      N/A     FILE_DEVICE_NETWORK
0x7f61a930      DRV     -       N/A     N/A     N/A
* 0x7f61a930    DEV     -       NDMP2   N/A     FILE_DEVICE_PHYSICAL_NETCARD
0x7f64c240      DRV     -       N/A     N/A     N/A
* 0x7f64c240    DEV     -       KeyboardClass1  N/A     FILE_DEVICE_KEYBOARD
0x7f660970      DRV     -       N/A     N/A     N/A
* 0x7f660970    DEV     -       PointerClass3   N/A     FILE_DEVICE_MOUSE
0x7f660c20      DRV     -       N/A     N/A     N/A
* 0x7f660c20    DEV     -       -       N/A     FILE_DEVICE_MOUSE
** 0x7f660c20   ATT     -       PointerClass0   \Driver\mouclass        FILE_DEVICE_MOUSE
0x7f67ec90      DRV     -       N/A     N/A     N/A
* 0x7f67ec90    DEV     -       -       N/A     FILE_DEVICE_BUS_EXTENDER
0x7f6b01e0      DRV     -       N/A     N/A     N/A
* 0x7f6b01e0    DEV     -       Video5  N/A     FILE_DEVICE_VIDEO
0x7f6b0db0      DRV     -       N/A     N/A     N/A
* 0x7f6b0db0    DEV     -       000000a3        N/A     FILE_DEVICE_SOUND
** 0x7f6b0db0   ATT     -       000000a4        \Driver\HdAudAddService FILE_DEVICE_KS
*** 0x7f6b0db0  ATT     -       000000a5        \Driver\ksthunk FILE_DEVICE_KS
0x7f7322b0      DRV     -       N/A     N/A     N/A
* 0x7f7322b0    DEV     -       DxgKrnl N/A     FILE_DEVICE_UNKNOWN
0x7f85f710      DRV     -       N/A     N/A     N/A
* 0x7f85f710    DEV     -       -       N/A     FILE_DEVICE_DISK_FILE_SYSTEM
** 0x7f85f710   ATT     -       -       \FileSystem\FltMgr      FILE_DEVICE_DISK_FILE_SYSTEM
0x7f863550      DRV     -       N/A     N/A     N/A
* 0x7f863550    DEV     -       -       N/A     FILE_DEVICE_DISK_FILE_SYSTEM
0x7f867550      DRV     -       N/A     N/A     N/A
* 0x7f867550    DEV     -       FileInfo        N/A     FILE_DEVICE_UNKNOWN
0x7f869550      DRV     -       N/A     N/A     N/A
0x7f86b2c0      DRV     -       N/A     N/A     N/A
* 0x7f86b2c0    DEV     -       PcwDrv  N/A     FILE_DEVICE_UNKNOWN
0x7f871c50      DRV     -       N/A     N/A     N/A
0x7f877360      DRV     -       N/A     N/A     N/A
* 0x7f877360    DEV     -       CNG     N/A     UNKNOWN
0x7f877550      DRV     -       N/A     N/A     N/A
* 0x7f877550    DEV     -       KsecDD  N/A     FILE_DEVICE_KSEC
0x7f877c40      DRV     -       N/A     N/A     N/A
* 0x7f877c40    DEV     -       Ndis    N/A     FILE_DEVICE_NETWORK
0x7f87d400      DRV     -       N/A     N/A     N/A
* 0x7f87d400    DEV     -       eQoS    N/A     FILE_DEVICE_NETWORK
0x7f89f550      DRV     -       N/A     N/A     N/A
* 0x7f89f550    DEV     -       ExFatRecognizer N/A     FILE_DEVICE_DISK_FILE_SYSTEM
0x7f8ff460      DRV     -       N/A     N/A     N/A
0x7f9156d0      DRV     -       N/A     N/A     N/A
* 0x7f9156d0    DEV     -       RdyBoost        N/A     FILE_DEVICE_UNKNOWN
0x7f91b6d0      DRV     -       N/A     N/A     N/A
* 0x7f91b6d0    DEV     -       HarddiskVolumeShadowCopy5       N/A     FILE_DEVICE_VIRTUAL_DISK
0x7f92f660      DRV     -       N/A     N/A     N/A
* 0x7f92f660    DEV     -       SPDevice        N/A     FILE_DEVICE_UNKNOWN
0x7f931430      DRV     -       N/A     N/A     N/A
* 0x7f931430    DEV     -       -       N/A     FILE_DEVICE_DISK
** 0x7f931430   ATT     -       -       \Driver\volsnap FILE_DEVICE_DISK
0x7f93b3f0      DRV     -       N/A     N/A     N/A
* 0x7f93b3f0    DEV     -       Mup     N/A     FILE_DEVICE_NETWORK_FILE_SYSTEM
** 0x7f93b3f0   ATT     -       -       \FileSystem\FltMgr      FILE_DEVICE_NETWORK_FILE_SYSTEM
0x7f93d480      DRV     -       N/A     N/A     N/A
* 0x7f93d480    DEV     -       DR0     N/A     FILE_DEVICE_DISK
** 0x7f93d480   ATT     -       -       \Driver\partmgr FILE_DEVICE_DISK
0x7f93d670      DRV     -       N/A     N/A     N/A
0x7f987e70      DRV     -       N/A     N/A     N/A
* 0x7f987e70    DEV     -       NetBT_Tcpip_{965ABEC5-556B-460C-8CE4-11F9DA96FBAC}      N/A     FILE_DEVICE_NETWORK
0x7f9a99d0      DRV     -       N/A     N/A     N/A
* 0x7f9a99d0    DEV     -       CdRom0  N/A     FILE_DEVICE_CD_ROM
0x7f9abe70      DRV     -       N/A     N/A     N/A
* 0x7f9abe70    DEV     -       Beep    N/A     FILE_DEVICE_BEEP
0x7f9ada20      DRV     -       N/A     N/A     N/A
* 0x7f9ada20    DEV     -       Null    N/A     FILE_DEVICE_NULL
0x7f9b58a0      DRV     -       N/A     N/A     N/A
0x7f9b9430      DRV     -       N/A     N/A     N/A
* 0x7f9b9430    DEV     -       Video0  N/A     FILE_DEVICE_VIDEO
0x7f9b9620      DRV     -       N/A     N/A     N/A
* 0x7f9b9620    DEV     -       Video3  N/A     FILE_DEVICE_VIDEO
0x7f9bbcf0      DRV     -       N/A     N/A     N/A
* 0x7f9bbcf0    DEV     -       Video1  N/A     FILE_DEVICE_VIDEO
0x7f9c1990      DRV     -       N/A     N/A     N/A
* 0x7f9c1990    DEV     -       Video2  N/A     FILE_DEVICE_VIDEO
0x7f9c34f0      DRV     -       N/A     N/A     N/A
* 0x7f9c34f0    DEV     -       NamedPipe       N/A     FILE_DEVICE_NAMED_PIPE
0x7f9c77d0      DRV     -       N/A     N/A     N/A
* 0x7f9c77d0    DEV     -       Mailslot        N/A     FILE_DEVICE_MAILSLOT
0x7f9c9920      DRV     -       N/A     N/A     N/A
* 0x7f9c9920    DEV     -       RawIp6  N/A     FILE_DEVICE_NETWORK
0x7f9d3660      DRV     -       N/A     N/A     N/A
* 0x7f9d3660    DEV     -       Afd     N/A     FILE_DEVICE_NAMED_PIPE
0x7f9db8c0      DRV     -       N/A     N/A     N/A
* 0x7f9db8c0    DEV     -       WS2IFSL N/A     FILE_DEVICE_NAMED_PIPE
0x7f9ddc00      DRV     -       N/A     N/A     N/A
* 0x7f9ddc00    DEV     -       Psched  N/A     FILE_DEVICE_NETWORK
0x7f9dfd40      DRV     -       N/A     N/A     N/A
0x7f9e58f0      DRV     -       N/A     N/A     N/A
* 0x7f9e58f0    DEV     -       Netbios N/A     FILE_DEVICE_TRANSPORT
0x7f9e7d90      DRV     -       N/A     N/A     N/A
* 0x7f9e7d90    DEV     -       hgfsInternal    N/A     UNKNOWN
0x7f9efa20      DRV     -       N/A     N/A     N/A
* 0x7f9efa20    DEV     -       WANARPV6        N/A     FILE_DEVICE_NETWORK
0x7f9efc10      DRV     -       N/A     N/A     N/A
* 0x7f9efc10    DEV     -       Serial0 N/A     FILE_DEVICE_SERIAL_PORT
** 0x7f9efc10   ATT     -       -       \Driver\Serenum FILE_DEVICE_BUS_EXTENDER
0x7f9f3650      DRV     -       N/A     N/A     N/A
* 0x7f9f3650    DEV     -       -       N/A     FILE_DEVICE_8042_PORT
** 0x7f9f3650   ATT     -       PointerClass1   \Driver\mouclass        FILE_DEVICE_MOUSE
0x7f9fb600      DRV     -       N/A     N/A     N/A
* 0x7f9fb600    DEV     -       FsWrap  N/A     FILE_DEVICE_NETWORK_FILE_SYSTEM
0x7fafb260      DRV     -       N/A     N/A     N/A
* 0x7fafb260    DEV     -       -       N/A     FILE_DEVICE_UNKNOWN
0x7fb0d060      DRV     -       N/A     N/A     N/A
* 0x7fb0d060    DEV     -       -       N/A     FILE_DEVICE_MOUSE
** 0x7fb0d060   ATT     -       PointerClass3   \Driver\mouclass        FILE_DEVICE_MOUSE
0x7fb717c0      DRV     -       N/A     N/A     N/A
* 0x7fb717c0    DEV     -       -       N/A     FILE_DEVICE_DISK
0x7fb727c0      DRV     -       N/A     N/A     N/A
* 0x7fb727c0    DEV     -       CompositeBattery        N/A     FILE_DEVICE_BATTERY
0x7fb737c0      DRV     -       N/A     N/A     N/A
* 0x7fb737c0    DEV     -       HarddiskVolume1 N/A     FILE_DEVICE_DISK
** 0x7fb737c0   ATT     -       -       \Driver\fvevol  FILE_DEVICE_DISK
*** 0x7fb737c0  ATT     -       -       \Driver\volsnap FILE_DEVICE_DISK
0x7fb787c0      DRV     -       N/A     N/A     N/A
0x7fb797c0      DRV     -       N/A     N/A     N/A
* 0x7fb797c0    DEV     -       PciIde0Channel1 N/A     FILE_DEVICE_CONTROLLER
** 0x7fb797c0   ATT     -       IdePort1        \Driver\atapi   FILE_DEVICE_CONTROLLER
0x7fb7c7c0      DRV     -       N/A     N/A     N/A
* 0x7fb7c7c0    DEV     -       MountPointManager       N/A     FILE_DEVICE_NETWORK
0x7fb7d120      DRV     -       N/A     N/A     N/A
* 0x7fb7d120    DEV     -       NTPNP_PCI0045   N/A     FILE_DEVICE_CONTROLLER
** 0x7fb7d120   ATT     -       -       \Driver\ACPI    FILE_DEVICE_ACPI
*** 0x7fb7d120  ATT     -       RaidPort0       \Driver\LSI_SAS FILE_DEVICE_CONTROLLER
0x7fba17c0      DRV     -       N/A     N/A     N/A
* 0x7fba17c0    DEV     -       vmci    N/A     FILE_DEVICE_UNKNOWN
0x7fba27c0      DRV     -       N/A     N/A     N/A
* 0x7fba27c0    DEV     -       IdeDeviceP3T0L0-5       N/A     FILE_DEVICE_CD_ROM
** 0x7fba27c0   ATT     -       CdRom0  \Driver\cdrom   FILE_DEVICE_CD_ROM
0x7fba57c0      DRV     -       N/A     N/A     N/A
* 0x7fba57c0    DEV     -       0000009f        N/A     FILE_DEVICE_DISK
** 0x7fba57c0   ATT     -       DR0     \Driver\Disk    FILE_DEVICE_DISK
*** 0x7fba57c0  ATT     -       -       \Driver\partmgr FILE_DEVICE_DISK
0x7fba77c0      DRV     -       N/A     N/A     N/A
* 0x7fba77c0    DEV     -       PciIde1Channel29        N/A     FILE_DEVICE_CONTROLLER
** 0x7fba77c0   ATT     -       IdePort31       \Driver\atapi   FILE_DEVICE_CONTROLLER
0x7fbd64b0      DRV     -       N/A     N/A     N/A
* 0x7fbd64b0    DEV     -       VMCIGuestDev    N/A     FILE_DEVICE_CONTROLLER
0x7fc05c50      DRV     -       N/A     N/A     N/A
* 0x7fc05c50    DEV     -       -       N/A     FILE_DEVICE_UNKNOWN
0x7fe199f0      DRV     -       N/A     N/A     N/A
* 0x7fe199f0    DEV     -       00000043        N/A     FILE_DEVICE_CONTROLLER
** 0x7fe199f0   ATT     -       VolMgrControl   \Driver\volmgr  FILE_DEVICE_NETWORK
0x7fe609b0      DRV     -       N/A     N/A     N/A
* 0x7fe609b0    DEV     -       clfs    N/A     FILE_DEVICE_DISK_FILE_SYSTEM
0x7fe6f060      DRV     -       N/A     N/A     N/A
* 0x7fe6f060    DEV     -       SrvNet  N/A     FILE_DEVICE_NETWORK_FILE_SYSTEM
0x7fe9ecd0      DRV     -       N/A     N/A     N/A
* 0x7fe9ecd0    DEV     -       KMDF0   N/A     FILE_DEVICE_UNKNOWN

```

# windows.devicetree.DeviceTree 分析

## 1. Plugin 功能說明

`windows.devicetree.DeviceTree` 用來列出 Windows 系統中的 Driver Object、Device Object，以及裝置堆疊中的 Attached Device。

在 Windows 中，Driver 會建立 Device Object，其他 Driver 也可以附掛在 Device Stack 上，用來攔截或處理 I/O Request。

在數位鑑識中，此 Plugin 可用來檢查：

```text
是否存在可疑 Driver
是否存在異常 Device Object
是否有不明 Driver 附掛在磁碟、網路、鍵盤、滑鼠等裝置堆疊
是否有疑似 Rootkit 或 Kernel-level Hooking 行為
```

---

## 2. 執行指令

```bash
.\vol.exe -f .\OtterCTF.vmem windows.devicetree.DeviceTree
```

---

## 3. 欄位說明

| 欄位                      | 說明                              |
| ----------------------- | ------------------------------- |
| `Offset`                | Driver / Device Object 在記憶體中的位置 |
| `Type`                  | 物件類型，包含 DRV、DEV、ATT             |
| `DriverName`            | Driver 名稱                       |
| `DeviceName`            | Device Object 名稱                |
| `DriverNameOfAttDevice` | 附掛裝置所屬 Driver                   |
| `DeviceType`            | 裝置類型                            |

其中：

```text
DRV = Driver Object
DEV = Device Object
ATT = Attached Device
```

---

## 4. 執行結果摘要

本次結果中可以看到多種正常 Windows 裝置類型，例如：

```text
FILE_DEVICE_DISK
FILE_DEVICE_NETWORK
FILE_DEVICE_MOUSE
FILE_DEVICE_KEYBOARD
FILE_DEVICE_CD_ROM
FILE_DEVICE_NAMED_PIPE
FILE_DEVICE_DISK_FILE_SYSTEM
FILE_DEVICE_NETWORK_FILE_SYSTEM
FILE_DEVICE_BUS_EXTENDER
```

這些大多屬於 Windows 系統正常裝置、網路裝置、磁碟裝置、輸入裝置與檔案系統裝置。

---

## 5. VMware 相關裝置觀察

結果中出現多個 VMware 相關 Device / Driver，例如：

```text
vmci
VMCIGuestDev
vmmemctl
vmusbmouse
vmmouse
vmhgfs
```

也看到 VMware 滑鼠裝置附掛關係，例如：

```text
\Driver\vmusbmouse
\Driver\vmmouse
\Driver\mouclass
```

這些結果與前面 `SvcScan`、`DriverScan`、`DriverIrp`、`Modules` 中看到的 VMware Tools / VMware Driver 結果一致。

由於本案記憶體映像來自 VMware 虛擬機環境，因此 VMware 相關裝置屬於合理現象。

---

## 6. 磁碟與檔案系統裝置觀察

結果中可看到磁碟與檔案系統相關裝置，例如：

```text
HarddiskVolume1
DR0
Disk
partmgr
volsnap
fvevol
FltMgr
FileInfo
Ntfs
Mup
DfsClient
```

其中 `HarddiskVolume1`、`DR0`、`Disk`、`partmgr` 屬於正常磁碟裝置堆疊。

`FltMgr` 與 `FileInfo` 屬於 Windows 檔案系統 Filter / Minifilter 架構中常見的元件。

本次沒有看到明確可疑 Driver 附掛在磁碟或檔案系統裝置堆疊上。

---

## 7. 網路裝置觀察

結果中也看到多個網路相關裝置，例如：

```text
Afd
Tcpip
Ndis
NetBT
LanmanServer
SrvNet
Srv2
Srv
Psched
Netbios
INTELPRO_{...}
```

這些大多屬於 Windows 網路堆疊或網卡相關裝置。

目前沒有看到與 `Rick And Morty`、`vmware-tray.exe` 或可疑惡意 Driver 直接相關的網路裝置附掛。

---

## 8. 輸入裝置觀察

結果中可看到滑鼠與鍵盤相關裝置，例如：

```text
PointerClass0
PointerClass1
PointerClass3
KeyboardClass1
mouclass
mouhid
vmusbmouse
vmmouse
```

這些結果與 VMware 虛擬機滑鼠 / 鍵盤環境相符，沒有看到疑似 Keylogger Driver 或不明輸入裝置附掛。

---

## 9. 可疑項目檢查

本次 `DeviceTree` 沒有看到以下與本案主線直接相關的名稱：

```text
Rick And Morty
vmware-tray
RarSFX0
READ_IT
ransom
encrypt
crypt
```

也沒有看到明確不明 Driver 附掛在磁碟、網路或鍵盤滑鼠裝置堆疊上。

雖然結果中有部分 DriverName 顯示為 `-` 或 `N/A`，但這在 Volatility 解析 Device Object 時並不少見，不能單獨判斷為惡意。

## 10. 與其他 Plugin 的關聯

此結果可與前面 Kernel 層分析互相補強：

```text
Modules：未發現明確可疑 Kernel Module
ModScan：未發現明確隱藏 Driver
DriverScan：未發現明確可疑 Driver
DriverIrp：未發現明確可疑 IRP Hook
DriverModule：未發現明確 Driver Rootkit
Callbacks：未發現明確可疑 Callback
SSDT：未發現明確 SSDT Hook
DeviceTree：未發現明確可疑 Device Stack 附掛
```

這些結果整體支持：本案目前不像是 Kernel-mode Rootkit 或 Driver-level 攻擊。
