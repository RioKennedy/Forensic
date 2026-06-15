# 測試內容

- .\vol.exe -f .\OtterCTF.vmem windows.svcscan.SvcScan

```
D:\Forensic\G140A006\VolatilityWorkbench>.\vol.exe -f .\OtterCTF.vmem windows.svcscan.SvcScan
Volatility 3 Framework 2.5.0
Progress:  100.00               PDB scanning finished
Offset  Order   PID     Start   State   Type    Name    Display Binary

0x93f370        202     1012    SERVICE_DEMAND_START    SERVICE_RUNNING SERVICE_WIN32_SHARE_PROCESS      netprofm        Network List Service    C:\Windows\system32\svchost.exe -k LocalService
0x93f370        201     N/A     SERVICE_DISABLED        SERVICE_STOPPED SERVICE_WIN32_SHARE_PROCESS      NetPipeActivator        Net.Pipe Listener Adapter       N/A
0x93fea0        200     N/A     SERVICE_DISABLED        SERVICE_STOPPED SERVICE_WIN32_SHARE_PROCESS      NetMsmqActivator        Net.Msmq Listener Adapter       N/A
0x93fda0        199     844     SERVICE_DEMAND_START    SERVICE_RUNNING SERVICE_WIN32_SHARE_PROCESS      Netman  Network Connections     C:\Windows\System32\svchost.exe -k LocalSystemNetworkRestricted
0x93f280        198     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_WIN32_SHARE_PROCESS      Netlogon        Netlogon        N/A
0x93f190        197     N/A     SERVICE_SYSTEM_START    SERVICE_RUNNING SERVICE_KERNEL_DRIVER   NetBT    NetBT   \Driver\NetBT
0x93f0a0        196     N/A     SERVICE_SYSTEM_START    SERVICE_RUNNING SERVICE_FILE_SYSTEM_DRIVER       NetBIOS NetBIOS Interface       \FileSystem\NetBIOS
0x93efb0        195     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   NDProxy  NDIS Proxy      N/A
0x93eec0        194     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   NdisWan  Remote Access NDIS WAN Driver   N/A
0x93edd0        193     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   Ndisuio  NDIS Usermode I/O Protocol      N/A
0x93ece0        192     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   NdisTapi Remote Access NDIS TAPI Driver  N/A
0x93ebf0        191     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   NdisCap  NDIS Capture LightWeight Filter N/A
0x93eb00        190     N/A     SERVICE_BOOT_START      SERVICE_RUNNING SERVICE_KERNEL_DRIVER   NDIS     NDIS System Driver      \Driver\NDIS
0x93ea10        189     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   NativeWifiP      NativeWiFi Filter       N/A
0x93e920        188     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_WIN32_SHARE_PROCESS      napagent        Network Access Protection Agent N/A
0x93e830        187     N/A     SERVICE_BOOT_START      SERVICE_RUNNING SERVICE_FILE_SYSTEM_DRIVER       Mup     Mup     \FileSystem\Mup
0x93fcc0        186     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   MTConfig Microsoft Input Configuration Driver    N/A
0x93e740        185     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   MSTEE    Microsoft Streaming Tee/Sink-to-Sink Converter  N/A
0x93e650        184     N/A     SERVICE_SYSTEM_START    SERVICE_RUNNING SERVICE_KERNEL_DRIVER   mssmbios Microsoft System Management BIOS Driver \Driver\mssmbios
0x93e560        183     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   MsRPC    MsRPC   N/A
0x93e470        182     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   MSPQM    Microsoft Streaming Quality Manager Proxy       N/A
0x93e380        181     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   MSPCLOCK Microsoft Streaming Clock Proxy N/A
0x93e290        180     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   MSKSSRV  Microsoft Streaming Service Proxy       N/A
0x93e1a0        179     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_WIN32_OWN_PROCESSmsiserver       Windows Installer       N/A
0x93e0b0        178     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_WIN32_SHARE_PROCESS      MSiSCSI Microsoft iSCSI Initiator Service       N/A
0x93dfc0        177     N/A     SERVICE_BOOT_START      SERVICE_RUNNING SERVICE_KERNEL_DRIVER   msisadrv msisadrv        \Driver\msisadrv
0x93ded0        176     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   mshidkmdf        Pass-through HID to KMDF Filter Driver  N/A
0x93dde0        175     N/A     SERVICE_SYSTEM_START    SERVICE_RUNNING SERVICE_FILE_SYSTEM_DRIVER       Msfs    Msfs    \FileSystem\Msfs
0x93dcf0        174     1436    SERVICE_DEMAND_START    SERVICE_RUNNING SERVICE_WIN32_OWN_PROCESSMSDTC   Distributed Transaction Coordinator     C:\Windows\System32\msdtc.exe
0x93d8f0        173     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   msdsm    msdsm   N/A
0x93d800        172     N/A     SERVICE_BOOT_START      SERVICE_RUNNING SERVICE_KERNEL_DRIVER   msahci   msahci  \Driver\msahci
0x93d710        171     N/A     SERVICE_DEMAND_START    SERVICE_RUNNING SERVICE_FILE_SYSTEM_DRIVER       mrxsmb20        SMB 2.0 MiniRedirector  \FileSystem\mrxsmb20
0x93d620        170     N/A     SERVICE_DEMAND_START    SERVICE_RUNNING SERVICE_FILE_SYSTEM_DRIVER       mrxsmb10        SMB 1.x MiniRedirector  \FileSystem\mrxsmb10
0x93d530        169     N/A     SERVICE_DEMAND_START    SERVICE_RUNNING SERVICE_FILE_SYSTEM_DRIVER       mrxsmb  SMB MiniRedirector Wrapper and Engine   \FileSystem\mrxsmb
0x93d440        168     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_FILE_SYSTEM_DRIVER       MRxDAV  WebDav Client Redirector Driver N/A
0x93d350        167     1164    SERVICE_AUTO_START      SERVICE_RUNNING SERVICE_WIN32_SHARE_PROCESS      MpsSvc  Windows Firewall        C:\Windows\system32\svchost.exe -k LocalServiceNoNetwork
0x93d260        166     N/A     SERVICE_DEMAND_START    SERVICE_RUNNING SERVICE_KERNEL_DRIVER   mpsdrv   Windows Firewall Authorization Driver   \Driver\mpsdrv
0x93d170        165     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   mpio     mpio    N/A
0x93d080        164     N/A     SERVICE_BOOT_START      SERVICE_RUNNING SERVICE_KERNEL_DRIVER   mountmgr Mount Point Manager     \Driver\mountmgr
0x93cf90        163     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   mouhid   Mouse HID Driver        N/A
0x93cea0        162     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   mouclass Mouse Class Driver      N/A
0x93cdb0        161     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   monitor  Microsoft Monitor Class Function Driver Service N/A
0x93ccc0        160     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   Modem    Modem   N/A
0x93cbd0        159     868     SERVICE_AUTO_START      SERVICE_RUNNING SERVICE_WIN32_SHARE_PROCESS      MMCSS   Multimedia Class Scheduler      C:\Windows\system32\svchost.exe -k netsvcs
0x93cae0        158     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   MegaSR   MegaSR  N/A
0x93c9f0        157     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   megasas  megasas N/A
0x93c900        156     N/A     SERVICE_DISABLED        SERVICE_STOPPED SERVICE_WIN32_SHARE_PROCESS      Mcx2Svc Media Center Extender Service   N/A
0x93c810        155     N/A     SERVICE_AUTO_START      SERVICE_RUNNING SERVICE_FILE_SYSTEM_DRIVER       luafv   UAC File Virtualization \FileSystem\luafv
0x93c720        154     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   LSI_SCSI LSI_SCSI        N/A
0x93c630        153     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   LSI_SAS2 LSI_SAS2        N/A
0x93c540        152     N/A     SERVICE_BOOT_START      SERVICE_RUNNING SERVICE_KERNEL_DRIVER   LSI_SAS  LSI_SAS \Driver\LSI_SAS
0x93c450        151     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   LSI_FC   LSI_FC  N/A
0x93c360        150     808     SERVICE_AUTO_START      SERVICE_RUNNING SERVICE_WIN32_SHARE_PROCESS      lmhosts TCP/IP NetBIOS Helper   C:\Windows\System32\svchost.exe -k LocalServiceNetworkRestricted
0x93c270        149     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_WIN32_SHARE_PROCESS      lltdsvc Link-Layer Topology Discovery Mapper    N/A
0x93c180        148     N/A     SERVICE_AUTO_START      SERVICE_RUNNING SERVICE_KERNEL_DRIVER   lltdio   Link-Layer Topology Discovery Mapper I/O Driver \Driver\lltdio
0x93c090        147     620     SERVICE_AUTO_START      SERVICE_RUNNING SERVICE_WIN32_SHARE_PROCESS      LanmanWorkstation       Workstation     C:\Windows\system32\svchost.exe -k NetworkService
0x93dbc0        146     868     SERVICE_AUTO_START      SERVICE_RUNNING SERVICE_WIN32_SHARE_PROCESS      LanmanServer    Server  C:\Windows\system32\svchost.exe -k netsvcs
0x93dac0        145     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_WIN32_SHARE_PROCESS      KtmRm   KtmRm for Distributed Transaction Coordinator   N/A
0x93bfa0        144     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   ksthunk  Kernel Streaming Thunks N/A
0x93beb0        143     N/A     SERVICE_BOOT_START      SERVICE_RUNNING SERVICE_KERNEL_DRIVER   KSecPkg  KSecPkg \Driver\KSecPkg
0x93bdc0        142     N/A     SERVICE_BOOT_START      SERVICE_RUNNING SERVICE_KERNEL_DRIVER   KSecDD   KSecDD  \Driver\KSecDD
0x93bcd0        141     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_WIN32_SHARE_PROCESS      KeyIso  CNG Key Isolation       N/A
0x93bbe0        140     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   kbdhid   Keyboard HID Driver     N/A
0x93baf0        139     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   kbdclass Keyboard Class Driver   N/A
0x93b3f0        138     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   iScsiPrt iScsiPort Driver        N/A
0x93b300        137     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   isapnp   isapnp  N/A
0x93b210        136     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   IRENUM   IR Bus Enumerator       N/A
0x93b120        135     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   IPNAT    IP Network Address Translator   N/A
0x93b030        134     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   IPMIDRV  IPMIDRV N/A
0x93af40        133     868     SERVICE_AUTO_START      SERVICE_RUNNING SERVICE_WIN32_SHARE_PROCESS      iphlpsvc        IP Helper       C:\Windows\system32\svchost.exe -k netsvcs
0x93ae50        132     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   IpFilterDriver   IP Traffic Filter Driver        N/A
0x93b9c0        131     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_WIN32_SHARE_PROCESS      IPBusEnum       PnP-X IP Bus Enumerator N/A
0x93ad60        130     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   intelppm Intel Processor Driver  N/A
0x93ac70        129     N/A     SERVICE_BOOT_START      SERVICE_RUNNING SERVICE_KERNEL_DRIVER   intelide intelide        \Driver\intelide
0x93ab80        128     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_WIN32_SHARE_PROCESS      IKEEXT  IKE and AuthIP IPsec Keying Modules     N/A
0x93aa90        127     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   iirsp    iirsp   N/A
0x93a9a0        126     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_WIN32_SHARE_PROCESS      idsvc   Windows CardSpace       N/A
0x93a8b0        125     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   iaStorV  iaStorV N/A
0x93a7c0        124     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   i8042prt i8042 Keyboard and PS/2 Mouse Port Driver       N/A
0x93a6d0        123     N/A     SERVICE_BOOT_START      SERVICE_RUNNING SERVICE_KERNEL_DRIVER   hwpolicy Hardware Policy Driver  \Driver\hwpolicy
0x93a5e0        122     N/A     SERVICE_DEMAND_START    SERVICE_RUNNING SERVICE_KERNEL_DRIVER   HTTP     HTTP    \Driver\HTTP
0x93a4f0        121     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   HpSAMD   HpSAMD  N/A
0x93a400        120     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_WIN32_SHARE_PROCESS      HomeGroupProvider       HomeGroup Provider      N/A
0x93b8c0        119     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_WIN32_SHARE_PROCESS      HomeGroupListener       HomeGroup Listener      N/A
0x93b7c0        118     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_WIN32_SHARE_PROCESS      hkmsvc  Health Key and Certificate Management   N/A
0x93a310        117     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   HidUsb   Microsoft HID Class Driver      N/A
0x93a220        116     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_WIN32_SHARE_PROCESS      hidserv Human Interface Device Access   N/A
0x93a130        115     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   HidIr    Microsoft Infrared HID Driver   N/A
0x93a040        114     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   HidBth   Microsoft Bluetooth HID Miniport        N/A
0x939f50        113     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   HidBatt  HID UPS Battery Driver  N/A
0x939e60        112     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   HDAudBus Microsoft UAA Bus Driver for High Definition Audio      N/A
0x939d70        111     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   HdAudAddService  Microsoft 1.1 UAA Function Driver for High Definition Audio Service     N/A
0x93b6c0        110     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   hcw85cir Hauppauge Consumer Infrared Receiver    N/A
0x939c80        109     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_WIN32_OWN_PROCESSgupdatem        Google Update Service (gupdatem)        N/A
0x939b90        108     N/A     SERVICE_AUTO_START      SERVICE_STOPPED SERVICE_WIN32_OWN_PROCESSgupdate Google Update Service (gupdate) N/A
0x939aa0        107     868     SERVICE_AUTO_START      SERVICE_RUNNING SERVICE_WIN32_SHARE_PROCESS      gpsvc   Group Policy Client     C:\Windows\system32\svchost.exe -k netsvcs
0x9399b0        106     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   gagp30kx Microsoft Generic AGPv3.0 Filter for K8 Processor Platforms     N/A
0x9398c0        105     N/A     SERVICE_BOOT_START      SERVICE_RUNNING SERVICE_KERNEL_DRIVER   fvevol   Bitlocker Drive Encryption Filter Driver        \Driver\fvevol
0x9397d0        104     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_FILE_SYSTEM_DRIVER       FsDepends       File System Dependency Minifilter       N/A
0x9396e0        103     724     SERVICE_DEMAND_START    SERVICE_RUNNING SERVICE_WIN32_OWN_PROCESSFontCache3.0.0.0        Windows Presentation Foundation Font Cache 3.0.0.0      C:\Windows\Microsoft.Net\Framework64\v3.0\WPF\PresentationFontCache.exe
0x93b5c0        102     164     SERVICE_AUTO_START      SERVICE_RUNNING SERVICE_WIN32_SHARE_PROCESS      FontCache       Windows Font Cache Service      C:\Windows\system32\svchost.exe -k LocalServiceAndNoImpersonation
0x9395f0        101     N/A     SERVICE_BOOT_START      SERVICE_RUNNING SERVICE_FILE_SYSTEM_DRIVER       FltMgr  FltMgr  \FileSystem\FltMgr
0x938e90        100     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   flpydisk Floppy Disk Driver      N/A
0x938da0        99      N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_FILE_SYSTEM_DRIVER       Filetrace       Filetrace       N/A
0x938cb0        98      N/A     SERVICE_BOOT_START      SERVICE_RUNNING SERVICE_FILE_SYSTEM_DRIVER       FileInfo        File Information FS MiniFilter  \FileSystem\FileInfo
0x938bc0        97      N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_WIN32_SHARE_PROCESS      FDResPub        Function Discovery Resource Publication N/A
0x938ad0        96      N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_WIN32_SHARE_PROCESS      fdPHost Function Discovery Provider Host        N/A
0x9389e0        95      N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   fdc      Floppy Disk Controller Driver   N/A
0x9394e0        94      N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_WIN32_OWN_PROCESSFax     Fax     N/A
0x939400        93      N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_FILE_SYSTEM_DRIVER       fastfat FAT12/16/32 File System Driver  N/A
0x9388f0        92      N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_FILE_SYSTEM_DRIVER       exfat   exFAT File System Driver        N/A
0x938800        91      1012    SERVICE_AUTO_START      SERVICE_RUNNING SERVICE_WIN32_SHARE_PROCESS      EventSystem     COM+ Event System       C:\Windows\system32\svchost.exe -k LocalService
0x938710        90      808     SERVICE_AUTO_START      SERVICE_RUNNING SERVICE_WIN32_SHARE_PROCESS      eventlog        Windows Event Log       C:\Windows\System32\svchost.exe -k LocalServiceNetworkRestricted
0x938620        89      N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   ErrDev   Microsoft Hardware Error Device Driver  N/A
0x938530        88      N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   elxstor  elxstor N/A
0x938440        87      N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_WIN32_OWN_PROCESSehSched Windows Media Center Scheduler Service  N/A
0x938350        86      N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_WIN32_OWN_PROCESSehRecvr Windows Media Center Receiver Service   N/A
0x938260        85      N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_WIN32_SHARE_PROCESS      EFS     Encrypting File System (EFS)    N/A
0x939320        84      N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   ebdrv    Broadcom NetXtreme II 10 GigE VBD       N/A
0x938170        83      N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_WIN32_SHARE_PROCESS      EapHost Extensible Authentication Protocol      N/A
0x938080        82      N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   E1G60    Intel(R) PRO/1000 NDIS 6 Adapter Driver N/A
0x937f90        81      N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   DXGKrnl  LDDM Graphics Subsystem N/A
0x937ea0        80      N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   drmkaud  Microsoft Trusted Audio Drivers N/A
0x937db0        79      1164    SERVICE_AUTO_START      SERVICE_RUNNING SERVICE_WIN32_SHARE_PROCESS      DPS     Diagnostic Policy Service       C:\Windows\system32\svchost.exe -k LocalServiceNoNetwork
0x939240        78      N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_WIN32_SHARE_PROCESS      dot3svc Wired AutoConfig        N/A
0x937cc0        77      620     SERVICE_AUTO_START      SERVICE_RUNNING SERVICE_WIN32_SHARE_PROCESS      Dnscache        DNS Client      C:\Windows\system32\svchost.exe -k NetworkService
0x937bd0        76      N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   dmvsc    dmvsc   N/A
0x937ae0        75      N/A     SERVICE_BOOT_START      SERVICE_RUNNING SERVICE_KERNEL_DRIVER   Disk     Disk Driver     \Driver\Disk
0x9379f0        74      N/A     SERVICE_SYSTEM_START    SERVICE_RUNNING SERVICE_KERNEL_DRIVER   discache System Attribute Cache  \Driver\discache
0x937900        73      808     SERVICE_AUTO_START      SERVICE_RUNNING SERVICE_WIN32_SHARE_PROCESS      Dhcp    DHCP Client     C:\Windows\System32\svchost.exe -k LocalServiceNetworkRestricted
0x937810        72      N/A     SERVICE_SYSTEM_START    SERVICE_RUNNING SERVICE_FILE_SYSTEM_DRIVER       DfsC    DFS Namespace Client Driver     \FileSystem\DfsC
0x937720        71      N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_WIN32_OWN_PROCESSdefragsvc       Disk Defragmenter       N/A
0x937630        70      604     SERVICE_AUTO_START      SERVICE_RUNNING SERVICE_WIN32_SHARE_PROCESS      DcomLaunch      DCOM Server Process Launcher    C:\Windows\system32\svchost.exe -k DcomLaunch
0x937540        69      844     SERVICE_AUTO_START      SERVICE_RUNNING SERVICE_WIN32_SHARE_PROCESS      CscService      Offline Files   C:\Windows\System32\svchost.exe -k LocalSystemNetworkRestricted
0x937450        68      N/A     SERVICE_SYSTEM_START    SERVICE_RUNNING SERVICE_KERNEL_DRIVER   CSC      Offline Files Driver    \Driver\CSC
0x939160        67      620     SERVICE_AUTO_START      SERVICE_RUNNING SERVICE_WIN32_SHARE_PROCESS      CryptSvc        Cryptographic Services  C:\Windows\system32\svchost.exe -k NetworkService
0x937360        66      N/A     SERVICE_DISABLED        SERVICE_STOPPED SERVICE_KERNEL_DRIVER   crcdisk  Crcdisk Filter Driver   N/A
0x937270        65      1324    SERVICE_DEMAND_START    SERVICE_RUNNING SERVICE_WIN32_OWN_PROCESSCOMSysApp       COM+ System Application C:\Windows\system32\dllhost.exe /Processid:{02D4B3F1-FD88-11D1-960D-00805FC79235}
0x937180        64      N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   CompositeBus     Composite Bus Enumerator Driver N/A
0x939060        63      N/A     SERVICE_BOOT_START      SERVICE_RUNNING SERVICE_KERNEL_DRIVER   Compbatt Microsoft Composite Battery Driver      \Driver\Compbatt
0x937090        62      N/A     SERVICE_BOOT_START      SERVICE_RUNNING SERVICE_KERNEL_DRIVER   CNG      CNG     \Driver\CNG
0x936f80        61      N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   cmdide   cmdide  N/A
0x936160        60      N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   CmBatt   Microsoft AC Adapter Driver     N/A
0x936070        59      3124    SERVICE_AUTO_START      SERVICE_RUNNING SERVICE_WIN32_OWN_PROCESSclr_optimization_v4.0.30319_64  Microsoft .NET Framework NGEN v4.0.30319_X64    C:\Windows\Microsoft.NET\Framework64\v4.0.30319\mscorsvw.exe
0x936e60        58      412     SERVICE_AUTO_START      SERVICE_RUNNING SERVICE_WIN32_OWN_PROCESSclr_optimization_v4.0.30319_32  Microsoft .NET Framework NGEN v4.0.30319_X86    C:\Windows\Microsoft.NET\Framework\v4.0.30319\mscorsvw.exe
0x936d40        57      N/A     SERVICE_DISABLED        SERVICE_STOPPED SERVICE_WIN32_OWN_PROCESSclr_optimization_v2.0.50727_64  Microsoft .NET Framework NGEN v2.0.50727_X64    N/A
0x936c20        56      N/A     SERVICE_DISABLED        SERVICE_STOPPED SERVICE_WIN32_OWN_PROCESSclr_optimization_v2.0.50727_32  Microsoft .NET Framework NGEN v2.0.50727_X86    N/A
0x936b00        55      N/A     SERVICE_BOOT_START      SERVICE_RUNNING SERVICE_KERNEL_DRIVER   CLFS     Common Log (CLFS)       \Driver\CLFS
0x935f80        54      N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   circlass Consumer IR Devices     N/A
0x935e90        53      N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_WIN32_SHARE_PROCESS      CertPropSvc     Certificate Propagation N/A
0x935da0        52      N/A     SERVICE_SYSTEM_START    SERVICE_RUNNING SERVICE_KERNEL_DRIVER   cdrom    CD-ROM Driver   \Driver\cdrom
0x935cb0        51      N/A     SERVICE_DISABLED        SERVICE_STOPPED SERVICE_FILE_SYSTEM_DRIVER       cdfs    CD/DVD File System Reader       N/A
0x935bc0        50      N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   BTHUSB   Bluetooth Radio USB Driver      N/A
0x935ad0        49      1948    SERVICE_DEMAND_START    SERVICE_RUNNING SERVICE_WIN32_SHARE_PROCESS      bthserv Bluetooth Support Service       C:\Windows\system32\svchost.exe -k bthsvcs
0x9359e0        48      N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   BTHPORT  Bluetooth Port Driver   N/A
0x9358f0        47      N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   BthPan   Bluetooth Device (Personal Area Network)        N/A
0x935800        46      N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   BTHMODEM Bluetooth Serial Communications Driver  N/A
0x935710        45      N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   BthEnum  Bluetooth Enumerator Service    N/A
0x935620        44      N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   BrUsbSer Brother MFC USB Serial WDM Driver       N/A
0x935530        43      N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   BrUsbMdm Brother MFC USB Fax Only Modem  N/A
0x935440        42      N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   BrSerWdm Brother WDM Serial driver       N/A
0x935350        41      N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   Brserid  Brother MFC Serial Port Interface Driver (WDM)  N/A
0x935260        40      N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_WIN32_SHARE_PROCESS      Browser Computer Browser        N/A
0x935170        39      N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   BrFiltUp Brother USB Mass-Storage Upper Filter Driver    N/A
0x935080        38      N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   BrFiltLo Brother USB Mass-Storage Lower Filter Driver    N/A
0x934f90        37      N/A     SERVICE_DEMAND_START    SERVICE_RUNNING SERVICE_FILE_SYSTEM_DRIVER       bowser  Browser Support Driver  \FileSystem\bowser
0x934ea0        36      N/A     SERVICE_SYSTEM_START    SERVICE_RUNNING SERVICE_KERNEL_DRIVER   blbdrive blbdrive        \Driver\blbdrive
0x934db0        35      868     SERVICE_AUTO_START      SERVICE_RUNNING SERVICE_WIN32_SHARE_PROCESS      BITS    Background Intelligent Transfer Service C:\Windows\system32\svchost.exe -k netsvcs
0x934cc0        34      1164    SERVICE_AUTO_START      SERVICE_RUNNING SERVICE_WIN32_SHARE_PROCESS      BFE     Base Filtering Engine   C:\Windows\system32\svchost.exe -k LocalServiceNoNetwork
0x936a20        33      N/A     SERVICE_SYSTEM_START    SERVICE_RUNNING SERVICE_KERNEL_DRIVER   Beep     Beep    \Driver\Beep
0x934bd0        32      N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_WIN32_SHARE_PROCESS      BDESVC  BitLocker Drive Encryption Service      N/A
0x934ae0        31      N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   b57nd60a Broadcom NetXtreme Gigabit Ethernet - NDIS 6.0  N/A
0x9349f0        30      N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   b06bdrv  Broadcom NetXtreme II VBD       N/A
0x934900        29      N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_WIN32_SHARE_PROCESS      AxInstSV        ActiveX Installer (AxInstSV)    N/A
0x934810        28      808     SERVICE_AUTO_START      SERVICE_RUNNING SERVICE_WIN32_SHARE_PROCESS      AudioSrv        Windows Audio   C:\Windows\System32\svchost.exe -k LocalServiceNetworkRestricted
0x934720        27      844     SERVICE_AUTO_START      SERVICE_RUNNING SERVICE_WIN32_SHARE_PROCESS      AudioEndpointBuilder    Windows Audio Endpoint Builder  C:\Windows\System32\svchost.exe -k LocalSystemNetworkRestricted
0x936910        26      N/A     SERVICE_BOOT_START      SERVICE_RUNNING SERVICE_KERNEL_DRIVER   atapi    IDE Channel     \Driver\atapi
0x934630        25      N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   AsyncMac RAS Asynchronous Media Driver   N/A
0x934540        24      N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_WIN32_OWN_PROCESSaspnet_state    ASP.NET State Service   N/A
0x936810        23      N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   arcsas   arcsas  N/A
0x934450        22      N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   arc      arc     N/A
0x936730        21      868     SERVICE_DEMAND_START    SERVICE_RUNNING SERVICE_WIN32_SHARE_PROCESS      AppMgmt Application Management  C:\Windows\system32\svchost.exe -k netsvcs
0x934360        20      868     SERVICE_DEMAND_START    SERVICE_RUNNING SERVICE_WIN32_SHARE_PROCESS      Appinfo Application Information C:\Windows\system32\svchost.exe -k netsvcs
0x934240        19      N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_WIN32_SHARE_PROCESS      AppIDSvc        Application Identity    N/A
0x9123b0        18      N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   AppID    AppID Driver    N/A
0x9122c0        17      N/A     SERVICE_BOOT_START      SERVICE_RUNNING SERVICE_KERNEL_DRIVER   amdxata  amdxata \Driver\amdxata
0x9121d0        16      N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   amdsbs   amdsbs  N/A
0x9120e0        15      N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   amdsata  amdsata N/A
0x911ff0        14      N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   AmdPPM   AMD Processor Driver    N/A
0x911f00        13      N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   AmdK8    AMD K8 Processor Driver N/A
0x911e10        12      N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   amdide   amdide  N/A
0x911d20        11      N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   aliide   aliide  N/A
0x911c30        10      N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_WIN32_OWN_PROCESSALG     Application Layer Gateway Service       N/A
0x911b50        9       N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   agp440   Intel AGP Bus Filter    N/A
0x911a60        8       N/A     SERVICE_SYSTEM_START    SERVICE_RUNNING SERVICE_KERNEL_DRIVER   AFD      Ancillary Function Driver for Winsock   \Driver\AFD
0x911980        7       868     SERVICE_DEMAND_START    SERVICE_RUNNING SERVICE_WIN32_SHARE_PROCESS      AeLookupSvc     Application Experience  C:\Windows\system32\svchost.exe -k netsvcs
0x911890        6       N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   adpu320  adpu320 N/A
0x9117a0        5       N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   adpahci  adpahci N/A
0x9116b0        4       N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   adp94xx  adp94xx N/A
0x9115c0        3       N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   AcpiPmi  ACPI Power Meter Driver N/A
0x9114d0        2       N/A     SERVICE_BOOT_START      SERVICE_RUNNING SERVICE_KERNEL_DRIVER   ACPI     Microsoft ACPI Driver   \Driver\ACPI
0x9113e0        1       N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   1394ohci 1394 OHCI Compliant Host Controller     N/A
0x934720        28      808     SERVICE_AUTO_START      SERVICE_RUNNING SERVICE_WIN32_SHARE_PROCESS      AudioSrv        Windows Audio   C:\Windows\System32\svchost.exe -k LocalServiceNetworkRestricted
0x93e830        188     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_WIN32_SHARE_PROCESS      napagent        Network Access Protection Agent N/A
0x941de0        248     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_WIN32_SHARE_PROCESS      RasMan  Remote Access Connection Manager        N/A
0x941de0        247     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   Rasl2tp  WAN Miniport (L2TP)     N/A
0x941cf0        246     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_WIN32_SHARE_PROCESS      RasAuto Remote Access Auto Connection Manager   N/A
0x941c00        245     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   RasAgileVpn      WAN Miniport (IKEv2)    N/A
0x941b10        244     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   RasAcd   Remote Access Auto Connection Driver    N/A
0x941a20        243     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   QWAVEdrv QWAVE driver    N/A
0x941930        242     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_WIN32_SHARE_PROCESS      QWAVE   Quality Windows Audio Video Experience  N/A
0x941840        241     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   ql40xx   ql40xx  N/A
0x941750        240     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   ql2300   ql2300  N/A
0x941660        239     N/A     SERVICE_SYSTEM_START    SERVICE_RUNNING SERVICE_KERNEL_DRIVER   Psched   QoS Packet Scheduler    \Driver\Psched
0x941570        238     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_WIN32_SHARE_PROCESS      ProtectedStorage        Protected Storage       N/A
0x942620        237     868     SERVICE_AUTO_START      SERVICE_RUNNING SERVICE_WIN32_SHARE_PROCESS      ProfSvc User Profile Service    C:\Windows\system32\svchost.exe -k netsvcs
0x941480        236     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   Processor        Processor Driver        N/A
0x941390        235     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   PptpMiniport     WAN Miniport (PPTP)     N/A
0x942520        234     604     SERVICE_AUTO_START      SERVICE_RUNNING SERVICE_WIN32_SHARE_PROCESS      Power   Power   C:\Windows\system32\svchost.exe -k DcomLaunch
0x9412a0        233     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_WIN32_SHARE_PROCESS      PolicyAgent     IPsec Policy Agent      N/A
0x9411b0        232     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_WIN32_SHARE_PROCESS      PNRPsvc Peer Name Resolution Protocol   N/A
0x9410c0        231     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_WIN32_SHARE_PROCESS      PNRPAutoReg     PNRP Machine Name Publication Service   N/A
0x940fd0        230     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   PNPMEM   Microsoft Memory Module Driver  N/A
0x940ee0        229     604     SERVICE_AUTO_START      SERVICE_RUNNING SERVICE_WIN32_SHARE_PROCESS      PlugPlay        Plug and Play   C:\Windows\system32\svchost.exe -k DcomLaunch
0x940df0        228     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_WIN32_SHARE_PROCESS      pla     Performance Logs & Alerts       N/A
0x942440        227     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_WIN32_OWN_PROCESSPerfHost        Performance Counter DLL Host    N/A
0x940d00        226     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_WIN32_SHARE_PROCESS      PeerDistSvc     BranchCache     N/A
0x940c10        225     N/A     SERVICE_AUTO_START      SERVICE_RUNNING SERVICE_KERNEL_DRIVER   PEAUTH   PEAUTH  \Driver\PEAUTH
0x940b20        224     N/A     SERVICE_BOOT_START      SERVICE_RUNNING SERVICE_KERNEL_DRIVER   pcw      Performance Counters for Windows Driver \Driver\pcw
0x942360        223     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   pcmcia   pcmcia  N/A
0x940a30        222     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   pciide   pciide  N/A
0x940940        221     N/A     SERVICE_BOOT_START      SERVICE_RUNNING SERVICE_KERNEL_DRIVER   pci      PCI Bus Driver  \Driver\pci
0x942280        220     844     SERVICE_AUTO_START      SERVICE_RUNNING SERVICE_WIN32_SHARE_PROCESS      PcaSvc  Program Compatibility Assistant Service C:\Windows\System32\svchost.exe -k LocalSystemNetworkRestricted
0x940850        219     N/A     SERVICE_BOOT_START      SERVICE_RUNNING SERVICE_KERNEL_DRIVER   partmgr  Partition Manager       \Driver\partmgr
0x940760        218     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   Parport  Parallel port driver    N/A
0x940670        217     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_WIN32_SHARE_PROCESS      p2psvc  Peer Networking Grouping        N/A
0x940580        216     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_WIN32_SHARE_PROCESS      p2pimsvc        Peer Networking Identity Manager        N/A
0x940490        215     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   ohci1394 1394 OHCI Compliant Host Controller (Legacy)    N/A
0x9403a0        214     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   nv_agp   NVIDIA nForce AGP Bus Filter    N/A
0x9402b0        213     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   nvstor   nvstor  N/A
0x93faf0        212     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   nvraid   nvraid  N/A
0x93fa00        211     N/A     SERVICE_SYSTEM_START    SERVICE_RUNNING SERVICE_KERNEL_DRIVER   Null     Null    \Driver\Null
0x93f910        210     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_FILE_SYSTEM_DRIVER       Ntfs    Ntfs    N/A
0x93f820        209     N/A     SERVICE_SYSTEM_START    SERVICE_RUNNING SERVICE_KERNEL_DRIVER   nsiproxy NSI proxy service driver.       \Driver\nsiproxy
0x93f730        208     1012    SERVICE_AUTO_START      SERVICE_RUNNING SERVICE_WIN32_SHARE_PROCESS      nsi     Network Store Interface Service C:\Windows\system32\svchost.exe -k LocalService
0x9401a0        207     N/A     SERVICE_SYSTEM_START    SERVICE_RUNNING SERVICE_FILE_SYSTEM_DRIVER       Npfs    Npfs    \FileSystem\Npfs
0x93f640        206     620     SERVICE_AUTO_START      SERVICE_RUNNING SERVICE_WIN32_SHARE_PROCESS      NlaSvc  Network Location Awareness      C:\Windows\system32\svchost.exe -k NetworkService
0x93f550        205     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   nfrd960  nfrd960 N/A
0x93f460        204     N/A     SERVICE_DISABLED        SERVICE_STOPPED SERVICE_WIN32_SHARE_PROCESS      NetTcpPortSharing       Net.Tcp Port Sharing Service    N/A
0x9400a0        203     N/A     SERVICE_DISABLED        SERVICE_STOPPED SERVICE_WIN32_SHARE_PROCESS      NetTcpActivator Net.Tcp Listener Adapter        N/A
0x93ffa0        202     1012    SERVICE_DEMAND_START    SERVICE_RUNNING SERVICE_WIN32_SHARE_PROCESS      netprofm        Network List Service    C:\Windows\system32\svchost.exe -k LocalService
0x945250        415     3496    SERVICE_AUTO_START      SERVICE_RUNNING SERVICE_WIN32_OWN_PROCESSWCAssistantService      WC Assistant    C:\Program Files (x86)\Lavasoft\Web Companion\Application\Lavasoft.WCAssistant.WinService.exe
0x945250        413     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_WIN32_SHARE_PROCESS      WwanSvc WWAN AutoConfig N/A
0x7923b0        412     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_WIN32_SHARE_PROCESS      wudfsvc Windows Driver Foundation - User-mode Driver Framework  N/A
0x7922c0        411     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   WudfPf   User Mode Driver Frameworks Platform Driver     N/A
0x7921d0        410     868     SERVICE_AUTO_START      SERVICE_RUNNING SERVICE_WIN32_SHARE_PROCESS      wuauserv        Windows Update  C:\Windows\system32\svchost.exe -k netsvcs
0x791eb0        409     3064    SERVICE_AUTO_START      SERVICE_RUNNING SERVICE_WIN32_OWN_PROCESSWSearch Windows Search  C:\Windows\system32\SearchIndexer.exe /Embedding
0x791dc0        408     808     SERVICE_AUTO_START      SERVICE_RUNNING SERVICE_WIN32_SHARE_PROCESS      wscsvc  Security Center C:\Windows\System32\svchost.exe -k LocalServiceNetworkRestricted
0x791cd0        407     N/A     SERVICE_SYSTEM_START    SERVICE_RUNNING SERVICE_KERNEL_DRIVER   ws2ifsl  Windows Socket 2.0 Non-IFS Service Provider Support Environment \Driver\ws2ifsl
0x791be0        406     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_WIN32_SHARE_PROCESS      WPDBusEnum      Portable Device Enumerator Service      N/A
0x791af0        405     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_WIN32_SHARE_PROCESS      WPCSvc  Parental Controls       N/A
0x791a00        404     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_WIN32_OWN_PROCESSWMPNetworkSvc   Windows Media Player Network Sharing Service    N/A
0x945850        403     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_WIN32_OWN_PROCESSwmiApSrv        WMI Performance Adapter N/A
0x791910        402     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   WmiAcpi  Microsoft Windows Management Interface for ACPI N/A
0x791820        401     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_WIN32_SHARE_PROCESS      Wlansvc WLAN AutoConfig N/A
0x791730        400     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_WIN32_SHARE_PROCESS      WinRM   Windows Remote Management (WS-Management)       N/A
0x791640        399     868     SERVICE_AUTO_START      SERVICE_RUNNING SERVICE_WIN32_SHARE_PROCESS      Winmgmt Windows Management Instrumentation      C:\Windows\system32\svchost.exe -k netsvcs
0x791550        398     1012    SERVICE_DEMAND_START    SERVICE_RUNNING SERVICE_WIN32_SHARE_PROCESS      WinHttpAutoProxySvc     WinHTTP Web Proxy Auto-Discovery Service        C:\Windows\system32\svchost.exe -k LocalService
0x945750        397     3196    SERVICE_AUTO_START      SERVICE_RUNNING SERVICE_WIN32_SHARE_PROCESS      WinDefend       Windows Defender        C:\Windows\System32\svchost.exe -k secsvcs
0x791460        396     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_FILE_SYSTEM_DRIVER       WIMMount        WIMMount        N/A
0x791370        395     N/A     SERVICE_SYSTEM_START    SERVICE_RUNNING SERVICE_KERNEL_DRIVER   WfpLwf   WFP Lightweight Filter  \Driver\WfpLwf
0x791280        394     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_WIN32_SHARE_PROCESS      WerSvc  Windows Error Reporting Service N/A
0x791190        393     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_WIN32_SHARE_PROCESS      wercplsupport   Problem Reports and Solutions Control Panel Support     N/A
0x945650        392     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_WIN32_SHARE_PROCESS      Wecsvc  Windows Event Collector N/A
0x7910a0        391     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_WIN32_SHARE_PROCESS      WebClient       WebClient       N/A
0x790fb0        390     844     SERVICE_DEMAND_START    SERVICE_RUNNING SERVICE_WIN32_SHARE_PROCESS      WdiSystemHost   Diagnostic System Host  C:\Windows\System32\svchost.exe -k LocalSystemNetworkRestricted
0x945550        389     1012    SERVICE_DEMAND_START    SERVICE_RUNNING SERVICE_WIN32_SHARE_PROCESS      WdiServiceHost  Diagnostic Service Host C:\Windows\system32\svchost.exe -k LocalService
0x945450        388     N/A     SERVICE_BOOT_START      SERVICE_RUNNING SERVICE_KERNEL_DRIVER   Wdf01000 Kernel Mode Driver Frameworks service   \Driver\Wdf01000
0x790ec0        387     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   Wd       Wd      N/A
0x94af70        386     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_WIN32_SHARE_PROCESS      WcsPlugInService        Windows Color System    N/A
0x945350        385     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_WIN32_SHARE_PROCESS      wcncsvc Windows Connect Now - Config Registrar  N/A
0x790dd0        383     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_WIN32_SHARE_PROCESS      WbioSrvc        Windows Biometric Service       N/A
0x790ce0        382     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_WIN32_OWN_PROCESSwbengine        Block Level Backup Engine Service       N/A
0x790bf0        381     N/A     SERVICE_SYSTEM_START    SERVICE_RUNNING SERVICE_KERNEL_DRIVER   Wanarpv6 Remote Access IPv6 ARP Driver   \Driver\Wanarpv6
0x790b00        380     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   WANARP   Remote Access IP ARP Driver     N/A
0x790a10        379     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   WacomPen Wacom Serial Pen HID Driver     N/A
0x790920        378     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_WIN32_SHARE_PROCESS      W32Time Windows Time    N/A
0x790830        377     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   vwifibus Virtual WiFi Bus Driver N/A
0x790740        376     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_WIN32_OWN_PROCESSVSS     Volume Shadow Copy      N/A
0x94ae90        375     N/A     SERVICE_BOOT_START      SERVICE_RUNNING SERVICE_KERNEL_DRIVER   vsock    vSockets Driver \Driver\vsock
0x790650        374     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   vsmraid  vsmraid N/A
0x790560        373     N/A     SERVICE_BOOT_START      SERVICE_RUNNING SERVICE_KERNEL_DRIVER   volsnap  Storage volumes \Driver\volsnap
0x790470        372     N/A     SERVICE_BOOT_START      SERVICE_RUNNING SERVICE_KERNEL_DRIVER   volmgrx  Dynamic Volume Manager  \Driver\volmgrx
0x790380        371     N/A     SERVICE_BOOT_START      SERVICE_RUNNING SERVICE_KERNEL_DRIVER   volmgr   Volume Manager Driver   \Driver\volmgr
0x790290        370     668     SERVICE_AUTO_START      SERVICE_RUNNING SERVICE_WIN32_OWN_PROCESSVMware Physical Disk Helper Service     VMware Physical Disk Helper Service     "C:\Program Files\VMware\VMware Tools\vmacthlp.exe"
0x792080        369     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_WIN32_OWN_PROCESSvmvss   VMware Snapshot Provider        N/A
0x7901a0        368     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   vmusbmouse       VMware USB Pointing Device      N/A
0x7900b0        367     1428    SERVICE_AUTO_START      SERVICE_RUNNING SERVICE_WIN32_OWN_PROCESSVMTools VMware Tools    "C:\Program Files\VMware\VMware Tools\vmtoolsd.exe"
0x94e910        366     N/A     SERVICE_SYSTEM_START    SERVICE_RUNNING SERVICE_KERNEL_DRIVER   vmrawdsk VMware Vista Physical Disk Helper       \Driver\vmrawdsk
0x94e820        365     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   vmmouse  VMware Pointing Device  N/A
0x94e730        364     N/A     SERVICE_AUTO_START      SERVICE_RUNNING SERVICE_KERNEL_DRIVER   VMMEMCTL Memory Control Driver   \Driver\VMMEMCTL
0x94e640        363     N/A     SERVICE_SYSTEM_START    SERVICE_RUNNING SERVICE_FILE_SYSTEM_DRIVER       vmhgfs  VMware Host Guest Client Redirector     \FileSystem\vmhgfs
0x94e550        362     N/A     SERVICE_BOOT_START      SERVICE_RUNNING SERVICE_KERNEL_DRIVER   vmci     VMware VMCI Bus Driver  \Driver\vmci
0x94e460        361     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   VMBusHID VMBusHID        N/A
0x94e370        360     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   vmbus    vmbus   N/A
0x94e280        359     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   vm3dmp   vm3dmp  N/A
0x94e190        358     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   viaide   viaide  N/A
0x94e0a0        357     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   vhdmp    vhdmp   N/A
0x94dfb0        356     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   VGPU     VGPU    N/A
0x94dec0        355     1356    SERVICE_AUTO_START      SERVICE_RUNNING SERVICE_WIN32_OWN_PROCESSVGAuthService   VMware Alias Manager and Ticket Service "C:\Program Files\VMware\VMware Tools\VMware VGAuth\VGAuthService.exe"
0x945150        354     N/A     SERVICE_SYSTEM_START    SERVICE_RUNNING SERVICE_KERNEL_DRIVER   VgaSave  VgaSave \Driver\VgaSave
0x94ddd0        353     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   vga      vga     N/A
0x94adb0        352     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_WIN32_OWN_PROCESSvds     Virtual Disk    N/A
0x94acd0        351     N/A     SERVICE_BOOT_START      SERVICE_RUNNING SERVICE_KERNEL_DRIVER   vdrvroot Microsoft Virtual Drive Enumerator Driver       \Driver\vdrvroot
0x94dce0        350     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_WIN32_SHARE_PROCESS      VaultSvc        Credential Manager      N/A
0x94dbf0        349     844     SERVICE_AUTO_START      SERVICE_RUNNING SERVICE_WIN32_SHARE_PROCESS      UxSms   Desktop Window Manager Session Manager  C:\Windows\System32\svchost.exe -k LocalSystemNetworkRestricted
0x94db00        348     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   usbuhci  Microsoft USB Universal Host Controller Miniport Driver N/A
0x94da10        347     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   USBSTOR  USB Mass Storage Driver N/A
0x94d920        346     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   usbprint Microsoft USB PRINTER Class     N/A
0x94d830        345     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   usbohci  Microsoft USB Open Host Controller Miniport Driver      N/A
0x94d740        344     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   usbhub   Microsoft USB Standard Hub Driver       N/A
0x94d650        343     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   usbehci  Microsoft USB 2.0 Enhanced Host Controller Miniport Driver      N/A
0x94d560        342     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   usbcir   eHome Infrared Receiver (USBCIR)        N/A
0x94d470        341     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   usbccgp  Microsoft USB Generic Parent Driver     N/A
0x94d380        340     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_WIN32_SHARE_PROCESS      upnphost        UPnP Device Host        N/A
0x94d290        339     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_WIN32_SHARE_PROCESS      UmRdpService    Remote Desktop Services UserMode Port Redirector        N/A
0x945050        338     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   UmPass   Microsoft UMPass Driver N/A
0x94d1a0        337     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   umbus    UMBus Enumerator Driver N/A
0x94d0b0        336     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   uliagpkx Uli AGP Bus Filter      N/A
0x94cfc0        335     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_WIN32_OWN_PROCESS|SERVICE_INTERACTIVE_PROCESS    UI0Detect       Interactive Services Detection  N/A
0x94ced0        334     N/A     SERVICE_DISABLED        SERVICE_STOPPED SERVICE_FILE_SYSTEM_DRIVER       udfs    udfs    N/A
0x94cde0        333     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   uagp35   Microsoft AGPv3.5 Filter        N/A
0x94ccf0        332     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   tunnel   Microsoft Tunnel Miniport Adapter Driver        N/A
0x94cc00        331     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   tsusbhub tsusbhub        N/A
0x94cb10        330     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   TsUsbGD  Remote Desktop Generic USB Device       N/A
0x94a830        329     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   TsUsbFlt TsUsbFlt        N/A
0x94a740        328     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   tssecsrv Remote Desktop Services Security Filter Driver  N/A
0x94a650        327     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_WIN32_OWN_PROCESSTrustedInstaller        Windows Modules Installer       N/A
0x944f50        326     844     SERVICE_AUTO_START      SERVICE_RUNNING SERVICE_WIN32_SHARE_PROCESS      TrkWks  Distributed Link Tracking Client        C:\Windows\System32\svchost.exe -k LocalSystemNetworkRestricted
0x94a560        325     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_WIN32_OWN_PROCESSTPVCGateway     TP VC Gateway Service   N/A
0x94a470        324     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_WIN32_OWN_PROCESSTPAutoConnSvc   TP AutoConnect Service  N/A
0x944e50        323     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_WIN32_SHARE_PROCESS      THREADORDER     Thread Ordering Server  N/A
0x94a380        322     868     SERVICE_AUTO_START      SERVICE_RUNNING SERVICE_WIN32_SHARE_PROCESS      Themes  Themes  C:\Windows\system32\svchost.exe -k netsvcs
0x94a290        321     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_WIN32_SHARE_PROCESS      TermService     Remote Desktop Services N/A
0x94a1a0        320     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   terminpt Microsoft Remote Desktop Input Driver   N/A
0x94a0b0        319     N/A     SERVICE_SYSTEM_START    SERVICE_RUNNING SERVICE_KERNEL_DRIVER   TermDD   Terminal Device Driver  \Driver\TermDD
0x949fc0        318     N/A     SERVICE_SYSTEM_START    SERVICE_RUNNING SERVICE_KERNEL_DRIVER   tdx      NetIO Legacy TDI Support Driver \Driver\tdx
0x94abf0        317     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   TDTCP    TDTCP   N/A
0x949ed0        316     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   TDPIPE   TDPIPE  N/A
0x949de0        315     N/A     SERVICE_AUTO_START      SERVICE_RUNNING SERVICE_KERNEL_DRIVER   tcpipreg TCP/IP Registry Compatibility   \Driver\tcpipreg
0x949cf0        314     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   TCPIP6   Microsoft IPv6 Protocol Driver  N/A
0x949c00        313     N/A     SERVICE_BOOT_START      SERVICE_RUNNING SERVICE_KERNEL_DRIVER   Tcpip    TCP/IP Protocol Driver  \Driver\Tcpip
0x949b10        312     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_WIN32_SHARE_PROCESS      TBS     TPM Base Services       N/A
0x94ab10        311     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_WIN32_SHARE_PROCESS      TapiSrv Telephony       N/A
0x949a20        310     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_WIN32_SHARE_PROCESS      TabletInputService      Tablet PC Input Service N/A
0x944d50        309     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_WIN32_SHARE_PROCESS      SysMain Superfetch      N/A
0x949930        308     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   Synth3dVsc       Synth3dVsc      N/A
0x949840        307     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_WIN32_OWN_PROCESSswprv   Microsoft Software Shadow Copy Provider N/A
0x949750        306     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   swenum   Software Bus Driver     N/A
0x949660        305     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   storvsc  storvsc N/A
0x949570        304     N/A     SERVICE_BOOT_START      SERVICE_RUNNING SERVICE_KERNEL_DRIVER   storflt  Disk Virtual Machine Bus Acceleration Filter Driver     \Driver\storflt
0x949480        303     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_WIN32_OWN_PROCESSstisvc  Windows Image Acquisition (WIA) N/A
0x949390        302     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   stexstor stexstor        N/A
0x9492a0        301     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_WIN32_SHARE_PROCESS      SstpSvc Secure Socket Tunneling Protocol Service        N/A
0x9491b0        300     164     SERVICE_DEMAND_START    SERVICE_RUNNING SERVICE_WIN32_SHARE_PROCESS      SSDPSRV SSDP Discovery  C:\Windows\system32\svchost.exe -k LocalServiceAndNoImpersonation
0x9490c0        299     N/A     SERVICE_DEMAND_START    SERVICE_RUNNING SERVICE_FILE_SYSTEM_DRIVER       srvnet  srvnet  \FileSystem\srvnet
0x948fd0        298     N/A     SERVICE_DEMAND_START    SERVICE_RUNNING SERVICE_FILE_SYSTEM_DRIVER       srv2    Server SMB 2.xxx Driver \FileSystem\srv2
0x948ee0        297     N/A     SERVICE_DEMAND_START    SERVICE_RUNNING SERVICE_FILE_SYSTEM_DRIVER       srv     Server SMB 1.xxx Driver \FileSystem\srv
0x94aa00        296     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_WIN32_SHARE_PROCESS      sppuinotify     SPP Notification Service        N/A
0x948df0        295     2500    SERVICE_AUTO_START      SERVICE_RUNNING SERVICE_WIN32_OWN_PROCESSsppsvc  Software Protection     C:\Windows\system32\sppsvc.exe
0x948d00        294     1120    SERVICE_AUTO_START      SERVICE_RUNNING SERVICE_WIN32_OWN_PROCESS|SERVICE_INTERACTIVE_PROCESS    Spooler Print Spooler   C:\Windows\System32\spoolsv.exe
0x948c10        293     N/A     SERVICE_BOOT_START      SERVICE_RUNNING SERVICE_KERNEL_DRIVER   spldr    Security Processor Loader Driver        \Driver\spldr
0x948b20        292     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_WIN32_OWN_PROCESSSNMPTRAP        SNMP Trap       N/A
0x948a30        291     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   Smb      Message-oriented TCP/IP and TCP/IPv6 Protocol (SMB session)     N/A
0x948920        290     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   SiSRaid4 SiSRaid4        N/A
0x944550        289     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   SiSRaid2 SiSRaid2        N/A
0x944460        288     868     SERVICE_AUTO_START      SERVICE_RUNNING SERVICE_WIN32_SHARE_PROCESS      ShellHWDetection        Shell Hardware Detection        C:\Windows\system32\svchost.exe -k netsvcs
0x944c50        287     N/A     SERVICE_DISABLED        SERVICE_STOPPED SERVICE_WIN32_SHARE_PROCESS      SharedAccess    Internet Connection Sharing (ICS)       N/A
0x944b50        286     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   sfloppy  High-Capacity Floppy Disk Drive N/A
0x944370        285     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   sffp_sd  SFF Storage Protocol Driver for SDBus   N/A
0x944280        284     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   sffp_mmc SFF Storage Protocol Driver for MMC     N/A
0x944190        283     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   sffdisk  SFF Storage Class Driver        N/A
0x9440a0        282     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_WIN32_SHARE_PROCESS      SessionEnv      Remote Desktop Configuration    N/A
0x943fb0        281     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   sermouse Serial Mouse Driver     N/A
0x943ec0        280     N/A     SERVICE_SYSTEM_START    SERVICE_RUNNING SERVICE_KERNEL_DRIVER   Serial   Serial port driver      \Driver\Serial
0x943dd0        279     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   Serenum  Serenum Filter Driver   N/A
0x943ce0        278     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_WIN32_SHARE_PROCESS      SensrSvc        Adaptive Brightness     N/A
0x943bf0        277     868     SERVICE_AUTO_START      SERVICE_RUNNING SERVICE_WIN32_SHARE_PROCESS      SENS    System Event Notification Service       C:\Windows\system32\svchost.exe -k netsvcs
0x943b00        276     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_WIN32_SHARE_PROCESS      seclogon        Secondary Logon N/A
0x943a10        275     N/A     SERVICE_AUTO_START      SERVICE_RUNNING SERVICE_KERNEL_DRIVER   secdrv   Security Driver \Driver\secdrv
0x943920        274     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_WIN32_OWN_PROCESSSDRSVC  Windows Backup  N/A
0x943830        273     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_WIN32_SHARE_PROCESS      SCPolicySvc     Smart Card Removal Policy       N/A
0x943740        272     868     SERVICE_AUTO_START      SERVICE_RUNNING SERVICE_WIN32_SHARE_PROCESS      Schedule        Task Scheduler  C:\Windows\system32\svchost.exe -k netsvcs
0x943650        271     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   scfilter Smart card PnP Class Filter Driver      N/A
0x943560        270     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_WIN32_SHARE_PROCESS      SCardSvr        Smart Card      N/A
0x943470        269     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   sbp2port sbp2port        N/A
0x943380        268     500     SERVICE_AUTO_START      SERVICE_RUNNING SERVICE_WIN32_SHARE_PROCESS      SamSs   Security Accounts Manager       C:\Windows\system32\lsass.exe
0x943290        267     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   s3cap    s3cap   N/A
0x9431a0        266     N/A     SERVICE_AUTO_START      SERVICE_RUNNING SERVICE_KERNEL_DRIVER   rspndr   Link-Layer Topology Discovery Responder \Driver\rspndr
0x9430b0        265     712     SERVICE_AUTO_START      SERVICE_RUNNING SERVICE_WIN32_SHARE_PROCESS      RpcSs   Remote Procedure Call (RPC)     C:\Windows\system32\svchost.exe -k RPCSS
0x942fc0        264     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_WIN32_OWN_PROCESSRpcLocator      Remote Procedure Call (RPC) Locator     N/A
0x942ed0        263     712     SERVICE_AUTO_START      SERVICE_RUNNING SERVICE_WIN32_SHARE_PROCESS      RpcEptMapper    RPC Endpoint Mapper     C:\Windows\system32\svchost.exe -k RPCSS
0x944a50        262     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   RFCOMM   Bluetooth Device (RFCOMM Protocol TDI)  N/A
0x942de0        261     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_WIN32_SHARE_PROCESS      RemoteRegistry  Remote Registry N/A
0x944950        260     N/A     SERVICE_DISABLED        SERVICE_STOPPED SERVICE_WIN32_SHARE_PROCESS      RemoteAccess    Routing and Remote Access       N/A
0x944820        259     N/A     SERVICE_BOOT_START      SERVICE_RUNNING SERVICE_KERNEL_DRIVER   rdyboost ReadyBoost      \Driver\rdyboost
0x942cf0        258     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   RDPWD    RDP Winstation Driver   N/A
0x942c00        257     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   RdpVideoMiniport Remote Desktop Video Miniport Driver    N/A
0x944720        256     N/A     SERVICE_SYSTEM_START    SERVICE_RUNNING SERVICE_KERNEL_DRIVER   RDPREFMP Reflector Display Driver used to gain access to graphics data   \Driver\RDPREFMP
0x942b10        255     N/A     SERVICE_SYSTEM_START    SERVICE_RUNNING SERVICE_KERNEL_DRIVER   RDPENCDD RDP Encoder Mirror Driver       \Driver\RDPENCDD
0x942a20        254     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   RDPDR    Terminal Server Device Redirector Driver        N/A
0x942930        253     N/A     SERVICE_SYSTEM_START    SERVICE_RUNNING SERVICE_KERNEL_DRIVER   RDPCDD   RDPCDD  \Driver\RDPCDD
0x942840        252     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   rdpbus   Remote Desktop Device Redirector Bus Driver     N/A
0x942750        251     N/A     SERVICE_SYSTEM_START    SERVICE_RUNNING SERVICE_FILE_SYSTEM_DRIVER       rdbss   Redirected Buffering Sub Sysytem        \FileSystem\rdbss
0x9420b0        250     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   RasSstp  WAN Miniport (SSTP)     N/A
0x941fc0        249     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_KERNEL_DRIVER   RasPppoe Remote Access PPPOE Driver      N/A
0x941ed0        248     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_WIN32_SHARE_PROCESS      RasMan  Remote Access Connection Manager        N/A
0x94a1a0        321     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_WIN32_SHARE_PROCESS      TermService     Remote Desktop Services N/A
0x943650        272     868     SERVICE_AUTO_START      SERVICE_RUNNING SERVICE_WIN32_SHARE_PROCESS      Schedule        Task Scheduler  C:\Windows\system32\svchost.exe -k netsvcs
0x9412a0        234     604     SERVICE_AUTO_START      SERVICE_RUNNING SERVICE_WIN32_SHARE_PROCESS      Power   Power   C:\Windows\system32\svchost.exe -k DcomLaunch
0x940df0        229     604     SERVICE_AUTO_START      SERVICE_RUNNING SERVICE_WIN32_SHARE_PROCESS      PlugPlay        Plug and Play   C:\Windows\system32\svchost.exe -k DcomLaunch
0x93ae50        133     868     SERVICE_AUTO_START      SERVICE_RUNNING SERVICE_WIN32_SHARE_PROCESS      iphlpsvc        IP Helper       C:\Windows\system32\svchost.exe -k netsvcs
0x934360        21      868     SERVICE_DEMAND_START    SERVICE_RUNNING SERVICE_WIN32_SHARE_PROCESS      AppMgmt Application Management  C:\Windows\system32\svchost.exe -k netsvcs
0x941de0        248     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_WIN32_SHARE_PROCESS      RasMan  Remote Access Connection Manager        N/A
0x911890        7       868     SERVICE_DEMAND_START    SERVICE_RUNNING SERVICE_WIN32_SHARE_PROCESS      AeLookupSvc     Application Experience  C:\Windows\system32\svchost.exe -k netsvcs
0x941de0        248     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_WIN32_SHARE_PROCESS      RasMan  Remote Access Connection Manager        N/A
0x936e60        59      3124    SERVICE_AUTO_START      SERVICE_RUNNING SERVICE_WIN32_OWN_PROCESSclr_optimization_v4.0.30319_64  Microsoft .NET Framework NGEN v4.0.30319_X64    C:\Windows\Microsoft.NET\Framework64\v4.0.30319\mscorsvw.exe
0x934720        28      808     SERVICE_AUTO_START      SERVICE_RUNNING SERVICE_WIN32_SHARE_PROCESS      AudioSrv        Windows Audio   C:\Windows\System32\svchost.exe -k LocalServiceNetworkRestricted
0x791eb0        410     868     SERVICE_AUTO_START      SERVICE_RUNNING SERVICE_WIN32_SHARE_PROCESS      wuauserv        Windows Update  C:\Windows\system32\svchost.exe -k netsvcs
0x791460        397     3196    SERVICE_AUTO_START      SERVICE_RUNNING SERVICE_WIN32_SHARE_PROCESS      WinDefend       Windows Defender        C:\Windows\System32\svchost.exe -k secsvcs
0x791cd0        408     808     SERVICE_AUTO_START      SERVICE_RUNNING SERVICE_WIN32_SHARE_PROCESS      wscsvc  Security Center C:\Windows\System32\svchost.exe -k LocalServiceNetworkRestricted
0x941de0        248     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_WIN32_SHARE_PROCESS      RasMan  Remote Access Connection Manager        N/A
0x934720        28      808     SERVICE_AUTO_START      SERVICE_RUNNING SERVICE_WIN32_SHARE_PROCESS      AudioSrv        Windows Audio   C:\Windows\System32\svchost.exe -k LocalServiceNetworkRestricted
0x792080        370     668     SERVICE_AUTO_START      SERVICE_RUNNING SERVICE_WIN32_OWN_PROCESSVMware Physical Disk Helper Service     VMware Physical Disk Helper Service     "C:\Program Files\VMware\VMware Tools\vmacthlp.exe"
0x937540        70      604     SERVICE_AUTO_START      SERVICE_RUNNING SERVICE_WIN32_SHARE_PROCESS      DcomLaunch      DCOM Server Process Launcher    C:\Windows\system32\svchost.exe -k DcomLaunch
0x944a50        263     712     SERVICE_AUTO_START      SERVICE_RUNNING SERVICE_WIN32_SHARE_PROCESS      RpcEptMapper    RPC Endpoint Mapper     C:\Windows\system32\svchost.exe -k RPCSS
0x942fc0        265     712     SERVICE_AUTO_START      SERVICE_RUNNING SERVICE_WIN32_SHARE_PROCESS      RpcSs   Remote Procedure Call (RPC)     C:\Windows\system32\svchost.exe -k RPCSS
0x938620        90      808     SERVICE_AUTO_START      SERVICE_RUNNING SERVICE_WIN32_SHARE_PROCESS      eventlog        Windows Event Log       C:\Windows\System32\svchost.exe -k LocalServiceNetworkRestricted
0x936910        27      844     SERVICE_AUTO_START      SERVICE_RUNNING SERVICE_WIN32_SHARE_PROCESS      AudioEndpointBuilder    Windows Audio Endpoint Builder  C:\Windows\System32\svchost.exe -k LocalSystemNetworkRestricted
0x791eb0        410     868     SERVICE_AUTO_START      SERVICE_RUNNING SERVICE_WIN32_SHARE_PROCESS      wuauserv        Windows Update  C:\Windows\system32\svchost.exe -k netsvcs
0x9395f0        102     164     SERVICE_AUTO_START      SERVICE_RUNNING SERVICE_WIN32_SHARE_PROCESS      FontCache       Windows Font Cache Service      C:\Windows\system32\svchost.exe -k LocalServiceAndNoImpersonation
0x934cc0        35      868     SERVICE_AUTO_START      SERVICE_RUNNING SERVICE_WIN32_SHARE_PROCESS      BITS    Background Intelligent Transfer Service C:\Windows\system32\svchost.exe -k netsvcs
0x94db00        349     844     SERVICE_AUTO_START      SERVICE_RUNNING SERVICE_WIN32_SHARE_PROCESS      UxSms   Desktop Window Manager Session Manager  C:\Windows\System32\svchost.exe -k LocalSystemNetworkRestricted
0x934720        28      808     SERVICE_AUTO_START      SERVICE_RUNNING SERVICE_WIN32_SHARE_PROCESS      AudioSrv        Windows Audio   C:\Windows\System32\svchost.exe -k LocalServiceNetworkRestricted
0x943b00        277     868     SERVICE_AUTO_START      SERVICE_RUNNING SERVICE_WIN32_SHARE_PROCESS      SENS    System Event Notification Service       C:\Windows\system32\svchost.exe -k netsvcs
0x93cae0        159     868     SERVICE_AUTO_START      SERVICE_RUNNING SERVICE_WIN32_SHARE_PROCESS      MMCSS   Multimedia Class Scheduler      C:\Windows\system32\svchost.exe -k netsvcs
0x937450        69      844     SERVICE_AUTO_START      SERVICE_RUNNING SERVICE_WIN32_SHARE_PROCESS      CscService      Offline Files   C:\Windows\System32\svchost.exe -k LocalSystemNetworkRestricted
0x9399b0        107     868     SERVICE_AUTO_START      SERVICE_RUNNING SERVICE_WIN32_SHARE_PROCESS      gpsvc   Group Policy Client     C:\Windows\system32\svchost.exe -k netsvcs
0x941480        237     868     SERVICE_AUTO_START      SERVICE_RUNNING SERVICE_WIN32_SHARE_PROCESS      ProfSvc User Profile Service    C:\Windows\system32\svchost.exe -k netsvcs
0x94a290        322     868     SERVICE_AUTO_START      SERVICE_RUNNING SERVICE_WIN32_SHARE_PROCESS      Themes  Themes  C:\Windows\system32\svchost.exe -k netsvcs
0x937810        73      808     SERVICE_AUTO_START      SERVICE_RUNNING SERVICE_WIN32_SHARE_PROCESS      Dhcp    DHCP Client     C:\Windows\System32\svchost.exe -k LocalServiceNetworkRestricted
0x9401a0        208     1012    SERVICE_AUTO_START      SERVICE_RUNNING SERVICE_WIN32_SHARE_PROCESS      nsi     Network Store Interface Service C:\Windows\system32\svchost.exe -k LocalService
0x93c270        150     808     SERVICE_AUTO_START      SERVICE_RUNNING SERVICE_WIN32_SHARE_PROCESS      lmhosts TCP/IP NetBIOS Helper   C:\Windows\System32\svchost.exe -k LocalServiceNetworkRestricted
0x943290        268     500     SERVICE_AUTO_START      SERVICE_RUNNING SERVICE_WIN32_SHARE_PROCESS      SamSs   Security Accounts Manager       C:\Windows\system32\lsass.exe
0x938710        91      1012    SERVICE_AUTO_START      SERVICE_RUNNING SERVICE_WIN32_SHARE_PROCESS      EventSystem     COM+ Event System       C:\Windows\system32\svchost.exe -k LocalService
0x948c10        294     1120    SERVICE_AUTO_START      SERVICE_RUNNING SERVICE_WIN32_OWN_PROCESS|SERVICE_INTERACTIVE_PROCESS    Spooler Print Spooler   C:\Windows\System32\spoolsv.exe
0x944c50        288     868     SERVICE_AUTO_START      SERVICE_RUNNING SERVICE_WIN32_SHARE_PROCESS      ShellHWDetection        Shell Hardware Detection        C:\Windows\system32\svchost.exe -k netsvcs
0x937bd0        77      620     SERVICE_AUTO_START      SERVICE_RUNNING SERVICE_WIN32_SHARE_PROCESS      Dnscache        DNS Client      C:\Windows\system32\svchost.exe -k NetworkService
0x936a20        34      1164    SERVICE_AUTO_START      SERVICE_RUNNING SERVICE_WIN32_SHARE_PROCESS      BFE     Base Filtering Engine   C:\Windows\system32\svchost.exe -k LocalServiceNoNetwork
0x940850        220     844     SERVICE_AUTO_START      SERVICE_RUNNING SERVICE_WIN32_SHARE_PROCESS      PcaSvc  Program Compatibility Assistant Service C:\Windows\System32\svchost.exe -k LocalSystemNetworkRestricted
0x939240        79      1164    SERVICE_AUTO_START      SERVICE_RUNNING SERVICE_WIN32_SHARE_PROCESS      DPS     Diagnostic Policy Service       C:\Windows\system32\svchost.exe -k LocalServiceNoNetwork
0x94a560        326     844     SERVICE_AUTO_START      SERVICE_RUNNING SERVICE_WIN32_SHARE_PROCESS      TrkWks  Distributed Link Tracking Client        C:\Windows\System32\svchost.exe -k LocalSystemNetworkRestricted
0x93f550        206     620     SERVICE_AUTO_START      SERVICE_RUNNING SERVICE_WIN32_SHARE_PROCESS      NlaSvc  Network Location Awareness      C:\Windows\system32\svchost.exe -k NetworkService
0x93d260        167     1164    SERVICE_AUTO_START      SERVICE_RUNNING SERVICE_WIN32_SHARE_PROCESS      MpsSvc  Windows Firewall        C:\Windows\system32\svchost.exe -k LocalServiceNoNetwork
0x93dbc0        147     620     SERVICE_AUTO_START      SERVICE_RUNNING SERVICE_WIN32_SHARE_PROCESS      LanmanWorkstation       Workstation     C:\Windows\system32\svchost.exe -k NetworkService
0x93f370        202     1012    SERVICE_DEMAND_START    SERVICE_RUNNING SERVICE_WIN32_SHARE_PROCESS      netprofm        Network List Service    C:\Windows\system32\svchost.exe -k LocalService
0x9490c0        300     164     SERVICE_DEMAND_START    SERVICE_RUNNING SERVICE_WIN32_SHARE_PROCESS      SSDPSRV SSDP Discovery  C:\Windows\system32\svchost.exe -k LocalServiceAndNoImpersonation
0x937360        67      620     SERVICE_AUTO_START      SERVICE_RUNNING SERVICE_WIN32_SHARE_PROCESS      CryptSvc        Cryptographic Services  C:\Windows\system32\svchost.exe -k NetworkService
0x945150        355     1356    SERVICE_AUTO_START      SERVICE_RUNNING SERVICE_WIN32_OWN_PROCESSVGAuthService   VMware Alias Manager and Ticket Service "C:\Program Files\VMware\VMware Tools\VMware VGAuth\VGAuthService.exe"
0x93dac0        146     868     SERVICE_AUTO_START      SERVICE_RUNNING SERVICE_WIN32_SHARE_PROCESS      LanmanServer    Server  C:\Windows\system32\svchost.exe -k netsvcs
0x791550        399     868     SERVICE_AUTO_START      SERVICE_RUNNING SERVICE_WIN32_SHARE_PROCESS      Winmgmt Windows Management Instrumentation      C:\Windows\system32\svchost.exe -k netsvcs
0x94e910        367     1428    SERVICE_AUTO_START      SERVICE_RUNNING SERVICE_WIN32_OWN_PROCESSVMTools VMware Tools    "C:\Program Files\VMware\VMware Tools\vmtoolsd.exe"
0x93f280        199     844     SERVICE_DEMAND_START    SERVICE_RUNNING SERVICE_WIN32_SHARE_PROCESS      Netman  Network Connections     C:\Windows\System32\svchost.exe -k LocalSystemNetworkRestricted
0x937450        69      844     SERVICE_AUTO_START      SERVICE_RUNNING SERVICE_WIN32_SHARE_PROCESS      CscService      Offline Files   C:\Windows\System32\svchost.exe -k LocalSystemNetworkRestricted
0x934720        28      808     SERVICE_AUTO_START      SERVICE_RUNNING SERVICE_WIN32_SHARE_PROCESS      AudioSrv        Windows Audio   C:\Windows\System32\svchost.exe -k LocalServiceNetworkRestricted
0x934720        28      808     SERVICE_AUTO_START      SERVICE_RUNNING SERVICE_WIN32_SHARE_PROCESS      AudioSrv        Windows Audio   C:\Windows\System32\svchost.exe -k LocalServiceNetworkRestricted
0x938350        87      N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_WIN32_OWN_PROCESSehSched Windows Media Center Scheduler Service  N/A
0x934720        28      808     SERVICE_AUTO_START      SERVICE_RUNNING SERVICE_WIN32_SHARE_PROCESS      AudioSrv        Windows Audio   C:\Windows\System32\svchost.exe -k LocalServiceNetworkRestricted
0x791dc0        409     3064    SERVICE_AUTO_START      SERVICE_RUNNING SERVICE_WIN32_OWN_PROCESSWSearch Windows Search  C:\Windows\system32\SearchIndexer.exe /Embedding
0x791dc0        409     3064    SERVICE_AUTO_START      SERVICE_RUNNING SERVICE_WIN32_OWN_PROCESSWSearch Windows Search  C:\Windows\system32\SearchIndexer.exe /Embedding
0x93b8c0        120     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_WIN32_SHARE_PROCESS      HomeGroupProvider       HomeGroup Provider      N/A
0x7923b0        413     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_WIN32_SHARE_PROCESS      WwanSvc WWAN AutoConfig N/A
0x93f280        199     844     SERVICE_DEMAND_START    SERVICE_RUNNING SERVICE_WIN32_SHARE_PROCESS      Netman  Network Connections     C:\Windows\System32\svchost.exe -k LocalSystemNetworkRestricted
0x791730        401     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_WIN32_SHARE_PROCESS      Wlansvc WLAN AutoConfig N/A
0x93f370        202     1012    SERVICE_DEMAND_START    SERVICE_RUNNING SERVICE_WIN32_SHARE_PROCESS      netprofm        Network List Service    C:\Windows\system32\svchost.exe -k LocalService
0x945450        389     1012    SERVICE_DEMAND_START    SERVICE_RUNNING SERVICE_WIN32_SHARE_PROCESS      WdiServiceHost  Diagnostic Service Host C:\Windows\system32\svchost.exe -k LocalService
0x945550        390     844     SERVICE_DEMAND_START    SERVICE_RUNNING SERVICE_WIN32_SHARE_PROCESS      WdiSystemHost   Diagnostic System Host  C:\Windows\System32\svchost.exe -k LocalSystemNetworkRestricted
0x93f550        206     620     SERVICE_AUTO_START      SERVICE_RUNNING SERVICE_WIN32_SHARE_PROCESS      NlaSvc  Network Location Awareness      C:\Windows\system32\svchost.exe -k NetworkService
0x941de0        248     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_WIN32_SHARE_PROCESS      RasMan  Remote Access Connection Manager        N/A
0x941de0        248     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_WIN32_SHARE_PROCESS      RasMan  Remote Access Connection Manager        N/A
0x9359e0        49      1948    SERVICE_DEMAND_START    SERVICE_RUNNING SERVICE_WIN32_SHARE_PROCESS      bthserv Bluetooth Support Service       C:\Windows\system32\svchost.exe -k bthsvcs
0x936a20        34      1164    SERVICE_AUTO_START      SERVICE_RUNNING SERVICE_WIN32_SHARE_PROCESS      BFE     Base Filtering Engine   C:\Windows\system32\svchost.exe -k LocalServiceNoNetwork
0x945750        398     1012    SERVICE_DEMAND_START    SERVICE_RUNNING SERVICE_WIN32_SHARE_PROCESS      WinHttpAutoProxySvc     WinHTTP Web Proxy Auto-Discovery Service        C:\Windows\system32\svchost.exe -k LocalService
0x937180        65      1324    SERVICE_DEMAND_START    SERVICE_RUNNING SERVICE_WIN32_OWN_PROCESSCOMSysApp       COM+ System Application C:\Windows\system32\dllhost.exe /Processid:{02D4B3F1-FD88-11D1-960D-00805FC79235}
0x93d8f0        174     1436    SERVICE_DEMAND_START    SERVICE_RUNNING SERVICE_WIN32_OWN_PROCESSMSDTC   Distributed Transaction Coordinator     C:\Windows\System32\msdtc.exe
0x941de0        248     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_WIN32_SHARE_PROCESS      RasMan  Remote Access Connection Manager        N/A
0x937450        69      844     SERVICE_AUTO_START      SERVICE_RUNNING SERVICE_WIN32_SHARE_PROCESS      CscService      Offline Files   C:\Windows\System32\svchost.exe -k LocalSystemNetworkRestricted
0x934bd0        33      N/A     SERVICE_SYSTEM_START    SERVICE_RUNNING SERVICE_KERNEL_DRIVER   Beep     Beep    \Driver\Beep
0x936d40        58      412     SERVICE_AUTO_START      SERVICE_RUNNING SERVICE_WIN32_OWN_PROCESSclr_optimization_v4.0.30319_32  Microsoft .NET Framework NGEN v4.0.30319_X86    C:\Windows\Microsoft.NET\Framework\v4.0.30319\mscorsvw.exe
0x9490c0        300     164     SERVICE_DEMAND_START    SERVICE_RUNNING SERVICE_WIN32_SHARE_PROCESS      SSDPSRV SSDP Discovery  C:\Windows\system32\svchost.exe -k LocalServiceAndNoImpersonation
0x948d00        295     2500    SERVICE_AUTO_START      SERVICE_RUNNING SERVICE_WIN32_OWN_PROCESSsppsvc  Software Protection     C:\Windows\system32\sppsvc.exe
0x941de0        248     N/A     SERVICE_DEMAND_START    SERVICE_STOPPED SERVICE_WIN32_SHARE_PROCESS      RasMan  Remote Access Connection Manager        N/A
0x934240        20      868     SERVICE_DEMAND_START    SERVICE_RUNNING SERVICE_WIN32_SHARE_PROCESS      Appinfo Application Information C:\Windows\system32\svchost.exe -k netsvcs
0x93b5c0        103     724     SERVICE_DEMAND_START    SERVICE_RUNNING SERVICE_WIN32_OWN_PROCESSFontCache3.0.0.0        Windows Presentation Foundation Font Cache 3.0.0.0      C:\Windows\Microsoft.Net\Framework64\v3.0\WPF\PresentationFontCache.exe

```


