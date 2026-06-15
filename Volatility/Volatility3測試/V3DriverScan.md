# 測試內容
- .\vol.exe -f .\OtterCTF.vmem windows.driverscan.DriverScan


```
D:\Forensic\G140A006\VolatilityWorkbench>.\vol.exe -f .\OtterCTF.vmem windows.driverscan.DriverScan
Volatility 3 Framework 2.5.0
Progress:  100.00               PDB scanning finished
Offset  Start   Size    Service Key     Driver Name     Name

0x5ded2e0       0xf80002a09000  0x0     \Driver\ACPI_HAL        N/A     \Driver\ACPI_HAL
0x5df52e0       0xf80002a52000  0x0     \Driver\WMIxWDM N/A     \Driver\WMIxWDM
0x5dfe060       0x0     0x0             N/A     \FileSystem\RAW
0x5dfe310       0xf88000e00000  0x57000 ACPI    N/A     \Driver\ACPI
0x12ab0301      0x100b8000800   0x0     N/A     N/A     N/A
0x7ac546dc      0x7419000a1901  0x86419 N/A     N/A     N/A
0x7dd1a990      0xf88000e9d000  0xd000  vdrvroot        N/A     \Driver\vdrvroot
0x7dd3bb00      0xf88003400000  0x6b000 srv2    N/A     \FileSystem\srv2
0x7dd3ce70      0xf88004a0d000  0x99000 srv     N/A     \FileSystem\srv
0x7dec3240      0xf8800459a000  0x15000 lltdio  N/A     \Driver\lltdio
0x7decde70      0xf880045af000  0x18000 rspndr  N/A     \Driver\rspndr
0x7df46300      0xf88002a33000  0xc9000 HTTP    N/A     \Driver\HTTP
0x7df5b420      0xf8800358d000  0x12000 tcpipreg        N/A     \Driver\tcpipreg
0x7df82b30      0xf88003551000  0xb000  secdrv  N/A     \Driver\secdrv
0x7df91060      0xf88002afc000  0x1e000 bowser  N/A     \FileSystem\bowser
0x7df94e70      0xf88002b1a000  0x18000 mpsdrv  N/A     \Driver\mpsdrv
0x7df99060      0xf88002b32000  0x2d000 mrxsmb  N/A     \FileSystem\mrxsmb
0x7df9e780      0xf88002b5f000  0x4d000 mrxsmb10        N/A     \FileSystem\mrxsmb10
0x7dfaa060      0xf88002bac000  0x24000 mrxsmb20        N/A     \FileSystem\mrxsmb20
0x7dfcf060      0xf88002bd0000  0xa000  VMMEMCTL        N/A     \Driver\VMMEMCTL
0x7dfd4aa0      0xf880034ab000  0xa6000 PEAUTH  N/A     \Driver\PEAUTH
0x7e1ac8a0      0xf88004577000  0x23000 luafv   N/A     \FileSystem\luafv
0x7ea7b770      0xf8800433d000  0xe000  HidUsb  N/A     \Driver\HidUsb
0x7ea86d80      0xf8800436d000  0xd000  mouhid  N/A     \Driver\mouhid
0x7ea8c060      0xf88004383000  0x18000 BTHUSB  N/A     \Driver\BTHUSB
0x7eaab060      0xf88004501000  0x2c000 RFCOMM  N/A     \Driver\RFCOMM
0x7eaae630      0xf8800452d000  0x10000 BthEnum N/A     \Driver\BthEnum
0x7eabb060      0xf88004549000  0x20000 BthPan  N/A     \Driver\BthPan
0x7eac42a0      0xf960000e0000  0x0     \Driver\Win32k  N/A     \Driver\Win32k
0x7eda4060      0xf88003e15000  0x5c000 HdAudAddService N/A     \Driver\HdAudAddService
0x7eda4e70      0xf880042d0000  0x5200  ksthunk N/A     \Driver\ksthunk
0x7f20b370      0xf88003b62000  0x1e000 i8042prt        N/A     \Driver\i8042prt
0x7f222960      0xf88003e00000  0x15000 NDProxy N/A     \Driver\NDProxy
0x7f233260      0xf8800431e000  0x1d000 usbccgp N/A     \Driver\usbccgp
0x7f237e70      0xf88003be8000  0x16000 intelppm        N/A     \Driver\intelppm
0x7f2542c0      0xf88003dfb000  0x4500  CmBatt  N/A     \Driver\CmBatt
0x7f262060      0xf88002cb9000  0x16000 RasAgileVpn     N/A     \Driver\RasAgileVpn
0x7f262470      0xf88003a00000  0xa000  PNPMEM  N/A     \Driver\PNPMEM
0x7f2655b0      0xf88002ca9000  0x10000 CompositeBus    N/A     \Driver\CompositeBus
0x7f26ccf0      0xf88003e81000  0x24000 Rasl2tp N/A     \Driver\Rasl2tp
0x7f26e590      0xf88003ea5000  0xc000  NdisTapi        N/A     \Driver\NdisTapi
0x7f271a90      0xf88003eb1000  0x2f000 NdisWan N/A     \Driver\NdisWan
0x7f27aa70      0xf88003ee0000  0x1b000 RasPppoe        N/A     \Driver\RasPppoe
0x7f27b060      0xf88003efb000  0x21000 PptpMiniport    N/A     \Driver\PptpMiniport
0x7f27f8c0      0xf88003f1c000  0x1a000 RasSstp N/A     \Driver\RasSstp
0x7f286e70      0xf88003f36000  0xb000  rdpbus  N/A     \Driver\rdpbus
0x7f289a40      0xf88003f41000  0x1480  swenum  N/A     \Driver\swenum
0x7f29be30      0xf88003f86000  0x12000 umbus   N/A     \Driver\umbus
0x7f2c1cb0      0xf88003c46000  0xd000  usbuhci N/A     \Driver\usbuhci
0x7f2dc980      0xf88003f98000  0x5a000 usbhub  N/A     \Driver\usbhub
0x7f304060      0xf88003dea000  0x11000 usbehci N/A     \Driver\usbehci
0x7f4ab4e0      0xf88003ca9000  0x23980 E1G60   N/A     \Driver\E1G60
0x7f60a820      0xf88003a64000  0xc000  nsiproxy        N/A     \Driver\nsiproxy
0x7f60c930      0xf88003a70000  0xb000  mssmbios        N/A     \Driver\mssmbios
0x7f60e9d0      0xf88003b0d000  0x1e000 DfsC    N/A     \FileSystem\DfsC
0x7f60ee70      0xf88003a7b000  0xf000  discache        N/A     \Driver\discache
0x7f610740      0xf88003a8a000  0x83000 CSC     N/A     \Driver\CSC
0x7f614a90      0xf88003b2b000  0x11000 blbdrive        N/A     \Driver\blbdrive
0x7f61a930      0xf88003b3c000  0x26000 tunnel  N/A     \Driver\tunnel
0x7f64c240      0xf88003b80000  0xf000  kbdclass        N/A     \Driver\kbdclass
0x7f660970      0xf88003b97000  0xf000  mouclass        N/A     \Driver\mouclass
0x7f660c20      0xf88003b8f000  0x8000  vmmouse N/A     \Driver\vmmouse
0x7f67ec90      0xf88003ba6000  0xc000  Serenum N/A     \Driver\Serenum
0x7f6b01e0      0xf88003bb2000  0x36000 vm3dmp  N/A     \Driver\vm3dmp
0x7f6b0db0      0xf88003ccd000  0x24000 HDAudBus        N/A     \Driver\HDAudBus
0x7f7322b0      0xf88003cf6000  0xf4000 DXGKrnl N/A     \Driver\DXGKrnl
0x7f85f710      0xf8800125d000  0x1a3000        Ntfs    N/A     \FileSystem\Ntfs
0x7f863550      0xf8800116e000  0x4c000 FltMgr  N/A     \FileSystem\FltMgr
0x7f867550      0xf880011ba000  0x14000 FileInfo        N/A     \FileSystem\FileInfo
0x7f869550      0xf88001163000  0xb000  amdxata N/A     \Driver\amdxata
0x7f86b2c0      0xf880014e6000  0x11000 pcw     N/A     \Driver\pcw
0x7f871c50      0xf8800121b000  0x2b000 KSecPkg N/A     \Driver\KSecPkg
0x7f877360      0xf88001474000  0x72000 CNG     N/A     \Driver\CNG
0x7f877550      0xf88001200000  0x1b000 KSecDD  N/A     \Driver\KSecDD
0x7f877c40      0xf88001501000  0xf3000 NDIS    N/A     \Driver\NDIS
0x7f87d400      0xf88001637000  0x204000        Tcpip   N/A     \Driver\Tcpip
0x7f89f550      0xf880014f7000  0xa000  Fs_Rec  N/A     \FileSystem\Fs_Rec
0x7f8ff460      0xf88001885000  0x10000 storflt N/A     \Driver\storflt
0x7f9156d0      0xf880018e9000  0x3a000 rdyboost        N/A     \Driver\rdyboost
0x7f91b6d0      0xf88001895000  0x4c000 volsnap N/A     \Driver\volsnap
0x7f92f660      0xf880018e1000  0x8000  spldr   N/A     \Driver\spldr
0x7f931430      0xf8800193e000  0x3a000 fvevol  N/A     \Driver\fvevol
0x7f93b3f0      0xf88001923000  0x12000 Mup     N/A     \FileSystem\Mup
0x7f93d480      0xf88001978000  0x16000 Disk    N/A     \Driver\Disk
0x7f93d670      0xf88001935000  0x9000  hwpolicy        N/A     \Driver\hwpolicy
0x7f987e70      0xf88002d92000  0x45000 NetBT   N/A     \Driver\NetBT
0x7f9a99d0      0xf8800105e000  0x2a000 cdrom   N/A     \Driver\cdrom
0x7f9abe70      0xf8800161c000  0x7000  Beep    N/A     \Driver\Beep
0x7f9ada20      0xf88001613000  0x9000  Null    N/A     \Driver\Null
0x7f9b58a0      0xf88001623000  0xf000  vmrawdsk        N/A     \Driver\vmrawdsk
0x7f9b9430      0xf880019f3000  0x9000  RDPCDD  N/A     \Driver\RDPCDD
0x7f9b9620      0xf88001460000  0xe000  VgaSave N/A     \Driver\VgaSave
0x7f9bbcf0      0xf880015f4000  0x9000  RDPENCDD        N/A     \Driver\RDPENCDD
0x7f9c1990      0xf880011ce000  0x9000  RDPREFMP        N/A     \Driver\RDPREFMP
0x7f9c34f0      0xf880011e2000  0x11000 Npfs    N/A     \FileSystem\Npfs
0x7f9c77d0      0xf880011d7000  0xb000  Msfs    N/A     \FileSystem\Msfs
0x7f9c9920      0xf88002cda000  0x22000 tdx     N/A     \Driver\tdx
0x7f9d3660      0xf88002d09000  0x89000 AFD     N/A     \Driver\AFD
0x7f9db8c0      0xf88002dd7000  0xb000  ws2ifsl N/A     \Driver\ws2ifsl
0x7f9ddc00      0xf88002c00000  0x26000 Psched  N/A     \Driver\Psched
0x7f9dfd40      0xf88002de2000  0x9000  WfpLwf  N/A     \Driver\WfpLwf
0x7f9e58f0      0xf88002c26000  0xf000  NetBIOS N/A     \FileSystem\NetBIOS
0x7f9e7d90      0xf88002c35000  0x28000 vmhgfs  N/A     \FileSystem\vmhgfs
0x7f9efa20      0xf88002c7a000  0x1b000 Wanarpv6        N/A     \Driver\Wanarpv6
0x7f9efc10      0xf88002c5d000  0x1d000 Serial  N/A     \Driver\Serial
0x7f9f3650      0xf88002c95000  0x14000 TermDD  N/A     \Driver\TermDD
0x7f9fb600      0xf88003a13000  0x51000 rdbss   N/A     \FileSystem\rdbss
0x7fafb260      0xf88000e60000  0xa000  msisadrv        N/A     \Driver\msisadrv
0x7fb0d060      0xf8800437a000  0x9000  vmusbmouse      N/A     \Driver\vmusbmouse
0x7fb717c0      0xf88000eaa000  0x15000 partmgr N/A     \Driver\partmgr
0x7fb727c0      0xf88000ebf000  0x9000  Compbatt        N/A     \Driver\Compbatt
0x7fb737c0      0xf88000ed4000  0x15000 volmgr  N/A     \Driver\volmgr
0x7fb787c0      0xf88000da0000  0x5c000 volmgrx N/A     \Driver\volmgrx
0x7fb797c0      0xf88000ee9000  0x8000  intelide        N/A     \Driver\intelide
0x7fb7c7c0      0xf88000fd6000  0x1a000 mountmgr        N/A     \Driver\mountmgr
0x7fb7d120      0xf88000e6a000  0x33000 pci     N/A     \Driver\pci
0x7fba17c0      0xf88000c00000  0x17000 vsock   N/A     \Driver\vsock
0x7fba27c0      0xf88000ff0000  0x9000  atapi   N/A     \Driver\atapi
0x7fba57c0      0xf880010d8000  0x1d000 LSI_SAS N/A     \Driver\LSI_SAS
0x7fba77c0      0xf88001158000  0xb000  msahci  N/A     \Driver\msahci
0x7fbd64b0      0xf88000fbd000  0x19000 vmci    N/A     \Driver\vmci
0x7fc05c50      0xf88004569000  0xe000  monitor N/A     \Driver\monitor
0x7fe199f0      0xf80002a52000  0x0     \Driver\PnpManager      N/A     \Driver\PnpManager
0x7fe609b0      0xf88000c82000  0x5e000 CLFS    N/A     \Driver\CLFS
0x7fe6f060      0xf8800355c000  0x31000 srvnet  N/A     \FileSystem\srvnet
0x7fe9ecd0      0xf88000efa000  0xa4000 Wdf01000        N/A     \Driver\Wdf01000
```