# windows.svcscan.SvcScan 分析

## 1. Plugin 功能說明

`windows.svcscan.SvcScan` 用來掃描 Windows 記憶體中的服務資訊，包含服務名稱、狀態、啟動方式、PID、服務類型與執行檔路徑。

在數位鑑識中，`SvcScan` 可以用來確認：

```text
系統中有哪些服務
服務是否正在執行
服務啟動方式是自動、手動或停用
服務是否對應到可疑執行檔
惡意程式是否註冊成 Windows Service
```

如果惡意程式透過服務方式常駐，通常可以在此 Plugin 中看到可疑服務名稱或異常 Binary Path。

---

## 2. 執行指令

```bash
.\vol.exe -f .\OtterCTF.vmem windows.svcscan.SvcScan
```

---

## 3. 欄位說明

| 欄位        | 說明                      |
| --------- | ----------------------- |
| `Offset`  | Service Object 在記憶體中的位置 |
| `Order`   | 服務順序                    |
| `PID`     | 服務對應的 Process ID        |
| `Start`   | 啟動方式                    |
| `State`   | 服務狀態                    |
| `Type`    | 服務類型                    |
| `Name`    | 服務名稱                    |
| `Display` | 顯示名稱                    |
| `Binary`  | 服務執行檔路徑                 |

---

## 4. 主要觀察

本次結果顯示系統存在大量正常 Windows 服務，例如：

```text
Windows Event Log
Windows Defender
Windows Update
Task Scheduler
Security Accounts Manager
Remote Procedure Call
DNS Client
DHCP Client
Windows Firewall
Windows Search
```

這些服務大多屬於 Windows 7 系統正常服務。

---

## 5. VMware 相關服務

結果中可看到多個 VMware 相關服務，例如：

```text
VMTools
VGAuthService
VMware Physical Disk Helper Service
vmci
vmhgfs
VMMEMCTL
vmrawdsk
vsock
```

其中幾個正在執行的服務包含：

```text
VMTools
VGAuthService
VMware Physical Disk Helper Service
```

其執行路徑位於：

```text
C:\Program Files\VMware\VMware Tools\
```

這些服務與本案記憶體映像來自 VMware 虛擬機環境相符，因此屬於合理現象。

需要注意的是，前面可疑的 `vmware-tray.exe` 位於：

```text
C:\Users\Rick\AppData\Local\Temp\RarSFX0\vmware-tray.exe
```

而不是 VMware Tools 正常安裝路徑。

因此，`SvcScan` 中正常的 VMware 服務，反而可以用來對比說明：真正 VMware 服務應該位於 `C:\Program Files\VMware\VMware Tools\`，而可疑 `vmware-tray.exe` 位於使用者暫存目錄，具有偽裝性。

---

## 6. WCAssistantService 觀察

本次結果中看到：

```text
WCAssistantService
Display Name: WC Assistant
PID: 3496
State: SERVICE_RUNNING
Start: SERVICE_AUTO_START
Binary: C:\Program Files (x86)\Lavasoft\Web Companion\Application\Lavasoft.WCAssistant.WinService.exe
```

此服務可對應前面分析中看到的：

```text
WebCompanionIn
WebCompanion.e
Lavasoft.WCAss
```

前面 `netscan` 也看到 WebCompanion / Lavasoft 相關程式有對外 HTTP 連線。

因此，`WCAssistantService` 可以作為系統中存在 WebCompanion / Lavasoft 軟體的證據。

不過，目前沒有證據顯示 `WCAssistantService` 是本案加密事件的主要來源，因此它應列為次要可疑或背景項目，不是本案主線。

---

## 7. 與 Rick And Morty / vmware-tray.exe 的關係

本次 `SvcScan` 結果中，沒有看到以下服務名稱或服務路徑：

```text
Rick And Morty
Rick And Morty season 1 download.exe
vmware-tray.exe
RarSFX0
READ_IT
ransom
encrypt
crypt
```

這表示目前沒有證據顯示 `Rick And Morty` 或 `vmware-tray.exe` 被註冊為 Windows Service。

這點可以配合前面結果判斷：

```text
Pstree：Rick And Morty 啟動 vmware-tray.exe
CmdLine：vmware-tray.exe 位於 Temp\RarSFX0
GetSIDs：兩者都屬於 Rick 使用者
Handles：Rick And Morty 持有 vmware-tray.exe Process handle
```

因此，本案主線較像是 Rick 使用者互動式執行可疑 EXE，而不是透過服務常駐機制執行。