# windows.driverscan.DriverScan 分析

## 1. Plugin 功能說明

`windows.driverscan.DriverScan` 用來掃描記憶體中的 Driver Object。

此 Plugin 會從記憶體中尋找可能存在的 Driver Object，而不只依賴系統正常鏈結結構，因此可以用來輔助發現：

```text
隱藏 Driver
已卸載但仍殘留的 Driver
可疑 Kernel Driver
Rootkit 相關 Driver Object
```

在數位鑑識中，`DriverScan` 常用於 Kernel Rootkit 檢查，確認系統中是否存在可疑或未知的驅動程式。

---

## 2. 執行指令

```bash
.\vol.exe -f .\OtterCTF.vmem windows.driverscan.DriverScan
```

---

## 3. 欄位說明

| 欄位            | 說明                     |
| ------------- | ---------------------- |
| `Offset`      | Driver Object 在記憶體中的位置 |
| `Start`       | Driver 載入的起始記憶體位址      |
| `Size`        | Driver 大小              |
| `Service Key` | Driver 對應的服務名稱         |
| `Driver Name` | Driver 名稱              |
| `Name`        | Driver Object 名稱       |

---

## 4. 執行結果摘要

本次結果中可看到大量正常 Windows Driver，例如：

```text
ACPI
Wdf01000
srv
srv2
HTTP
tcpipreg
secdrv
mpsdrv
mrxsmb
mrxsmb10
mrxsmb20
luafv
HidUsb
mouhid
BTHUSB
RFCOMM
BthEnum
Ntfs
FltMgr
FileInfo
KSecDD
NDIS
Tcpip
Disk
AFD
USBPORT
usbhub
WfpLwf
volmgr
pci
CLFS
```

這些大多是 Windows 系統、檔案系統、網路、USB、藍牙、磁碟與硬體相關驅動。

---

## 5. VMware 相關 Driver

結果中也出現多個 VMware 相關 Driver，例如：

```text
VMMEMCTL
vmmouse
vm3dmp
vmrawdsk
vmhgfs
vmusbmouse
vsock
vmci
```

這些與本案記憶體來源為 VMware 環境相符，因此目前不視為異常。

---

## 6. 需要注意的項目

結果中有兩筆較不完整的項目：

```text
0x12ab0301      0x100b8000800   0x0     N/A     N/A     N/A
0x7ac546dc      0x7419000a1901  0x86419 N/A     N/A     N/A
```

這兩筆沒有顯示 Service Key、Driver Name 或 Name，因此可能是：

```text
記憶體殘留資料
解析不完整的 Driver Object
誤判的掃描結果
已卸載或損壞的結構
```

由於它們沒有明確 Driver 名稱、路徑、Service Key，也沒有在前面的 `SSDT`、`Callbacks`、`DriverIrp` 中看到相關可疑 Hook，因此目前不能單獨判斷為惡意。
