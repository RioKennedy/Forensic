# 測試內容
- vol.exe -f .\OtterCTF.vmem windows.envars.Envars

```
D:\Forensic\G140A006\VolatilityWorkbench>.\vol.exe -f .\OtterCTF.vmem windows.envars.Envars
Volatility 3 Framework 2.5.0
Progress:  100.00               PDB scanning finished
PID     Process Block   Variable        Value

260     smss.exe        0x301430        Path    C:\Windows\System32
260     smss.exe        0x301430        SystemDrive     C:
260     smss.exe        0x301430        SystemRoot      C:\Windows
348     csrss.exe       0x4018f0        ComSpec C:\Windows\system32\cmd.exe
348     csrss.exe       0x4018f0        FP_NO_HOST_CHECK        NO
348     csrss.exe       0x4018f0        NUMBER_OF_PROCESSORS    2
348     csrss.exe       0x4018f0        OS      Windows_NT
348     csrss.exe       0x4018f0        Path    C:\Windows\system32;C:\Windows;C:\Windows\System32\Wbem;C:\Windows\System32\WindowsPowerShell\v1.0\
348     csrss.exe       0x4018f0        PATHEXT .COM;.EXE;.BAT;.CMD;.VBS;.VBE;.JS;.JSE;.WSF;.WSH;.MSC
348     csrss.exe       0x4018f0        PROCESSOR_ARCHITECTURE  AMD64
348     csrss.exe       0x4018f0        PROCESSOR_IDENTIFIER    Intel64 Family 6 Model 60 Stepping 3, GenuineIntel
348     csrss.exe       0x4018f0        PROCESSOR_LEVEL 6
348     csrss.exe       0x4018f0        PROCESSOR_REVISION      3c03
348     csrss.exe       0x4018f0        PSModulePath    C:\Windows\system32\WindowsPowerShell\v1.0\Modules\
348     csrss.exe       0x4018f0        SystemDrive     C:
348     csrss.exe       0x4018f0        SystemRoot      C:\Windows
348     csrss.exe       0x4018f0        TEMP    C:\Windows\TEMP
348     csrss.exe       0x4018f0        TMP     C:\Windows\TEMP
348     csrss.exe       0x4018f0        USERNAME        SYSTEM
348     csrss.exe       0x4018f0        windir  C:\Windows
348     csrss.exe       0x4018f0        windows_tracing_flags   3
348     csrss.exe       0x4018f0        windows_tracing_logfile C:\BVTBin\Tests\installpackage\csilogfile.log
388     csrss.exe       0x4518f0        ComSpec C:\Windows\system32\cmd.exe
388     csrss.exe       0x4518f0        FP_NO_HOST_CHECK        NO
388     csrss.exe       0x4518f0        NUMBER_OF_PROCESSORS    2
388     csrss.exe       0x4518f0        OS      Windows_NT
388     csrss.exe       0x4518f0        Path    C:\Windows\system32;C:\Windows;C:\Windows\System32\Wbem;C:\Windows\System32\WindowsPowerShell\v1.0\
388     csrss.exe       0x4518f0        PATHEXT .COM;.EXE;.BAT;.CMD;.VBS;.VBE;.JS;.JSE;.WSF;.WSH;.MSC
388     csrss.exe       0x4518f0        PROCESSOR_ARCHITECTURE  AMD64
388     csrss.exe       0x4518f0        PROCESSOR_IDENTIFIER    Intel64 Family 6 Model 60 Stepping 3, GenuineIntel
388     csrss.exe       0x4518f0        PROCESSOR_LEVEL 6
388     csrss.exe       0x4518f0        PROCESSOR_REVISION      3c03
388     csrss.exe       0x4518f0        PSModulePath    C:\Windows\system32\WindowsPowerShell\v1.0\Modules\
388     csrss.exe       0x4518f0        SystemDrive     C:
388     csrss.exe       0x4518f0        SystemRoot      C:\Windows
388     csrss.exe       0x4518f0        TEMP    C:\Windows\TEMP
388     csrss.exe       0x4518f0        TMP     C:\Windows\TEMP
388     csrss.exe       0x4518f0        USERNAME        SYSTEM
388     csrss.exe       0x4518f0        windir  C:\Windows
388     csrss.exe       0x4518f0        windows_tracing_flags   3
388     csrss.exe       0x4518f0        windows_tracing_logfile C:\BVTBin\Tests\installpackage\csilogfile.log
396     wininit.exe     0x2718f0        ALLUSERSPROFILE C:\ProgramData
396     wininit.exe     0x2718f0        CommonProgramFiles      C:\Program Files\Common Files
396     wininit.exe     0x2718f0        CommonProgramFiles(x86) C:\Program Files (x86)\Common Files
396     wininit.exe     0x2718f0        CommonProgramW6432      C:\Program Files\Common Files
396     wininit.exe     0x2718f0        COMPUTERNAME    WIN-LO6FAF3DTFE
396     wininit.exe     0x2718f0        ComSpec C:\Windows\system32\cmd.exe
396     wininit.exe     0x2718f0        FP_NO_HOST_CHECK        NO
396     wininit.exe     0x2718f0        NUMBER_OF_PROCESSORS    2
396     wininit.exe     0x2718f0        OS      Windows_NT
396     wininit.exe     0x2718f0        Path    C:\Windows\system32;C:\Windows;C:\Windows\System32\Wbem;C:\Windows\System32\WindowsPowerShell\v1.0\
396     wininit.exe     0x2718f0        PATHEXT .COM;.EXE;.BAT;.CMD;.VBS;.VBE;.JS;.JSE;.WSF;.WSH;.MSC
396     wininit.exe     0x2718f0        PROCESSOR_ARCHITECTURE  AMD64
396     wininit.exe     0x2718f0        PROCESSOR_IDENTIFIER    Intel64 Family 6 Model 60 Stepping 3, GenuineIntel
396     wininit.exe     0x2718f0        PROCESSOR_LEVEL 6
396     wininit.exe     0x2718f0        PROCESSOR_REVISION      3c03
396     wininit.exe     0x2718f0        ProgramData     C:\ProgramData
396     wininit.exe     0x2718f0        ProgramFiles    C:\Program Files
396     wininit.exe     0x2718f0        ProgramFiles(x86)       C:\Program Files (x86)
396     wininit.exe     0x2718f0        ProgramW6432    C:\Program Files
396     wininit.exe     0x2718f0        PSModulePath    C:\Windows\system32\WindowsPowerShell\v1.0\Modules\
396     wininit.exe     0x2718f0        PUBLIC  C:\Users\Public
396     wininit.exe     0x2718f0        SystemDrive     C:
396     wininit.exe     0x2718f0        SystemRoot      C:\Windows
396     wininit.exe     0x2718f0        TEMP    C:\Windows\TEMP
396     wininit.exe     0x2718f0        TMP     C:\Windows\TEMP
396     wininit.exe     0x2718f0        USERNAME        SYSTEM
396     wininit.exe     0x2718f0        USERPROFILE     C:\Windows\system32\config\systemprofile
396     wininit.exe     0x2718f0        windir  C:\Windows
396     wininit.exe     0x2718f0        windows_tracing_flags   3
396     wininit.exe     0x2718f0        windows_tracing_logfile C:\BVTBin\Tests\installpackage\csilogfile.log
432     winlogon.exe    0x1818f0        ALLUSERSPROFILE C:\ProgramData
432     winlogon.exe    0x1818f0        CommonProgramFiles      C:\Program Files\Common Files
432     winlogon.exe    0x1818f0        CommonProgramFiles(x86) C:\Program Files (x86)\Common Files
432     winlogon.exe    0x1818f0        CommonProgramW6432      C:\Program Files\Common Files
432     winlogon.exe    0x1818f0        COMPUTERNAME    WIN-LO6FAF3DTFE
432     winlogon.exe    0x1818f0        ComSpec C:\Windows\system32\cmd.exe
432     winlogon.exe    0x1818f0        FP_NO_HOST_CHECK        NO
432     winlogon.exe    0x1818f0        NUMBER_OF_PROCESSORS    2
432     winlogon.exe    0x1818f0        OS      Windows_NT
432     winlogon.exe    0x1818f0        Path    C:\Windows\system32;C:\Windows;C:\Windows\System32\Wbem;C:\Windows\System32\WindowsPowerShell\v1.0\
432     winlogon.exe    0x1818f0        PATHEXT .COM;.EXE;.BAT;.CMD;.VBS;.VBE;.JS;.JSE;.WSF;.WSH;.MSC
432     winlogon.exe    0x1818f0        PROCESSOR_ARCHITECTURE  AMD64
432     winlogon.exe    0x1818f0        PROCESSOR_IDENTIFIER    Intel64 Family 6 Model 60 Stepping 3, GenuineIntel
432     winlogon.exe    0x1818f0        PROCESSOR_LEVEL 6
432     winlogon.exe    0x1818f0        PROCESSOR_REVISION      3c03
432     winlogon.exe    0x1818f0        ProgramData     C:\ProgramData
432     winlogon.exe    0x1818f0        ProgramFiles    C:\Program Files
432     winlogon.exe    0x1818f0        ProgramFiles(x86)       C:\Program Files (x86)
432     winlogon.exe    0x1818f0        ProgramW6432    C:\Program Files
432     winlogon.exe    0x1818f0        PSModulePath    C:\Windows\system32\WindowsPowerShell\v1.0\Modules\
432     winlogon.exe    0x1818f0        PUBLIC  C:\Users\Public
432     winlogon.exe    0x1818f0        SystemDrive     C:
432     winlogon.exe    0x1818f0        SystemRoot      C:\Windows
432     winlogon.exe    0x1818f0        TEMP    C:\Windows\TEMP
432     winlogon.exe    0x1818f0        TMP     C:\Windows\TEMP
432     winlogon.exe    0x1818f0        USERNAME        SYSTEM
432     winlogon.exe    0x1818f0        USERPROFILE     C:\Windows\system32\config\systemprofile
432     winlogon.exe    0x1818f0        windir  C:\Windows
432     winlogon.exe    0x1818f0        windows_tracing_flags   3
432     winlogon.exe    0x1818f0        windows_tracing_logfile C:\BVTBin\Tests\installpackage\csilogfile.log
492     services.exe    0x91c40 ALLUSERSPROFILE C:\ProgramData
492     services.exe    0x91c40 CommonProgramFiles      C:\Program Files\Common Files
492     services.exe    0x91c40 CommonProgramFiles(x86) C:\Program Files (x86)\Common Files
492     services.exe    0x91c40 CommonProgramW6432      C:\Program Files\Common Files
492     services.exe    0x91c40 COMPUTERNAME    WIN-LO6FAF3DTFE
492     services.exe    0x91c40 ComSpec C:\Windows\system32\cmd.exe
492     services.exe    0x91c40 FP_NO_HOST_CHECK        NO
492     services.exe    0x91c40 NUMBER_OF_PROCESSORS    2
492     services.exe    0x91c40 OS      Windows_NT
492     services.exe    0x91c40 Path    C:\Windows\system32;C:\Windows;C:\Windows\System32\Wbem;C:\Windows\System32\WindowsPowerShell\v1.0\
492     services.exe    0x91c40 PATHEXT .COM;.EXE;.BAT;.CMD;.VBS;.VBE;.JS;.JSE;.WSF;.WSH;.MSC
492     services.exe    0x91c40 PROCESSOR_ARCHITECTURE  AMD64
492     services.exe    0x91c40 PROCESSOR_IDENTIFIER    Intel64 Family 6 Model 60 Stepping 3, GenuineIntel
492     services.exe    0x91c40 PROCESSOR_LEVEL 6
492     services.exe    0x91c40 PROCESSOR_REVISION      3c03
492     services.exe    0x91c40 ProgramData     C:\ProgramData
492     services.exe    0x91c40 ProgramFiles    C:\Program Files
492     services.exe    0x91c40 ProgramFiles(x86)       C:\Program Files (x86)
492     services.exe    0x91c40 ProgramW6432    C:\Program Files
492     services.exe    0x91c40 PSModulePath    C:\Windows\system32\WindowsPowerShell\v1.0\Modules\
492     services.exe    0x91c40 PUBLIC  C:\Users\Public
492     services.exe    0x91c40 SystemDrive     C:
492     services.exe    0x91c40 SystemRoot      C:\Windows
492     services.exe    0x91c40 TEMP    C:\Windows\TEMP
492     services.exe    0x91c40 TMP     C:\Windows\TEMP
492     services.exe    0x91c40 USERNAME        SYSTEM
492     services.exe    0x91c40 USERPROFILE     C:\Windows\system32\config\systemprofile
492     services.exe    0x91c40 windir  C:\Windows
492     services.exe    0x91c40 windows_tracing_flags   3
492     services.exe    0x91c40 windows_tracing_logfile C:\BVTBin\Tests\installpackage\csilogfile.log
500     lsass.exe       0x481c40        ALLUSERSPROFILE C:\ProgramData
500     lsass.exe       0x481c40        CommonProgramFiles      C:\Program Files\Common Files
500     lsass.exe       0x481c40        CommonProgramFiles(x86) C:\Program Files (x86)\Common Files
500     lsass.exe       0x481c40        CommonProgramW6432      C:\Program Files\Common Files
500     lsass.exe       0x481c40        COMPUTERNAME    WIN-LO6FAF3DTFE
500     lsass.exe       0x481c40        ComSpec C:\Windows\system32\cmd.exe
500     lsass.exe       0x481c40        FP_NO_HOST_CHECK        NO
500     lsass.exe       0x481c40        NUMBER_OF_PROCESSORS    2
500     lsass.exe       0x481c40        OS      Windows_NT
500     lsass.exe       0x481c40        Path    C:\Windows\System32
500     lsass.exe       0x481c40        PATHEXT .COM;.EXE;.BAT;.CMD;.VBS;.VBE;.JS;.JSE;.WSF;.WSH;.MSC
500     lsass.exe       0x481c40        PROCESSOR_ARCHITECTURE  AMD64
500     lsass.exe       0x481c40        PROCESSOR_IDENTIFIER    Intel64 Family 6 Model 60 Stepping 3, GenuineIntel
500     lsass.exe       0x481c40        PROCESSOR_LEVEL 6
500     lsass.exe       0x481c40        PROCESSOR_REVISION      3c03
500     lsass.exe       0x481c40        ProgramData     C:\ProgramData
500     lsass.exe       0x481c40        ProgramFiles    C:\Program Files
500     lsass.exe       0x481c40        ProgramFiles(x86)       C:\Program Files (x86)
500     lsass.exe       0x481c40        ProgramW6432    C:\Program Files
500     lsass.exe       0x481c40        PSModulePath    C:\Windows\system32\WindowsPowerShell\v1.0\Modules\
500     lsass.exe       0x481c40        PUBLIC  C:\Users\Public
500     lsass.exe       0x481c40        SystemDrive     C:
500     lsass.exe       0x481c40        SystemRoot      C:\Windows
500     lsass.exe       0x481c40        TEMP    C:\Windows\TEMP
500     lsass.exe       0x481c40        TMP     C:\Windows\TEMP
500     lsass.exe       0x481c40        USERNAME        SYSTEM
500     lsass.exe       0x481c40        USERPROFILE     C:\Windows\system32\config\systemprofile
500     lsass.exe       0x481c40        windir  C:\Windows
500     lsass.exe       0x481c40        windows_tracing_flags   3
500     lsass.exe       0x481c40        windows_tracing_logfile C:\BVTBin\Tests\installpackage\csilogfile.log
500     lsass.exe       0x481c40        _flags  3
500     lsass.exe       0x481c40        windows_tracing_logfile C:\BVTBin\Tests\installpackage\csilogfile.log
508     lsm.exe 0x3d1c40        ALLUSERSPROFILE C:\ProgramData
508     lsm.exe 0x3d1c40        CommonProgramFiles      C:\Program Files\Common Files
508     lsm.exe 0x3d1c40        CommonProgramFiles(x86) C:\Program Files (x86)\Common Files
508     lsm.exe 0x3d1c40        CommonProgramW6432      C:\Program Files\Common Files
508     lsm.exe 0x3d1c40        COMPUTERNAME    WIN-LO6FAF3DTFE
508     lsm.exe 0x3d1c40        ComSpec C:\Windows\system32\cmd.exe
508     lsm.exe 0x3d1c40        FP_NO_HOST_CHECK        NO
508     lsm.exe 0x3d1c40        NUMBER_OF_PROCESSORS    2
508     lsm.exe 0x3d1c40        OS      Windows_NT
508     lsm.exe 0x3d1c40        Path    C:\Windows\system32;C:\Windows;C:\Windows\System32\Wbem;C:\Windows\System32\WindowsPowerShell\v1.0\
508     lsm.exe 0x3d1c40        PATHEXT .COM;.EXE;.BAT;.CMD;.VBS;.VBE;.JS;.JSE;.WSF;.WSH;.MSC
508     lsm.exe 0x3d1c40        PROCESSOR_ARCHITECTURE  AMD64
508     lsm.exe 0x3d1c40        PROCESSOR_IDENTIFIER    Intel64 Family 6 Model 60 Stepping 3, GenuineIntel
508     lsm.exe 0x3d1c40        PROCESSOR_LEVEL 6
508     lsm.exe 0x3d1c40        PROCESSOR_REVISION      3c03
508     lsm.exe 0x3d1c40        ProgramData     C:\ProgramData
508     lsm.exe 0x3d1c40        ProgramFiles    C:\Program Files
508     lsm.exe 0x3d1c40        ProgramFiles(x86)       C:\Program Files (x86)
508     lsm.exe 0x3d1c40        ProgramW6432    C:\Program Files
508     lsm.exe 0x3d1c40        PSModulePath    C:\Windows\system32\WindowsPowerShell\v1.0\Modules\
508     lsm.exe 0x3d1c40        PUBLIC  C:\Users\Public
508     lsm.exe 0x3d1c40        SystemDrive     C:
508     lsm.exe 0x3d1c40        SystemRoot      C:\Windows
508     lsm.exe 0x3d1c40        TEMP    C:\Windows\TEMP
508     lsm.exe 0x3d1c40        TMP     C:\Windows\TEMP
508     lsm.exe 0x3d1c40        USERNAME        SYSTEM
508     lsm.exe 0x3d1c40        USERPROFILE     C:\Windows\system32\config\systemprofile
508     lsm.exe 0x3d1c40        windir  C:\Windows
508     lsm.exe 0x3d1c40        windows_tracing_flags   3
508     lsm.exe 0x3d1c40        windows_tracing_logfile C:\BVTBin\Tests\installpackage\csilogfile.log
604     svchost.exe     0x251d90        ALLUSERSPROFILE C:\ProgramData
604     svchost.exe     0x251d90        APPDATA C:\Windows\system32\config\systemprofile\AppData\Roaming
604     svchost.exe     0x251d90        CommonProgramFiles      C:\Program Files\Common Files
604     svchost.exe     0x251d90        CommonProgramFiles(x86) C:\Program Files (x86)\Common Files
604     svchost.exe     0x251d90        CommonProgramW6432      C:\Program Files\Common Files
604     svchost.exe     0x251d90        COMPUTERNAME    WIN-LO6FAF3DTFE
604     svchost.exe     0x251d90        ComSpec C:\Windows\system32\cmd.exe
604     svchost.exe     0x251d90        FP_NO_HOST_CHECK        NO
604     svchost.exe     0x251d90        LOCALAPPDATA    C:\Windows\system32\config\systemprofile\AppData\Local
604     svchost.exe     0x251d90        NUMBER_OF_PROCESSORS    2
604     svchost.exe     0x251d90        OS      Windows_NT
604     svchost.exe     0x251d90        Path    C:\Windows\system32;C:\Windows;C:\Windows\System32\Wbem;C:\Windows\System32\WindowsPowerShell\v1.0\
604     svchost.exe     0x251d90        PATHEXT .COM;.EXE;.BAT;.CMD;.VBS;.VBE;.JS;.JSE;.WSF;.WSH;.MSC
604     svchost.exe     0x251d90        PROCESSOR_ARCHITECTURE  AMD64
604     svchost.exe     0x251d90        PROCESSOR_IDENTIFIER    Intel64 Family 6 Model 60 Stepping 3, GenuineIntel
604     svchost.exe     0x251d90        PROCESSOR_LEVEL 6
604     svchost.exe     0x251d90        PROCESSOR_REVISION      3c03
604     svchost.exe     0x251d90        ProgramData     C:\ProgramData
604     svchost.exe     0x251d90        ProgramFiles    C:\Program Files
604     svchost.exe     0x251d90        ProgramFiles(x86)       C:\Program Files (x86)
604     svchost.exe     0x251d90        ProgramW6432    C:\Program Files
604     svchost.exe     0x251d90        PSModulePath    C:\Windows\system32\WindowsPowerShell\v1.0\Modules\
604     svchost.exe     0x251d90        PUBLIC  C:\Users\Public
604     svchost.exe     0x251d90        SystemDrive     C:
604     svchost.exe     0x251d90        SystemRoot      C:\Windows
604     svchost.exe     0x251d90        TEMP    C:\Windows\TEMP
604     svchost.exe     0x251d90        TMP     C:\Windows\TEMP
604     svchost.exe     0x251d90        USERDOMAIN      WORKGROUP
604     svchost.exe     0x251d90        USERNAME        WIN-LO6FAF3DTFE$
604     svchost.exe     0x251d90        USERPROFILE     C:\Windows\system32\config\systemprofile
604     svchost.exe     0x251d90        windir  C:\Windows
604     svchost.exe     0x251d90        windows_tracing_flags   3
604     svchost.exe     0x251d90        windows_tracing_logfile C:\BVTBin\Tests\installpackage\csilogfile.log
668     vmacthlp.exe    0x421d90        ALLUSERSPROFILE C:\ProgramData
668     vmacthlp.exe    0x421d90        APPDATA C:\Windows\system32\config\systemprofile\AppData\Roaming
668     vmacthlp.exe    0x421d90        CommonProgramFiles      C:\Program Files\Common Files
668     vmacthlp.exe    0x421d90        CommonProgramFiles(x86) C:\Program Files (x86)\Common Files
668     vmacthlp.exe    0x421d90        CommonProgramW6432      C:\Program Files\Common Files
668     vmacthlp.exe    0x421d90        COMPUTERNAME    WIN-LO6FAF3DTFE
668     vmacthlp.exe    0x421d90        ComSpec C:\Windows\system32\cmd.exe
668     vmacthlp.exe    0x421d90        FP_NO_HOST_CHECK        NO
668     vmacthlp.exe    0x421d90        LOCALAPPDATA    C:\Windows\system32\config\systemprofile\AppData\Local
668     vmacthlp.exe    0x421d90        NUMBER_OF_PROCESSORS    2
668     vmacthlp.exe    0x421d90        OS      Windows_NT
668     vmacthlp.exe    0x421d90        Path    C:\Windows\system32;C:\Windows;C:\Windows\System32\Wbem;C:\Windows\System32\WindowsPowerShell\v1.0\;
668     vmacthlp.exe    0x421d90        PATHEXT .COM;.EXE;.BAT;.CMD;.VBS;.VBE;.JS;.JSE;.WSF;.WSH;.MSC
668     vmacthlp.exe    0x421d90        PROCESSOR_ARCHITECTURE  AMD64
668     vmacthlp.exe    0x421d90        PROCESSOR_IDENTIFIER    Intel64 Family 6 Model 60 Stepping 3, GenuineIntel
668     vmacthlp.exe    0x421d90        PROCESSOR_LEVEL 6
668     vmacthlp.exe    0x421d90        PROCESSOR_REVISION      3c03
668     vmacthlp.exe    0x421d90        ProgramData     C:\ProgramData
668     vmacthlp.exe    0x421d90        ProgramFiles    C:\Program Files
668     vmacthlp.exe    0x421d90        ProgramFiles(x86)       C:\Program Files (x86)
668     vmacthlp.exe    0x421d90        ProgramW6432    C:\Program Files
668     vmacthlp.exe    0x421d90        PSModulePath    C:\Windows\system32\WindowsPowerShell\v1.0\Modules\
668     vmacthlp.exe    0x421d90        PUBLIC  C:\Users\Public
668     vmacthlp.exe    0x421d90        SystemDrive     C:
668     vmacthlp.exe    0x421d90        SystemRoot      C:\Windows
668     vmacthlp.exe    0x421d90        TEMP    C:\Windows\TEMP
668     vmacthlp.exe    0x421d90        TMP     C:\Windows\TEMP
668     vmacthlp.exe    0x421d90        USERDOMAIN      WORKGROUP
668     vmacthlp.exe    0x421d90        USERNAME        WIN-LO6FAF3DTFE$
668     vmacthlp.exe    0x421d90        USERPROFILE     C:\Windows\system32\config\systemprofile
668     vmacthlp.exe    0x421d90        windir  C:\Windows
668     vmacthlp.exe    0x421d90        windows_tracing_flags   3
668     vmacthlp.exe    0x421d90        windows_tracing_logfile C:\BVTBin\Tests\installpackage\csilogfile.log
712     svchost.exe     0x2a1e10        ALLUSERSPROFILE C:\ProgramData
712     svchost.exe     0x2a1e10        APPDATA C:\Windows\ServiceProfiles\NetworkService\AppData\Roaming
712     svchost.exe     0x2a1e10        CommonProgramFiles      C:\Program Files\Common Files
712     svchost.exe     0x2a1e10        CommonProgramFiles(x86) C:\Program Files (x86)\Common Files
712     svchost.exe     0x2a1e10        CommonProgramW6432      C:\Program Files\Common Files
712     svchost.exe     0x2a1e10        COMPUTERNAME    WIN-LO6FAF3DTFE
712     svchost.exe     0x2a1e10        ComSpec C:\Windows\system32\cmd.exe
712     svchost.exe     0x2a1e10        FP_NO_HOST_CHECK        NO
712     svchost.exe     0x2a1e10        LOCALAPPDATA    C:\Windows\ServiceProfiles\NetworkService\AppData\Local
712     svchost.exe     0x2a1e10        NUMBER_OF_PROCESSORS    2
712     svchost.exe     0x2a1e10        OS      Windows_NT
712     svchost.exe     0x2a1e10        Path    C:\Windows\system32;C:\Windows;C:\Windows\System32\Wbem;C:\Windows\System32\WindowsPowerShell\v1.0\
712     svchost.exe     0x2a1e10        PATHEXT .COM;.EXE;.BAT;.CMD;.VBS;.VBE;.JS;.JSE;.WSF;.WSH;.MSC
712     svchost.exe     0x2a1e10        PROCESSOR_ARCHITECTURE  AMD64
712     svchost.exe     0x2a1e10        PROCESSOR_IDENTIFIER    Intel64 Family 6 Model 60 Stepping 3, GenuineIntel
712     svchost.exe     0x2a1e10        PROCESSOR_LEVEL 6
712     svchost.exe     0x2a1e10        PROCESSOR_REVISION      3c03
712     svchost.exe     0x2a1e10        ProgramData     C:\ProgramData
712     svchost.exe     0x2a1e10        ProgramFiles    C:\Program Files
712     svchost.exe     0x2a1e10        ProgramFiles(x86)       C:\Program Files (x86)
712     svchost.exe     0x2a1e10        ProgramW6432    C:\Program Files
712     svchost.exe     0x2a1e10        PSModulePath    C:\Windows\system32\WindowsPowerShell\v1.0\Modules\
712     svchost.exe     0x2a1e10        PUBLIC  C:\Users\Public
712     svchost.exe     0x2a1e10        SystemDrive     C:
712     svchost.exe     0x2a1e10        SystemRoot      C:\Windows
712     svchost.exe     0x2a1e10        TEMP    C:\Windows\SERVIC~2\NETWOR~1\AppData\Local\Temp
712     svchost.exe     0x2a1e10        TMP     C:\Windows\SERVIC~2\NETWOR~1\AppData\Local\Temp
712     svchost.exe     0x2a1e10        USERDOMAIN      WORKGROUP
712     svchost.exe     0x2a1e10        USERNAME        WIN-LO6FAF3DTFE$
712     svchost.exe     0x2a1e10        USERPROFILE     C:\Windows\ServiceProfiles\NetworkService
712     svchost.exe     0x2a1e10        windir  C:\Windows
712     svchost.exe     0x2a1e10        windows_tracing_flags   3
712     svchost.exe     0x2a1e10        windows_tracing_logfile C:\BVTBin\Tests\installpackage\csilogfile.log
808     svchost.exe     0x261e00        ALLUSERSPROFILE C:\ProgramData
808     svchost.exe     0x261e00        APPDATA C:\Windows\ServiceProfiles\LocalService\AppData\Roaming
808     svchost.exe     0x261e00        CommonProgramFiles      C:\Program Files\Common Files
808     svchost.exe     0x261e00        CommonProgramFiles(x86) C:\Program Files (x86)\Common Files
808     svchost.exe     0x261e00        CommonProgramW6432      C:\Program Files\Common Files
808     svchost.exe     0x261e00        COMPUTERNAME    WIN-LO6FAF3DTFE
808     svchost.exe     0x261e00        ComSpec C:\Windows\system32\cmd.exe
808     svchost.exe     0x261e00        FP_NO_HOST_CHECK        NO
808     svchost.exe     0x261e00        LOCALAPPDATA    C:\Windows\ServiceProfiles\LocalService\AppData\Local
808     svchost.exe     0x261e00        NUMBER_OF_PROCESSORS    2
808     svchost.exe     0x261e00        OS      Windows_NT
808     svchost.exe     0x261e00        Path    C:\Windows\system32;C:\Windows;C:\Windows\System32\Wbem;C:\Windows\System32\WindowsPowerShell\v1.0\
808     svchost.exe     0x261e00        PATHEXT .COM;.EXE;.BAT;.CMD;.VBS;.VBE;.JS;.JSE;.WSF;.WSH;.MSC
808     svchost.exe     0x261e00        PROCESSOR_ARCHITECTURE  AMD64
808     svchost.exe     0x261e00        PROCESSOR_IDENTIFIER    Intel64 Family 6 Model 60 Stepping 3, GenuineIntel
808     svchost.exe     0x261e00        PROCESSOR_LEVEL 6
808     svchost.exe     0x261e00        PROCESSOR_REVISION      3c03
808     svchost.exe     0x261e00        ProgramData     C:\ProgramData
808     svchost.exe     0x261e00        ProgramFiles    C:\Program Files
808     svchost.exe     0x261e00        ProgramFiles(x86)       C:\Program Files (x86)
808     svchost.exe     0x261e00        ProgramW6432    C:\Program Files
808     svchost.exe     0x261e00        PSModulePath    C:\Windows\system32\WindowsPowerShell\v1.0\Modules\
808     svchost.exe     0x261e00        PUBLIC  C:\Users\Public
808     svchost.exe     0x261e00        SystemDrive     C:
808     svchost.exe     0x261e00        SystemRoot      C:\Windows
808     svchost.exe     0x261e00        TEMP    C:\Windows\SERVIC~2\LOCALS~1\AppData\Local\Temp
808     svchost.exe     0x261e00        TMP     C:\Windows\SERVIC~2\LOCALS~1\AppData\Local\Temp
808     svchost.exe     0x261e00        USERDOMAIN      NT AUTHORITY
808     svchost.exe     0x261e00        USERNAME        LOCAL SERVICE
808     svchost.exe     0x261e00        USERPROFILE     C:\Windows\ServiceProfiles\LocalService
808     svchost.exe     0x261e00        windir  C:\Windows
808     svchost.exe     0x261e00        windows_tracing_flags   3
808     svchost.exe     0x261e00        windows_tracing_logfile C:\BVTBin\Tests\installpackage\csilogfile.log
844     svchost.exe     0x1b1d90        ALLUSERSPROFILE C:\ProgramData
844     svchost.exe     0x1b1d90        APPDATA C:\Windows\system32\config\systemprofile\AppData\Roaming
844     svchost.exe     0x1b1d90        CommonProgramFiles      C:\Program Files\Common Files
844     svchost.exe     0x1b1d90        CommonProgramFiles(x86) C:\Program Files (x86)\Common Files
844     svchost.exe     0x1b1d90        CommonProgramW6432      C:\Program Files\Common Files
844     svchost.exe     0x1b1d90        COMPUTERNAME    WIN-LO6FAF3DTFE
844     svchost.exe     0x1b1d90        ComSpec C:\Windows\system32\cmd.exe
844     svchost.exe     0x1b1d90        FP_NO_HOST_CHECK        NO
844     svchost.exe     0x1b1d90        LOCALAPPDATA    C:\Windows\system32\config\systemprofile\AppData\Local
844     svchost.exe     0x1b1d90        NUMBER_OF_PROCESSORS    2
844     svchost.exe     0x1b1d90        OS      Windows_NT
844     svchost.exe     0x1b1d90        Path    C:\Windows\system32;C:\Windows;C:\Windows\System32\Wbem;C:\Windows\System32\WindowsPowerShell\v1.0\
844     svchost.exe     0x1b1d90        PATHEXT .COM;.EXE;.BAT;.CMD;.VBS;.VBE;.JS;.JSE;.WSF;.WSH;.MSC
844     svchost.exe     0x1b1d90        PROCESSOR_ARCHITECTURE  AMD64
844     svchost.exe     0x1b1d90        PROCESSOR_IDENTIFIER    Intel64 Family 6 Model 60 Stepping 3, GenuineIntel
844     svchost.exe     0x1b1d90        PROCESSOR_LEVEL 6
844     svchost.exe     0x1b1d90        PROCESSOR_REVISION      3c03
844     svchost.exe     0x1b1d90        ProgramData     C:\ProgramData
844     svchost.exe     0x1b1d90        ProgramFiles    C:\Program Files
844     svchost.exe     0x1b1d90        ProgramFiles(x86)       C:\Program Files (x86)
844     svchost.exe     0x1b1d90        ProgramW6432    C:\Program Files
844     svchost.exe     0x1b1d90        PSModulePath    C:\Windows\system32\WindowsPowerShell\v1.0\Modules\
844     svchost.exe     0x1b1d90        PUBLIC  C:\Users\Public
844     svchost.exe     0x1b1d90        SystemDrive     C:
844     svchost.exe     0x1b1d90        SystemRoot      C:\Windows
844     svchost.exe     0x1b1d90        TEMP    C:\Windows\TEMP
844     svchost.exe     0x1b1d90        TMP     C:\Windows\TEMP
844     svchost.exe     0x1b1d90        USERDOMAIN      WORKGROUP
844     svchost.exe     0x1b1d90        USERNAME        WIN-LO6FAF3DTFE$
844     svchost.exe     0x1b1d90        USERPROFILE     C:\Windows\system32\config\systemprofile
844     svchost.exe     0x1b1d90        windir  C:\Windows
844     svchost.exe     0x1b1d90        windows_tracing_flags   3
844     svchost.exe     0x1b1d90        windows_tracing_logfile C:\BVTBin\Tests\installpackage\csilogfile.log
868     svchost.exe     0x341d90        ALLUSERSPROFILE C:\ProgramData
868     svchost.exe     0x341d90        APPDATA C:\Windows\system32\config\systemprofile\AppData\Roaming
868     svchost.exe     0x341d90        CommonProgramFiles      C:\Program Files\Common Files
868     svchost.exe     0x341d90        CommonProgramFiles(x86) C:\Program Files (x86)\Common Files
868     svchost.exe     0x341d90        CommonProgramW6432      C:\Program Files\Common Files
868     svchost.exe     0x341d90        COMPUTERNAME    WIN-LO6FAF3DTFE
868     svchost.exe     0x341d90        ComSpec C:\Windows\system32\cmd.exe
868     svchost.exe     0x341d90        FP_NO_HOST_CHECK        NO
868     svchost.exe     0x341d90        LOCALAPPDATA    C:\Windows\system32\config\systemprofile\AppData\Local
868     svchost.exe     0x341d90        NUMBER_OF_PROCESSORS    2
868     svchost.exe     0x341d90        OS      Windows_NT
868     svchost.exe     0x341d90        Path    C:\Windows\system32;C:\Windows;C:\Windows\System32\Wbem;C:\Windows\System32\WindowsPowerShell\v1.0\
868     svchost.exe     0x341d90        PATHEXT .COM;.EXE;.BAT;.CMD;.VBS;.VBE;.JS;.JSE;.WSF;.WSH;.MSC
868     svchost.exe     0x341d90        PROCESSOR_ARCHITECTURE  AMD64
868     svchost.exe     0x341d90        PROCESSOR_IDENTIFIER    Intel64 Family 6 Model 60 Stepping 3, GenuineIntel
868     svchost.exe     0x341d90        PROCESSOR_LEVEL 6
868     svchost.exe     0x341d90        PROCESSOR_REVISION      3c03
868     svchost.exe     0x341d90        ProgramData     C:\ProgramData
868     svchost.exe     0x341d90        ProgramFiles    C:\Program Files
868     svchost.exe     0x341d90        ProgramFiles(x86)       C:\Program Files (x86)
868     svchost.exe     0x341d90        ProgramW6432    C:\Program Files
868     svchost.exe     0x341d90        PSModulePath    C:\Windows\system32\WindowsPowerShell\v1.0\Modules\
868     svchost.exe     0x341d90        PUBLIC  C:\Users\Public
868     svchost.exe     0x341d90        SystemDrive     C:
868     svchost.exe     0x341d90        SystemRoot      C:\Windows
868     svchost.exe     0x341d90        TEMP    C:\Windows\TEMP
868     svchost.exe     0x341d90        TMP     C:\Windows\TEMP
868     svchost.exe     0x341d90        USERDOMAIN      WORKGROUP
868     svchost.exe     0x341d90        USERNAME        WIN-LO6FAF3DTFE$
868     svchost.exe     0x341d90        USERPROFILE     C:\Windows\system32\config\systemprofile
868     svchost.exe     0x341d90        windir  C:\Windows
868     svchost.exe     0x341d90        windows_tracing_flags   3
868     svchost.exe     0x341d90        windows_tracing_logfile C:\BVTBin\Tests\installpackage\csilogfile.log
960     audiodg.exe     0x31430 Path    C:\Windows\System32
960     audiodg.exe     0x31430 SystemDrive     C:
960     audiodg.exe     0x31430 SystemRoot      C:\Windows
1012    svchost.exe     0x241e00        ALLUSERSPROFILE C:\ProgramData
1012    svchost.exe     0x241e00        APPDATA C:\Windows\ServiceProfiles\LocalService\AppData\Roaming
1012    svchost.exe     0x241e00        CommonProgramFiles      C:\Program Files\Common Files
1012    svchost.exe     0x241e00        CommonProgramFiles(x86) C:\Program Files (x86)\Common Files
1012    svchost.exe     0x241e00        CommonProgramW6432      C:\Program Files\Common Files
1012    svchost.exe     0x241e00        COMPUTERNAME    WIN-LO6FAF3DTFE
1012    svchost.exe     0x241e00        ComSpec C:\Windows\system32\cmd.exe
1012    svchost.exe     0x241e00        FP_NO_HOST_CHECK        NO
1012    svchost.exe     0x241e00        LOCALAPPDATA    C:\Windows\ServiceProfiles\LocalService\AppData\Local
1012    svchost.exe     0x241e00        NUMBER_OF_PROCESSORS    2
1012    svchost.exe     0x241e00        OS      Windows_NT
1012    svchost.exe     0x241e00        Path    C:\Windows\system32;C:\Windows;C:\Windows\System32\Wbem;C:\Windows\System32\WindowsPowerShell\v1.0\
1012    svchost.exe     0x241e00        PATHEXT .COM;.EXE;.BAT;.CMD;.VBS;.VBE;.JS;.JSE;.WSF;.WSH;.MSC
1012    svchost.exe     0x241e00        PROCESSOR_ARCHITECTURE  AMD64
1012    svchost.exe     0x241e00        PROCESSOR_IDENTIFIER    Intel64 Family 6 Model 60 Stepping 3, GenuineIntel
1012    svchost.exe     0x241e00        PROCESSOR_LEVEL 6
1012    svchost.exe     0x241e00        PROCESSOR_REVISION      3c03
1012    svchost.exe     0x241e00        ProgramData     C:\ProgramData
1012    svchost.exe     0x241e00        ProgramFiles    C:\Program Files
1012    svchost.exe     0x241e00        ProgramFiles(x86)       C:\Program Files (x86)
1012    svchost.exe     0x241e00        ProgramW6432    C:\Program Files
1012    svchost.exe     0x241e00        PSModulePath    C:\Windows\system32\WindowsPowerShell\v1.0\Modules\
1012    svchost.exe     0x241e00        PUBLIC  C:\Users\Public
1012    svchost.exe     0x241e00        SystemDrive     C:
1012    svchost.exe     0x241e00        SystemRoot      C:\Windows
1012    svchost.exe     0x241e00        TEMP    C:\Windows\SERVIC~2\LOCALS~1\AppData\Local\Temp
1012    svchost.exe     0x241e00        TMP     C:\Windows\SERVIC~2\LOCALS~1\AppData\Local\Temp
1012    svchost.exe     0x241e00        USERDOMAIN      NT AUTHORITY
1012    svchost.exe     0x241e00        USERNAME        LOCAL SERVICE
1012    svchost.exe     0x241e00        USERPROFILE     C:\Windows\ServiceProfiles\LocalService
1012    svchost.exe     0x241e00        windir  C:\Windows
1012    svchost.exe     0x241e00        windows_tracing_flags   3
1012    svchost.exe     0x241e00        windows_tracing_logfile C:\BVTBin\Tests\installpackage\csilogfile.log
620     svchost.exe     0x2c1e10        ALLUSERSPROFILE C:\ProgramData
620     svchost.exe     0x2c1e10        APPDATA C:\Windows\ServiceProfiles\NetworkService\AppData\Roaming
620     svchost.exe     0x2c1e10        CommonProgramFiles      C:\Program Files\Common Files
620     svchost.exe     0x2c1e10        CommonProgramFiles(x86) C:\Program Files (x86)\Common Files
620     svchost.exe     0x2c1e10        CommonProgramW6432      C:\Program Files\Common Files
620     svchost.exe     0x2c1e10        COMPUTERNAME    WIN-LO6FAF3DTFE
620     svchost.exe     0x2c1e10        ComSpec C:\Windows\system32\cmd.exe
620     svchost.exe     0x2c1e10        FP_NO_HOST_CHECK        NO
620     svchost.exe     0x2c1e10        LOCALAPPDATA    C:\Windows\ServiceProfiles\NetworkService\AppData\Local
620     svchost.exe     0x2c1e10        NUMBER_OF_PROCESSORS    2
620     svchost.exe     0x2c1e10        OS      Windows_NT
620     svchost.exe     0x2c1e10        Path    C:\Windows\system32;C:\Windows;C:\Windows\System32\Wbem;C:\Windows\System32\WindowsPowerShell\v1.0\
620     svchost.exe     0x2c1e10        PATHEXT .COM;.EXE;.BAT;.CMD;.VBS;.VBE;.JS;.JSE;.WSF;.WSH;.MSC
620     svchost.exe     0x2c1e10        PROCESSOR_ARCHITECTURE  AMD64
620     svchost.exe     0x2c1e10        PROCESSOR_IDENTIFIER    Intel64 Family 6 Model 60 Stepping 3, GenuineIntel
620     svchost.exe     0x2c1e10        PROCESSOR_LEVEL 6
620     svchost.exe     0x2c1e10        PROCESSOR_REVISION      3c03
620     svchost.exe     0x2c1e10        ProgramData     C:\ProgramData
620     svchost.exe     0x2c1e10        ProgramFiles    C:\Program Files
620     svchost.exe     0x2c1e10        ProgramFiles(x86)       C:\Program Files (x86)
620     svchost.exe     0x2c1e10        ProgramW6432    C:\Program Files
620     svchost.exe     0x2c1e10        PSModulePath    C:\Windows\system32\WindowsPowerShell\v1.0\Modules\
620     svchost.exe     0x2c1e10        PUBLIC  C:\Users\Public
620     svchost.exe     0x2c1e10        SystemDrive     C:
620     svchost.exe     0x2c1e10        SystemRoot      C:\Windows
620     svchost.exe     0x2c1e10        TEMP    C:\Windows\SERVIC~2\NETWOR~1\AppData\Local\Temp
620     svchost.exe     0x2c1e10        TMP     C:\Windows\SERVIC~2\NETWOR~1\AppData\Local\Temp
620     svchost.exe     0x2c1e10        USERDOMAIN      WORKGROUP
620     svchost.exe     0x2c1e10        USERNAME        WIN-LO6FAF3DTFE$
620     svchost.exe     0x2c1e10        USERPROFILE     C:\Windows\ServiceProfiles\NetworkService
620     svchost.exe     0x2c1e10        windir  C:\Windows
620     svchost.exe     0x2c1e10        windows_tracing_flags   3
620     svchost.exe     0x2c1e10        windows_tracing_logfile C:\BVTBin\Tests\installpackage\csilogfile.log
1120    spoolsv.exe     0x131d90        ALLUSERSPROFILE C:\ProgramData
1120    spoolsv.exe     0x131d90        APPDATA C:\Windows\system32\config\systemprofile\AppData\Roaming
1120    spoolsv.exe     0x131d90        CommonProgramFiles      C:\Program Files\Common Files
1120    spoolsv.exe     0x131d90        CommonProgramFiles(x86) C:\Program Files (x86)\Common Files
1120    spoolsv.exe     0x131d90        CommonProgramW6432      C:\Program Files\Common Files
1120    spoolsv.exe     0x131d90        COMPUTERNAME    WIN-LO6FAF3DTFE
1120    spoolsv.exe     0x131d90        ComSpec C:\Windows\system32\cmd.exe
1120    spoolsv.exe     0x131d90        FP_NO_HOST_CHECK        NO
1120    spoolsv.exe     0x131d90        LOCALAPPDATA    C:\Windows\system32\config\systemprofile\AppData\Local
1120    spoolsv.exe     0x131d90        NUMBER_OF_PROCESSORS    2
1120    spoolsv.exe     0x131d90        OS      Windows_NT
1120    spoolsv.exe     0x131d90        Path    C:\Windows\system32;C:\Windows;C:\Windows\System32\Wbem;C:\Windows\System32\WindowsPowerShell\v1.0\
1120    spoolsv.exe     0x131d90        PATHEXT .COM;.EXE;.BAT;.CMD;.VBS;.VBE;.JS;.JSE;.WSF;.WSH;.MSC
1120    spoolsv.exe     0x131d90        PROCESSOR_ARCHITECTURE  AMD64
1120    spoolsv.exe     0x131d90        PROCESSOR_IDENTIFIER    Intel64 Family 6 Model 60 Stepping 3, GenuineIntel
1120    spoolsv.exe     0x131d90        PROCESSOR_LEVEL 6
1120    spoolsv.exe     0x131d90        PROCESSOR_REVISION      3c03
1120    spoolsv.exe     0x131d90        ProgramData     C:\ProgramData
1120    spoolsv.exe     0x131d90        ProgramFiles    C:\Program Files
1120    spoolsv.exe     0x131d90        ProgramFiles(x86)       C:\Program Files (x86)
1120    spoolsv.exe     0x131d90        ProgramW6432    C:\Program Files
1120    spoolsv.exe     0x131d90        PSModulePath    C:\Windows\system32\WindowsPowerShell\v1.0\Modules\
1120    spoolsv.exe     0x131d90        PUBLIC  C:\Users\Public
1120    spoolsv.exe     0x131d90        SystemDrive     C:
1120    spoolsv.exe     0x131d90        SystemRoot      C:\Windows
1120    spoolsv.exe     0x131d90        TEMP    C:\Windows\TEMP
1120    spoolsv.exe     0x131d90        TMP     C:\Windows\TEMP
1120    spoolsv.exe     0x131d90        USERDOMAIN      WORKGROUP
1120    spoolsv.exe     0x131d90        USERNAME        WIN-LO6FAF3DTFE$
1120    spoolsv.exe     0x131d90        USERPROFILE     C:\Windows\system32\config\systemprofile
1120    spoolsv.exe     0x131d90        windir  C:\Windows
1120    spoolsv.exe     0x131d90        windows_tracing_flags   3
1120    spoolsv.exe     0x131d90        windows_tracing_logfile C:\BVTBin\Tests\installpackage\csilogfile.log
1164    svchost.exe     0x291e00        ALLUSERSPROFILE C:\ProgramData
1164    svchost.exe     0x291e00        APPDATA C:\Windows\ServiceProfiles\LocalService\AppData\Roaming
1164    svchost.exe     0x291e00        CommonProgramFiles      C:\Program Files\Common Files
1164    svchost.exe     0x291e00        CommonProgramFiles(x86) C:\Program Files (x86)\Common Files
1164    svchost.exe     0x291e00        CommonProgramW6432      C:\Program Files\Common Files
1164    svchost.exe     0x291e00        COMPUTERNAME    WIN-LO6FAF3DTFE
1164    svchost.exe     0x291e00        ComSpec C:\Windows\system32\cmd.exe
1164    svchost.exe     0x291e00        FP_NO_HOST_CHECK        NO
1164    svchost.exe     0x291e00        LOCALAPPDATA    C:\Windows\ServiceProfiles\LocalService\AppData\Local
1164    svchost.exe     0x291e00        NUMBER_OF_PROCESSORS    2
1164    svchost.exe     0x291e00        OS      Windows_NT
1164    svchost.exe     0x291e00        Path    C:\Windows\system32;C:\Windows;C:\Windows\System32\Wbem;C:\Windows\System32\WindowsPowerShell\v1.0\
1164    svchost.exe     0x291e00        PATHEXT .COM;.EXE;.BAT;.CMD;.VBS;.VBE;.JS;.JSE;.WSF;.WSH;.MSC
1164    svchost.exe     0x291e00        PROCESSOR_ARCHITECTURE  AMD64
1164    svchost.exe     0x291e00        PROCESSOR_IDENTIFIER    Intel64 Family 6 Model 60 Stepping 3, GenuineIntel
1164    svchost.exe     0x291e00        PROCESSOR_LEVEL 6
1164    svchost.exe     0x291e00        PROCESSOR_REVISION      3c03
1164    svchost.exe     0x291e00        ProgramData     C:\ProgramData
1164    svchost.exe     0x291e00        ProgramFiles    C:\Program Files
1164    svchost.exe     0x291e00        ProgramFiles(x86)       C:\Program Files (x86)
1164    svchost.exe     0x291e00        ProgramW6432    C:\Program Files
1164    svchost.exe     0x291e00        PSModulePath    C:\Windows\system32\WindowsPowerShell\v1.0\Modules\
1164    svchost.exe     0x291e00        PUBLIC  C:\Users\Public
1164    svchost.exe     0x291e00        SystemDrive     C:
1164    svchost.exe     0x291e00        SystemRoot      C:\Windows
1164    svchost.exe     0x291e00        TEMP    C:\Windows\SERVIC~2\LOCALS~1\AppData\Local\Temp
1164    svchost.exe     0x291e00        TMP     C:\Windows\SERVIC~2\LOCALS~1\AppData\Local\Temp
1164    svchost.exe     0x291e00        USERDOMAIN      NT AUTHORITY
1164    svchost.exe     0x291e00        USERNAME        LOCAL SERVICE
1164    svchost.exe     0x291e00        USERPROFILE     C:\Windows\ServiceProfiles\LocalService
1164    svchost.exe     0x291e00        windir  C:\Windows
1164    svchost.exe     0x291e00        windows_tracing_flags   3
1164    svchost.exe     0x291e00        windows_tracing_logfile C:\BVTBin\Tests\installpackage\csilogfile.log
1356    VGAuthService.  0x2c1d90        ALLUSERSPROFILE C:\ProgramData
1356    VGAuthService.  0x2c1d90        APPDATA C:\Windows\system32\config\systemprofile\AppData\Roaming
1356    VGAuthService.  0x2c1d90        CommonProgramFiles      C:\Program Files\Common Files
1356    VGAuthService.  0x2c1d90        CommonProgramFiles(x86) C:\Program Files (x86)\Common Files
1356    VGAuthService.  0x2c1d90        CommonProgramW6432      C:\Program Files\Common Files
1356    VGAuthService.  0x2c1d90        COMPUTERNAME    WIN-LO6FAF3DTFE
1356    VGAuthService.  0x2c1d90        ComSpec C:\Windows\system32\cmd.exe
1356    VGAuthService.  0x2c1d90        FP_NO_HOST_CHECK        NO
1356    VGAuthService.  0x2c1d90        LOCALAPPDATA    C:\Windows\system32\config\systemprofile\AppData\Local
1356    VGAuthService.  0x2c1d90        NUMBER_OF_PROCESSORS    2
1356    VGAuthService.  0x2c1d90        OS      Windows_NT
1356    VGAuthService.  0x2c1d90        Path    C:\Windows\system32;C:\Windows;C:\Windows\System32\Wbem;C:\Windows\System32\WindowsPowerShell\v1.0\;
1356    VGAuthService.  0x2c1d90        PATHEXT .COM;.EXE;.BAT;.CMD;.VBS;.VBE;.JS;.JSE;.WSF;.WSH;.MSC
1356    VGAuthService.  0x2c1d90        PROCESSOR_ARCHITECTURE  AMD64
1356    VGAuthService.  0x2c1d90        PROCESSOR_IDENTIFIER    Intel64 Family 6 Model 60 Stepping 3, GenuineIntel
1356    VGAuthService.  0x2c1d90        PROCESSOR_LEVEL 6
1356    VGAuthService.  0x2c1d90        PROCESSOR_REVISION      3c03
1356    VGAuthService.  0x2c1d90        ProgramData     C:\ProgramData
1356    VGAuthService.  0x2c1d90        ProgramFiles    C:\Program Files
1356    VGAuthService.  0x2c1d90        ProgramFiles(x86)       C:\Program Files (x86)
1356    VGAuthService.  0x2c1d90        ProgramW6432    C:\Program Files
1356    VGAuthService.  0x2c1d90        PSModulePath    C:\Windows\system32\WindowsPowerShell\v1.0\Modules\
1356    VGAuthService.  0x2c1d90        PUBLIC  C:\Users\Public
1356    VGAuthService.  0x2c1d90        SystemDrive     C:
1356    VGAuthService.  0x2c1d90        SystemRoot      C:\Windows
1356    VGAuthService.  0x2c1d90        TEMP    C:\Windows\TEMP
1356    VGAuthService.  0x2c1d90        TMP     C:\Windows\TEMP
1356    VGAuthService.  0x2c1d90        USERDOMAIN      WORKGROUP
1356    VGAuthService.  0x2c1d90        USERNAME        WIN-LO6FAF3DTFE$
1356    VGAuthService.  0x2c1d90        USERPROFILE     C:\Windows\system32\config\systemprofile
1356    VGAuthService.  0x2c1d90        windir  C:\Windows
1356    VGAuthService.  0x2c1d90        windows_tracing_flags   3
1356    VGAuthService.  0x2c1d90        windows_tracing_logfile C:\BVTBin\Tests\installpackage\csilogfile.log
1428    vmtoolsd.exe    0x341d90        ALLUSERSPROFILE C:\ProgramData
1428    vmtoolsd.exe    0x341d90        APPDATA C:\Windows\system32\config\systemprofile\AppData\Roaming
1428    vmtoolsd.exe    0x341d90        CommonProgramFiles      C:\Program Files\Common Files
1428    vmtoolsd.exe    0x341d90        CommonProgramFiles(x86) C:\Program Files (x86)\Common Files
1428    vmtoolsd.exe    0x341d90        CommonProgramW6432      C:\Program Files\Common Files
1428    vmtoolsd.exe    0x341d90        COMPUTERNAME    WIN-LO6FAF3DTFE
1428    vmtoolsd.exe    0x341d90        ComSpec C:\Windows\system32\cmd.exe
1428    vmtoolsd.exe    0x341d90        FP_NO_HOST_CHECK        NO
1428    vmtoolsd.exe    0x341d90        LOCALAPPDATA    C:\Windows\system32\config\systemprofile\AppData\Local
1428    vmtoolsd.exe    0x341d90        NUMBER_OF_PROCESSORS    2
1428    vmtoolsd.exe    0x341d90        OS      Windows_NT
1428    vmtoolsd.exe    0x341d90        Path    C:\Windows\system32;C:\Windows;C:\Windows\System32\Wbem;C:\Windows\System32\WindowsPowerShell\v1.0\;
1428    vmtoolsd.exe    0x341d90        PATHEXT .COM;.EXE;.BAT;.CMD;.VBS;.VBE;.JS;.JSE;.WSF;.WSH;.MSC
1428    vmtoolsd.exe    0x341d90        PROCESSOR_ARCHITECTURE  AMD64
1428    vmtoolsd.exe    0x341d90        PROCESSOR_IDENTIFIER    Intel64 Family 6 Model 60 Stepping 3, GenuineIntel
1428    vmtoolsd.exe    0x341d90        PROCESSOR_LEVEL 6
1428    vmtoolsd.exe    0x341d90        PROCESSOR_REVISION      3c03
1428    vmtoolsd.exe    0x341d90        ProgramData     C:\ProgramData
1428    vmtoolsd.exe    0x341d90        ProgramFiles    C:\Program Files
1428    vmtoolsd.exe    0x341d90        ProgramFiles(x86)       C:\Program Files (x86)
1428    vmtoolsd.exe    0x341d90        ProgramW6432    C:\Program Files
1428    vmtoolsd.exe    0x341d90        PSModulePath    C:\Windows\system32\WindowsPowerShell\v1.0\Modules\
1428    vmtoolsd.exe    0x341d90        PUBLIC  C:\Users\Public
1428    vmtoolsd.exe    0x341d90        SystemDrive     C:
1428    vmtoolsd.exe    0x341d90        SystemRoot      C:\Windows
1428    vmtoolsd.exe    0x341d90        TEMP    C:\Windows\TEMP
1428    vmtoolsd.exe    0x341d90        TMP     C:\Windows\TEMP
1428    vmtoolsd.exe    0x341d90        USERDOMAIN      WORKGROUP
1428    vmtoolsd.exe    0x341d90        USERNAME        WIN-LO6FAF3DTFE$
1428    vmtoolsd.exe    0x341d90        USERPROFILE     C:\Windows\system32\config\systemprofile
1428    vmtoolsd.exe    0x341d90        windir  C:\Windows
1428    vmtoolsd.exe    0x341d90        windows_tracing_flags   3
1428    vmtoolsd.exe    0x341d90        windows_tracing_logfile C:\BVTBin\Tests\installpackage\csilogfile.log
1800    WmiPrvSE.exe    0x191d90        ALLUSERSPROFILE C:\ProgramData
1800    WmiPrvSE.exe    0x191d90        APPDATA C:\Windows\system32\config\systemprofile\AppData\Roaming
1800    WmiPrvSE.exe    0x191d90        CommonProgramFiles      C:\Program Files\Common Files
1800    WmiPrvSE.exe    0x191d90        CommonProgramFiles(x86) C:\Program Files (x86)\Common Files
1800    WmiPrvSE.exe    0x191d90        CommonProgramW6432      C:\Program Files\Common Files
1800    WmiPrvSE.exe    0x191d90        COMPUTERNAME    WIN-LO6FAF3DTFE
1800    WmiPrvSE.exe    0x191d90        ComSpec C:\Windows\system32\cmd.exe
1800    WmiPrvSE.exe    0x191d90        FP_NO_HOST_CHECK        NO
1800    WmiPrvSE.exe    0x191d90        LOCALAPPDATA    C:\Windows\system32\config\systemprofile\AppData\Local
1800    WmiPrvSE.exe    0x191d90        NUMBER_OF_PROCESSORS    2
1800    WmiPrvSE.exe    0x191d90        OS      Windows_NT
1800    WmiPrvSE.exe    0x191d90        Path    C:\Windows\system32;C:\Windows;C:\Windows\System32\Wbem;C:\Windows\System32\WindowsPowerShell\v1.0\
1800    WmiPrvSE.exe    0x191d90        PATHEXT .COM;.EXE;.BAT;.CMD;.VBS;.VBE;.JS;.JSE;.WSF;.WSH;.MSC
1800    WmiPrvSE.exe    0x191d90        PROCESSOR_ARCHITECTURE  AMD64
1800    WmiPrvSE.exe    0x191d90        PROCESSOR_IDENTIFIER    Intel64 Family 6 Model 60 Stepping 3, GenuineIntel
1800    WmiPrvSE.exe    0x191d90        PROCESSOR_LEVEL 6
1800    WmiPrvSE.exe    0x191d90        PROCESSOR_REVISION      3c03
1800    WmiPrvSE.exe    0x191d90        ProgramData     C:\ProgramData
1800    WmiPrvSE.exe    0x191d90        ProgramFiles    C:\Program Files
1800    WmiPrvSE.exe    0x191d90        ProgramFiles(x86)       C:\Program Files (x86)
1800    WmiPrvSE.exe    0x191d90        ProgramW6432    C:\Program Files
1800    WmiPrvSE.exe    0x191d90        PSModulePath    C:\Windows\system32\WindowsPowerShell\v1.0\Modules\
1800    WmiPrvSE.exe    0x191d90        PUBLIC  C:\Users\Public
1800    WmiPrvSE.exe    0x191d90        SystemDrive     C:
1800    WmiPrvSE.exe    0x191d90        SystemRoot      C:\Windows
1800    WmiPrvSE.exe    0x191d90        TEMP    C:\Windows\TEMP
1800    WmiPrvSE.exe    0x191d90        TMP     C:\Windows\TEMP
1800    WmiPrvSE.exe    0x191d90        USERDOMAIN      WORKGROUP
1800    WmiPrvSE.exe    0x191d90        USERNAME        WIN-LO6FAF3DTFE$
1800    WmiPrvSE.exe    0x191d90        USERPROFILE     C:\Windows\system32\config\systemprofile
1800    WmiPrvSE.exe    0x191d90        windir  C:\Windows
1800    WmiPrvSE.exe    0x191d90        windows_tracing_flags   3
1800    WmiPrvSE.exe    0x191d90        windows_tracing_logfile C:\BVTBin\Tests\installpackage\csilogfile.log
1948    svchost.exe     0x3f1e00        ALLUSERSPROFILE C:\ProgramData
1948    svchost.exe     0x3f1e00        APPDATA C:\Windows\ServiceProfiles\LocalService\AppData\Roaming
1948    svchost.exe     0x3f1e00        CommonProgramFiles      C:\Program Files\Common Files
1948    svchost.exe     0x3f1e00        CommonProgramFiles(x86) C:\Program Files (x86)\Common Files
1948    svchost.exe     0x3f1e00        CommonProgramW6432      C:\Program Files\Common Files
1948    svchost.exe     0x3f1e00        COMPUTERNAME    WIN-LO6FAF3DTFE
1948    svchost.exe     0x3f1e00        ComSpec C:\Windows\system32\cmd.exe
1948    svchost.exe     0x3f1e00        FP_NO_HOST_CHECK        NO
1948    svchost.exe     0x3f1e00        LOCALAPPDATA    C:\Windows\ServiceProfiles\LocalService\AppData\Local
1948    svchost.exe     0x3f1e00        NUMBER_OF_PROCESSORS    2
1948    svchost.exe     0x3f1e00        OS      Windows_NT
1948    svchost.exe     0x3f1e00        Path    C:\Windows\system32;C:\Windows;C:\Windows\System32\Wbem;C:\Windows\System32\WindowsPowerShell\v1.0\
1948    svchost.exe     0x3f1e00        PATHEXT .COM;.EXE;.BAT;.CMD;.VBS;.VBE;.JS;.JSE;.WSF;.WSH;.MSC
1948    svchost.exe     0x3f1e00        PROCESSOR_ARCHITECTURE  AMD64
1948    svchost.exe     0x3f1e00        PROCESSOR_IDENTIFIER    Intel64 Family 6 Model 60 Stepping 3, GenuineIntel
1948    svchost.exe     0x3f1e00        PROCESSOR_LEVEL 6
1948    svchost.exe     0x3f1e00        PROCESSOR_REVISION      3c03
1948    svchost.exe     0x3f1e00        ProgramData     C:\ProgramData
1948    svchost.exe     0x3f1e00        ProgramFiles    C:\Program Files
1948    svchost.exe     0x3f1e00        ProgramFiles(x86)       C:\Program Files (x86)
1948    svchost.exe     0x3f1e00        ProgramW6432    C:\Program Files
1948    svchost.exe     0x3f1e00        PSModulePath    C:\Windows\system32\WindowsPowerShell\v1.0\Modules\
1948    svchost.exe     0x3f1e00        PUBLIC  C:\Users\Public
1948    svchost.exe     0x3f1e00        SystemDrive     C:
1948    svchost.exe     0x3f1e00        SystemRoot      C:\Windows
1948    svchost.exe     0x3f1e00        TEMP    C:\Windows\SERVIC~2\LOCALS~1\AppData\Local\Temp
1948    svchost.exe     0x3f1e00        TMP     C:\Windows\SERVIC~2\LOCALS~1\AppData\Local\Temp
1948    svchost.exe     0x3f1e00        USERDOMAIN      NT AUTHORITY
1948    svchost.exe     0x3f1e00        USERNAME        LOCAL SERVICE
1948    svchost.exe     0x3f1e00        USERPROFILE     C:\Windows\ServiceProfiles\LocalService
1948    svchost.exe     0x3f1e00        windir  C:\Windows
1948    svchost.exe     0x3f1e00        windows_tracing_flags   3
1948    svchost.exe     0x3f1e00        windows_tracing_logfile C:\BVTBin\Tests\installpackage\csilogfile.log
1324    dllhost.exe     0x441d90        ALLUSERSPROFILE C:\ProgramData
1324    dllhost.exe     0x441d90        APPDATA C:\Windows\system32\config\systemprofile\AppData\Roaming
1324    dllhost.exe     0x441d90        CommonProgramFiles      C:\Program Files\Common Files
1324    dllhost.exe     0x441d90        CommonProgramFiles(x86) C:\Program Files (x86)\Common Files
1324    dllhost.exe     0x441d90        CommonProgramW6432      C:\Program Files\Common Files
1324    dllhost.exe     0x441d90        COMPUTERNAME    WIN-LO6FAF3DTFE
1324    dllhost.exe     0x441d90        ComSpec C:\Windows\system32\cmd.exe
1324    dllhost.exe     0x441d90        FP_NO_HOST_CHECK        NO
1324    dllhost.exe     0x441d90        LOCALAPPDATA    C:\Windows\system32\config\systemprofile\AppData\Local
1324    dllhost.exe     0x441d90        NUMBER_OF_PROCESSORS    2
1324    dllhost.exe     0x441d90        OS      Windows_NT
1324    dllhost.exe     0x441d90        Path    C:\Windows\system32;C:\Windows;C:\Windows\System32\Wbem;C:\Windows\System32\WindowsPowerShell\v1.0\
1324    dllhost.exe     0x441d90        PATHEXT .COM;.EXE;.BAT;.CMD;.VBS;.VBE;.JS;.JSE;.WSF;.WSH;.MSC
1324    dllhost.exe     0x441d90        PROCESSOR_ARCHITECTURE  AMD64
1324    dllhost.exe     0x441d90        PROCESSOR_IDENTIFIER    Intel64 Family 6 Model 60 Stepping 3, GenuineIntel
1324    dllhost.exe     0x441d90        PROCESSOR_LEVEL 6
1324    dllhost.exe     0x441d90        PROCESSOR_REVISION      3c03
1324    dllhost.exe     0x441d90        ProgramData     C:\ProgramData
1324    dllhost.exe     0x441d90        ProgramFiles    C:\Program Files
1324    dllhost.exe     0x441d90        ProgramFiles(x86)       C:\Program Files (x86)
1324    dllhost.exe     0x441d90        ProgramW6432    C:\Program Files
1324    dllhost.exe     0x441d90        PSModulePath    C:\Windows\system32\WindowsPowerShell\v1.0\Modules\
1324    dllhost.exe     0x441d90        PUBLIC  C:\Users\Public
1324    dllhost.exe     0x441d90        SystemDrive     C:
1324    dllhost.exe     0x441d90        SystemRoot      C:\Windows
1324    dllhost.exe     0x441d90        TEMP    C:\Windows\TEMP
1324    dllhost.exe     0x441d90        TMP     C:\Windows\TEMP
1324    dllhost.exe     0x441d90        USERDOMAIN      WORKGROUP
1324    dllhost.exe     0x441d90        USERNAME        WIN-LO6FAF3DTFE$
1324    dllhost.exe     0x441d90        USERPROFILE     C:\Windows\system32\config\systemprofile
1324    dllhost.exe     0x441d90        windir  C:\Windows
1324    dllhost.exe     0x441d90        windows_tracing_flags   3
1324    dllhost.exe     0x441d90        windows_tracing_logfile C:\BVTBin\Tests\installpackage\csilogfile.log
1436    msdtc.exe       0x321e10        ALLUSERSPROFILE C:\ProgramData
1436    msdtc.exe       0x321e10        APPDATA C:\Windows\ServiceProfiles\NetworkService\AppData\Roaming
1436    msdtc.exe       0x321e10        CommonProgramFiles      C:\Program Files\Common Files
1436    msdtc.exe       0x321e10        CommonProgramFiles(x86) C:\Program Files (x86)\Common Files
1436    msdtc.exe       0x321e10        CommonProgramW6432      C:\Program Files\Common Files
1436    msdtc.exe       0x321e10        COMPUTERNAME    WIN-LO6FAF3DTFE
1436    msdtc.exe       0x321e10        ComSpec C:\Windows\system32\cmd.exe
1436    msdtc.exe       0x321e10        FP_NO_HOST_CHECK        NO
1436    msdtc.exe       0x321e10        LOCALAPPDATA    C:\Windows\ServiceProfiles\NetworkService\AppData\Local
1436    msdtc.exe       0x321e10        NUMBER_OF_PROCESSORS    2
1436    msdtc.exe       0x321e10        OS      Windows_NT
1436    msdtc.exe       0x321e10        Path    C:\Windows\system32;C:\Windows;C:\Windows\System32\Wbem;C:\Windows\System32\WindowsPowerShell\v1.0\
1436    msdtc.exe       0x321e10        PATHEXT .COM;.EXE;.BAT;.CMD;.VBS;.VBE;.JS;.JSE;.WSF;.WSH;.MSC
1436    msdtc.exe       0x321e10        PROCESSOR_ARCHITECTURE  AMD64
1436    msdtc.exe       0x321e10        PROCESSOR_IDENTIFIER    Intel64 Family 6 Model 60 Stepping 3, GenuineIntel
1436    msdtc.exe       0x321e10        PROCESSOR_LEVEL 6
1436    msdtc.exe       0x321e10        PROCESSOR_REVISION      3c03
1436    msdtc.exe       0x321e10        ProgramData     C:\ProgramData
1436    msdtc.exe       0x321e10        ProgramFiles    C:\Program Files
1436    msdtc.exe       0x321e10        ProgramFiles(x86)       C:\Program Files (x86)
1436    msdtc.exe       0x321e10        ProgramW6432    C:\Program Files
1436    msdtc.exe       0x321e10        PSModulePath    C:\Windows\system32\WindowsPowerShell\v1.0\Modules\
1436    msdtc.exe       0x321e10        PUBLIC  C:\Users\Public
1436    msdtc.exe       0x321e10        SystemDrive     C:
1436    msdtc.exe       0x321e10        SystemRoot      C:\Windows
1436    msdtc.exe       0x321e10        TEMP    C:\Windows\SERVIC~2\NETWOR~1\AppData\Local\Temp
1436    msdtc.exe       0x321e10        TMP     C:\Windows\SERVIC~2\NETWOR~1\AppData\Local\Temp
1436    msdtc.exe       0x321e10        USERDOMAIN      WORKGROUP
1436    msdtc.exe       0x321e10        USERNAME        WIN-LO6FAF3DTFE$
1436    msdtc.exe       0x321e10        USERPROFILE     C:\Windows\ServiceProfiles\NetworkService
1436    msdtc.exe       0x321e10        windir  C:\Windows
1436    msdtc.exe       0x321e10        windows_tracing_flags   3
1436    msdtc.exe       0x321e10        windows_tracing_logfile C:\BVTBin\Tests\installpackage\csilogfile.log
2136    WmiPrvSE.exe    0x1e1d90        ALLUSERSPROFILE C:\ProgramData
2136    WmiPrvSE.exe    0x1e1d90        APPDATA C:\Windows\system32\config\systemprofile\AppData\Roaming
2136    WmiPrvSE.exe    0x1e1d90        CommonProgramFiles      C:\Program Files\Common Files
2136    WmiPrvSE.exe    0x1e1d90        CommonProgramFiles(x86) C:\Program Files (x86)\Common Files
2136    WmiPrvSE.exe    0x1e1d90        CommonProgramW6432      C:\Program Files\Common Files
2136    WmiPrvSE.exe    0x1e1d90        COMPUTERNAME    WIN-LO6FAF3DTFE
2136    WmiPrvSE.exe    0x1e1d90        ComSpec C:\Windows\system32\cmd.exe
2136    WmiPrvSE.exe    0x1e1d90        FP_NO_HOST_CHECK        NO
2136    WmiPrvSE.exe    0x1e1d90        LOCALAPPDATA    C:\Windows\system32\config\systemprofile\AppData\Local
2136    WmiPrvSE.exe    0x1e1d90        NUMBER_OF_PROCESSORS    2
2136    WmiPrvSE.exe    0x1e1d90        OS      Windows_NT
2136    WmiPrvSE.exe    0x1e1d90        Path    C:\Windows\system32;C:\Windows;C:\Windows\System32\Wbem;C:\Windows\System32\WindowsPowerShell\v1.0\
2136    WmiPrvSE.exe    0x1e1d90        PATHEXT .COM;.EXE;.BAT;.CMD;.VBS;.VBE;.JS;.JSE;.WSF;.WSH;.MSC
2136    WmiPrvSE.exe    0x1e1d90        PROCESSOR_ARCHITECTURE  AMD64
2136    WmiPrvSE.exe    0x1e1d90        PROCESSOR_IDENTIFIER    Intel64 Family 6 Model 60 Stepping 3, GenuineIntel
2136    WmiPrvSE.exe    0x1e1d90        PROCESSOR_LEVEL 6
2136    WmiPrvSE.exe    0x1e1d90        PROCESSOR_REVISION      3c03
2136    WmiPrvSE.exe    0x1e1d90        ProgramData     C:\ProgramData
2136    WmiPrvSE.exe    0x1e1d90        ProgramFiles    C:\Program Files
2136    WmiPrvSE.exe    0x1e1d90        ProgramFiles(x86)       C:\Program Files (x86)
2136    WmiPrvSE.exe    0x1e1d90        ProgramW6432    C:\Program Files
2136    WmiPrvSE.exe    0x1e1d90        PSModulePath    C:\Windows\system32\WindowsPowerShell\v1.0\Modules\
2136    WmiPrvSE.exe    0x1e1d90        PUBLIC  C:\Users\Public
2136    WmiPrvSE.exe    0x1e1d90        SystemDrive     C:
2136    WmiPrvSE.exe    0x1e1d90        SystemRoot      C:\Windows
2136    WmiPrvSE.exe    0x1e1d90        TEMP    C:\Windows\TEMP
2136    WmiPrvSE.exe    0x1e1d90        TMP     C:\Windows\TEMP
2136    WmiPrvSE.exe    0x1e1d90        USERDOMAIN      WORKGROUP
2136    WmiPrvSE.exe    0x1e1d90        USERNAME        WIN-LO6FAF3DTFE$
2136    WmiPrvSE.exe    0x1e1d90        USERPROFILE     C:\Windows\system32\config\systemprofile
2136    WmiPrvSE.exe    0x1e1d90        windir  C:\Windows
2136    WmiPrvSE.exe    0x1e1d90        windows_tracing_flags   3
2136    WmiPrvSE.exe    0x1e1d90        windows_tracing_logfile C:\BVTBin\Tests\installpackage\csilogfile.log
2344    taskhost.exe    0x201da0        ALLUSERSPROFILE C:\ProgramData
2344    taskhost.exe    0x201da0        APPDATA C:\Users\Rick\AppData\Roaming
2344    taskhost.exe    0x201da0        CommonProgramFiles      C:\Program Files\Common Files
2344    taskhost.exe    0x201da0        CommonProgramFiles(x86) C:\Program Files (x86)\Common Files
2344    taskhost.exe    0x201da0        CommonProgramW6432      C:\Program Files\Common Files
2344    taskhost.exe    0x201da0        COMPUTERNAME    WIN-LO6FAF3DTFE
2344    taskhost.exe    0x201da0        ComSpec C:\Windows\system32\cmd.exe
2344    taskhost.exe    0x201da0        FP_NO_HOST_CHECK        NO
2344    taskhost.exe    0x201da0        HOMEDRIVE       C:
2344    taskhost.exe    0x201da0        HOMEPATH        \Users\Rick
2344    taskhost.exe    0x201da0        LOCALAPPDATA    C:\Users\Rick\AppData\Local
2344    taskhost.exe    0x201da0        LOGONSERVER     \\WIN-LO6FAF3DTFE
2344    taskhost.exe    0x201da0        NUMBER_OF_PROCESSORS    2
2344    taskhost.exe    0x201da0        OS      Windows_NT
2344    taskhost.exe    0x201da0        Path    C:\Windows\system32;C:\Windows;C:\Windows\System32\Wbem;C:\Windows\System32\WindowsPowerShell\v1.0\
2344    taskhost.exe    0x201da0        PATHEXT .COM;.EXE;.BAT;.CMD;.VBS;.VBE;.JS;.JSE;.WSF;.WSH;.MSC
2344    taskhost.exe    0x201da0        PROCESSOR_ARCHITECTURE  AMD64
2344    taskhost.exe    0x201da0        PROCESSOR_IDENTIFIER    Intel64 Family 6 Model 60 Stepping 3, GenuineIntel
2344    taskhost.exe    0x201da0        PROCESSOR_LEVEL 6
2344    taskhost.exe    0x201da0        PROCESSOR_REVISION      3c03
2344    taskhost.exe    0x201da0        ProgramData     C:\ProgramData
2344    taskhost.exe    0x201da0        ProgramFiles    C:\Program Files
2344    taskhost.exe    0x201da0        ProgramFiles(x86)       C:\Program Files (x86)
2344    taskhost.exe    0x201da0        ProgramW6432    C:\Program Files
2344    taskhost.exe    0x201da0        PSModulePath    C:\Windows\system32\WindowsPowerShell\v1.0\Modules\
2344    taskhost.exe    0x201da0        PUBLIC  C:\Users\Public
2344    taskhost.exe    0x201da0        SystemDrive     C:
2344    taskhost.exe    0x201da0        SystemRoot      C:\Windows
2344    taskhost.exe    0x201da0        TEMP    C:\Users\Rick\AppData\Local\Temp
2344    taskhost.exe    0x201da0        TMP     C:\Users\Rick\AppData\Local\Temp
2344    taskhost.exe    0x201da0        USERDOMAIN      WIN-LO6FAF3DTFE
2344    taskhost.exe    0x201da0        USERNAME        Rick
2344    taskhost.exe    0x201da0        USERPROFILE     C:\Users\Rick
2344    taskhost.exe    0x201da0        windir  C:\Windows
2344    taskhost.exe    0x201da0        windows_tracing_flags   3
2344    taskhost.exe    0x201da0        windows_tracing_logfile C:\BVTBin\Tests\installpackage\csilogfile.log
2500    sppsvc.exe      0x341e10        ALLUSERSPROFILE C:\ProgramData
2500    sppsvc.exe      0x341e10        APPDATA C:\Windows\ServiceProfiles\NetworkService\AppData\Roaming
2500    sppsvc.exe      0x341e10        CommonProgramFiles      C:\Program Files\Common Files
2500    sppsvc.exe      0x341e10        CommonProgramFiles(x86) C:\Program Files (x86)\Common Files
2500    sppsvc.exe      0x341e10        CommonProgramW6432      C:\Program Files\Common Files
2500    sppsvc.exe      0x341e10        COMPUTERNAME    WIN-LO6FAF3DTFE
2500    sppsvc.exe      0x341e10        ComSpec C:\Windows\system32\cmd.exe
2500    sppsvc.exe      0x341e10        FP_NO_HOST_CHECK        NO
2500    sppsvc.exe      0x341e10        LOCALAPPDATA    C:\Windows\ServiceProfiles\NetworkService\AppData\Local
2500    sppsvc.exe      0x341e10        NUMBER_OF_PROCESSORS    2
2500    sppsvc.exe      0x341e10        OS      Windows_NT
2500    sppsvc.exe      0x341e10        Path    C:\Windows\system32;C:\Windows;C:\Windows\System32\Wbem;C:\Windows\System32\WindowsPowerShell\v1.0\
2500    sppsvc.exe      0x341e10        PATHEXT .COM;.EXE;.BAT;.CMD;.VBS;.VBE;.JS;.JSE;.WSF;.WSH;.MSC
2500    sppsvc.exe      0x341e10        PROCESSOR_ARCHITECTURE  AMD64
2500    sppsvc.exe      0x341e10        PROCESSOR_IDENTIFIER    Intel64 Family 6 Model 60 Stepping 3, GenuineIntel
2500    sppsvc.exe      0x341e10        PROCESSOR_LEVEL 6
2500    sppsvc.exe      0x341e10        PROCESSOR_REVISION      3c03
2500    sppsvc.exe      0x341e10        ProgramData     C:\ProgramData
2500    sppsvc.exe      0x341e10        ProgramFiles    C:\Program Files
2500    sppsvc.exe      0x341e10        ProgramFiles(x86)       C:\Program Files (x86)
2500    sppsvc.exe      0x341e10        ProgramW6432    C:\Program Files
2500    sppsvc.exe      0x341e10        PSModulePath    C:\Windows\system32\WindowsPowerShell\v1.0\Modules\
2500    sppsvc.exe      0x341e10        PUBLIC  C:\Users\Public
2500    sppsvc.exe      0x341e10        SystemDrive     C:
2500    sppsvc.exe      0x341e10        SystemRoot      C:\Windows
2500    sppsvc.exe      0x341e10        TEMP    C:\Windows\SERVIC~2\NETWOR~1\AppData\Local\Temp
2500    sppsvc.exe      0x341e10        TMP     C:\Windows\SERVIC~2\NETWOR~1\AppData\Local\Temp
2500    sppsvc.exe      0x341e10        USERDOMAIN      WORKGROUP
2500    sppsvc.exe      0x341e10        USERNAME        WIN-LO6FAF3DTFE$
2500    sppsvc.exe      0x341e10        USERPROFILE     C:\Windows\ServiceProfiles\NetworkService
2500    sppsvc.exe      0x341e10        windir  C:\Windows
2500    sppsvc.exe      0x341e10        windows_tracing_flags   3
2500    sppsvc.exe      0x341e10        windows_tracing_logfile C:\BVTBin\Tests\installpackage\csilogfile.log
2704    dwm.exe 0x1c1da0        ALLUSERSPROFILE C:\ProgramData
2704    dwm.exe 0x1c1da0        APPDATA C:\Users\Rick\AppData\Roaming
2704    dwm.exe 0x1c1da0        CommonProgramFiles      C:\Program Files\Common Files
2704    dwm.exe 0x1c1da0        CommonProgramFiles(x86) C:\Program Files (x86)\Common Files
2704    dwm.exe 0x1c1da0        CommonProgramW6432      C:\Program Files\Common Files
2704    dwm.exe 0x1c1da0        COMPUTERNAME    WIN-LO6FAF3DTFE
2704    dwm.exe 0x1c1da0        ComSpec C:\Windows\system32\cmd.exe
2704    dwm.exe 0x1c1da0        FP_NO_HOST_CHECK        NO
2704    dwm.exe 0x1c1da0        HOMEDRIVE       C:
2704    dwm.exe 0x1c1da0        HOMEPATH        \Users\Rick
2704    dwm.exe 0x1c1da0        LOCALAPPDATA    C:\Users\Rick\AppData\Local
2704    dwm.exe 0x1c1da0        LOGONSERVER     \\WIN-LO6FAF3DTFE
2704    dwm.exe 0x1c1da0        NUMBER_OF_PROCESSORS    2
2704    dwm.exe 0x1c1da0        OS      Windows_NT
2704    dwm.exe 0x1c1da0        Path    C:\Windows\system32;C:\Windows;C:\Windows\System32\Wbem;C:\Windows\System32\WindowsPowerShell\v1.0\
2704    dwm.exe 0x1c1da0        PATHEXT .COM;.EXE;.BAT;.CMD;.VBS;.VBE;.JS;.JSE;.WSF;.WSH;.MSC
2704    dwm.exe 0x1c1da0        PROCESSOR_ARCHITECTURE  AMD64
2704    dwm.exe 0x1c1da0        PROCESSOR_IDENTIFIER    Intel64 Family 6 Model 60 Stepping 3, GenuineIntel
2704    dwm.exe 0x1c1da0        PROCESSOR_LEVEL 6
2704    dwm.exe 0x1c1da0        PROCESSOR_REVISION      3c03
2704    dwm.exe 0x1c1da0        ProgramData     C:\ProgramData
2704    dwm.exe 0x1c1da0        ProgramFiles    C:\Program Files
2704    dwm.exe 0x1c1da0        ProgramFiles(x86)       C:\Program Files (x86)
2704    dwm.exe 0x1c1da0        ProgramW6432    C:\Program Files
2704    dwm.exe 0x1c1da0        PSModulePath    C:\Windows\system32\WindowsPowerShell\v1.0\Modules\
2704    dwm.exe 0x1c1da0        PUBLIC  C:\Users\Public
2704    dwm.exe 0x1c1da0        SystemDrive     C:
2704    dwm.exe 0x1c1da0        SystemRoot      C:\Windows
2704    dwm.exe 0x1c1da0        TEMP    C:\Users\Rick\AppData\Local\Temp
2704    dwm.exe 0x1c1da0        TMP     C:\Users\Rick\AppData\Local\Temp
2704    dwm.exe 0x1c1da0        USERDOMAIN      WIN-LO6FAF3DTFE
2704    dwm.exe 0x1c1da0        USERNAME        Rick
2704    dwm.exe 0x1c1da0        USERPROFILE     C:\Users\Rick
2704    dwm.exe 0x1c1da0        windir  C:\Windows
2704    dwm.exe 0x1c1da0        windows_tracing_flags   3
2704    dwm.exe 0x1c1da0        windows_tracing_logfile C:\BVTBin\Tests\installpackage\csilogfile.log
2728    explorer.exe    0x391dc0        ALLUSERSPROFILE C:\ProgramData
2728    explorer.exe    0x391dc0        APPDATA C:\Users\Rick\AppData\Roaming
2728    explorer.exe    0x391dc0        CommonProgramFiles      C:\Program Files\Common Files
2728    explorer.exe    0x391dc0        CommonProgramFiles(x86) C:\Program Files (x86)\Common Files
2728    explorer.exe    0x391dc0        CommonProgramW6432      C:\Program Files\Common Files
2728    explorer.exe    0x391dc0        COMPUTERNAME    WIN-LO6FAF3DTFE
2728    explorer.exe    0x391dc0        ComSpec C:\Windows\system32\cmd.exe
2728    explorer.exe    0x391dc0        FP_NO_HOST_CHECK        NO
2728    explorer.exe    0x391dc0        HOMEDRIVE       C:
2728    explorer.exe    0x391dc0        HOMEPATH        \Users\Rick
2728    explorer.exe    0x391dc0        LOCALAPPDATA    C:\Users\Rick\AppData\Local
2728    explorer.exe    0x391dc0        LOGONSERVER     \\WIN-LO6FAF3DTFE
2728    explorer.exe    0x391dc0        NUMBER_OF_PROCESSORS    2
2728    explorer.exe    0x391dc0        OS      Windows_NT
2728    explorer.exe    0x391dc0        Path    C:\Windows\system32;C:\Windows;C:\Windows\System32\Wbem;C:\Windows\System32\WindowsPowerShell\v1.0\
2728    explorer.exe    0x391dc0        PATHEXT .COM;.EXE;.BAT;.CMD;.VBS;.VBE;.JS;.JSE;.WSF;.WSH;.MSC
2728    explorer.exe    0x391dc0        PROCESSOR_ARCHITECTURE  AMD64
2728    explorer.exe    0x391dc0        PROCESSOR_IDENTIFIER    Intel64 Family 6 Model 60 Stepping 3, GenuineIntel
2728    explorer.exe    0x391dc0        PROCESSOR_LEVEL 6
2728    explorer.exe    0x391dc0        PROCESSOR_REVISION      3c03
2728    explorer.exe    0x391dc0        ProgramData     C:\ProgramData
2728    explorer.exe    0x391dc0        ProgramFiles    C:\Program Files
2728    explorer.exe    0x391dc0        ProgramFiles(x86)       C:\Program Files (x86)
2728    explorer.exe    0x391dc0        ProgramW6432    C:\Program Files
2728    explorer.exe    0x391dc0        PSModulePath    C:\Windows\system32\WindowsPowerShell\v1.0\Modules\
2728    explorer.exe    0x391dc0        PUBLIC  C:\Users\Public
2728    explorer.exe    0x391dc0        SESSIONNAME     Console
2728    explorer.exe    0x391dc0        SystemDrive     C:
2728    explorer.exe    0x391dc0        SystemRoot      C:\Windows
2728    explorer.exe    0x391dc0        TEMP    C:\Users\Rick\AppData\Local\Temp
2728    explorer.exe    0x391dc0        TMP     C:\Users\Rick\AppData\Local\Temp
2728    explorer.exe    0x391dc0        USERDOMAIN      WIN-LO6FAF3DTFE
2728    explorer.exe    0x391dc0        USERNAME        Rick
2728    explorer.exe    0x391dc0        USERPROFILE     C:\Users\Rick
2728    explorer.exe    0x391dc0        windir  C:\Windows
2728    explorer.exe    0x391dc0        windows_tracing_flags   3
2728    explorer.exe    0x391dc0        windows_tracing_logfile C:\BVTBin\Tests\installpackage\csilogfile.log
2804    vmtoolsd.exe    0x341dd0        ALLUSERSPROFILE C:\ProgramData
2804    vmtoolsd.exe    0x341dd0        APPDATA C:\Users\Rick\AppData\Roaming
2804    vmtoolsd.exe    0x341dd0        CommonProgramFiles      C:\Program Files\Common Files
2804    vmtoolsd.exe    0x341dd0        CommonProgramFiles(x86) C:\Program Files (x86)\Common Files
2804    vmtoolsd.exe    0x341dd0        CommonProgramW6432      C:\Program Files\Common Files
2804    vmtoolsd.exe    0x341dd0        COMPUTERNAME    WIN-LO6FAF3DTFE
2804    vmtoolsd.exe    0x341dd0        ComSpec C:\Windows\system32\cmd.exe
2804    vmtoolsd.exe    0x341dd0        FP_NO_HOST_CHECK        NO
2804    vmtoolsd.exe    0x341dd0        HOMEDRIVE       C:
2804    vmtoolsd.exe    0x341dd0        HOMEPATH        \Users\Rick
2804    vmtoolsd.exe    0x341dd0        LOCALAPPDATA    C:\Users\Rick\AppData\Local
2804    vmtoolsd.exe    0x341dd0        LOGONSERVER     \\WIN-LO6FAF3DTFE
2804    vmtoolsd.exe    0x341dd0        NUMBER_OF_PROCESSORS    2
2804    vmtoolsd.exe    0x341dd0        OS      Windows_NT
2804    vmtoolsd.exe    0x341dd0        Path    C:\Windows\system32;C:\Windows;C:\Windows\System32\Wbem;C:\Windows\System32\WindowsPowerShell\v1.0\
2804    vmtoolsd.exe    0x341dd0        PATHEXT .COM;.EXE;.BAT;.CMD;.VBS;.VBE;.JS;.JSE;.WSF;.WSH;.MSC
2804    vmtoolsd.exe    0x341dd0        PROCESSOR_ARCHITECTURE  AMD64
2804    vmtoolsd.exe    0x341dd0        PROCESSOR_IDENTIFIER    Intel64 Family 6 Model 60 Stepping 3, GenuineIntel
2804    vmtoolsd.exe    0x341dd0        PROCESSOR_LEVEL 6
2804    vmtoolsd.exe    0x341dd0        PROCESSOR_REVISION      3c03
2804    vmtoolsd.exe    0x341dd0        ProgramData     C:\ProgramData
2804    vmtoolsd.exe    0x341dd0        ProgramFiles    C:\Program Files
2804    vmtoolsd.exe    0x341dd0        ProgramFiles(x86)       C:\Program Files (x86)
2804    vmtoolsd.exe    0x341dd0        ProgramW6432    C:\Program Files
2804    vmtoolsd.exe    0x341dd0        PSModulePath    C:\Windows\system32\WindowsPowerShell\v1.0\Modules\
2804    vmtoolsd.exe    0x341dd0        PUBLIC  C:\Users\Public
2804    vmtoolsd.exe    0x341dd0        SESSIONNAME     Console
2804    vmtoolsd.exe    0x341dd0        SystemDrive     C:
2804    vmtoolsd.exe    0x341dd0        SystemRoot      C:\Windows
2804    vmtoolsd.exe    0x341dd0        TEMP    C:\Users\Rick\AppData\Local\Temp
2804    vmtoolsd.exe    0x341dd0        TMP     C:\Users\Rick\AppData\Local\Temp
2804    vmtoolsd.exe    0x341dd0        USERDOMAIN      WIN-LO6FAF3DTFE
2804    vmtoolsd.exe    0x341dd0        USERNAME        Rick
2804    vmtoolsd.exe    0x341dd0        USERPROFILE     C:\Users\Rick
2804    vmtoolsd.exe    0x341dd0        windir  C:\Windows
2804    vmtoolsd.exe    0x341dd0        windows_tracing_flags   3
2804    vmtoolsd.exe    0x341dd0        windows_tracing_logfile C:\BVTBin\Tests\installpackage\csilogfile.log
2836    BitTorrent.exe  0x1f1dd0        ALLUSERSPROFILE C:\ProgramData
2836    BitTorrent.exe  0x1f1dd0        APPDATA C:\Users\Rick\AppData\Roaming
2836    BitTorrent.exe  0x1f1dd0        CommonProgramFiles      C:\Program Files\Common Files
2836    BitTorrent.exe  0x1f1dd0        CommonProgramFiles(x86) C:\Program Files (x86)\Common Files
2836    BitTorrent.exe  0x1f1dd0        CommonProgramW6432      C:\Program Files\Common Files
2836    BitTorrent.exe  0x1f1dd0        COMPUTERNAME    WIN-LO6FAF3DTFE
2836    BitTorrent.exe  0x1f1dd0        ComSpec C:\Windows\system32\cmd.exe
2836    BitTorrent.exe  0x1f1dd0        FP_NO_HOST_CHECK        NO
2836    BitTorrent.exe  0x1f1dd0        HOMEDRIVE       C:
2836    BitTorrent.exe  0x1f1dd0        HOMEPATH        \Users\Rick
2836    BitTorrent.exe  0x1f1dd0        LOCALAPPDATA    C:\Users\Rick\AppData\Local
2836    BitTorrent.exe  0x1f1dd0        LOGONSERVER     \\WIN-LO6FAF3DTFE
2836    BitTorrent.exe  0x1f1dd0        NUMBER_OF_PROCESSORS    2
2836    BitTorrent.exe  0x1f1dd0        OS      Windows_NT
2836    BitTorrent.exe  0x1f1dd0        Path    C:\Windows\system32;C:\Windows;C:\Windows\System32\Wbem;C:\Windows\System32\WindowsPowerShell\v1.0\
2836    BitTorrent.exe  0x1f1dd0        PATHEXT .COM;.EXE;.BAT;.CMD;.VBS;.VBE;.JS;.JSE;.WSF;.WSH;.MSC
2836    BitTorrent.exe  0x1f1dd0        PROCESSOR_ARCHITECTURE  AMD64
2836    BitTorrent.exe  0x1f1dd0        PROCESSOR_IDENTIFIER    Intel64 Family 6 Model 60 Stepping 3, GenuineIntel
2836    BitTorrent.exe  0x1f1dd0        PROCESSOR_LEVEL 6
2836    BitTorrent.exe  0x1f1dd0        PROCESSOR_REVISION      3c03
2836    BitTorrent.exe  0x1f1dd0        ProgramData     C:\ProgramData
2836    BitTorrent.exe  0x1f1dd0        ProgramFiles    C:\Program Files
2836    BitTorrent.exe  0x1f1dd0        ProgramFiles(x86)       C:\Program Files (x86)
2836    BitTorrent.exe  0x1f1dd0        ProgramW6432    C:\Program Files
2836    BitTorrent.exe  0x1f1dd0        PSModulePath    C:\Windows\system32\WindowsPowerShell\v1.0\Modules\
2836    BitTorrent.exe  0x1f1dd0        PUBLIC  C:\Users\Public
2836    BitTorrent.exe  0x1f1dd0        SESSIONNAME     Console
2836    BitTorrent.exe  0x1f1dd0        SystemDrive     C:
2836    BitTorrent.exe  0x1f1dd0        SystemRoot      C:\Windows
2836    BitTorrent.exe  0x1f1dd0        TEMP    C:\Users\Rick\AppData\Local\Temp
2836    BitTorrent.exe  0x1f1dd0        TMP     C:\Users\Rick\AppData\Local\Temp
2836    BitTorrent.exe  0x1f1dd0        USERDOMAIN      WIN-LO6FAF3DTFE
2836    BitTorrent.exe  0x1f1dd0        USERNAME        Rick
2836    BitTorrent.exe  0x1f1dd0        USERPROFILE     C:\Users\Rick
2836    BitTorrent.exe  0x1f1dd0        windir  C:\Windows
2836    BitTorrent.exe  0x1f1dd0        windows_tracing_flags   3
2836    BitTorrent.exe  0x1f1dd0        windows_tracing_logfile C:\BVTBin\Tests\installpackage\csilogfile.log
3064    SearchIndexer.  0x161d90        ALLUSERSPROFILE C:\ProgramData
3064    SearchIndexer.  0x161d90        APPDATA C:\Windows\system32\config\systemprofile\AppData\Roaming
3064    SearchIndexer.  0x161d90        CommonProgramFiles      C:\Program Files\Common Files
3064    SearchIndexer.  0x161d90        CommonProgramFiles(x86) C:\Program Files (x86)\Common Files
3064    SearchIndexer.  0x161d90        CommonProgramW6432      C:\Program Files\Common Files
3064    SearchIndexer.  0x161d90        COMPUTERNAME    WIN-LO6FAF3DTFE
3064    SearchIndexer.  0x161d90        ComSpec C:\Windows\system32\cmd.exe
3064    SearchIndexer.  0x161d90        FP_NO_HOST_CHECK        NO
3064    SearchIndexer.  0x161d90        LOCALAPPDATA    C:\Windows\system32\config\systemprofile\AppData\Local
3064    SearchIndexer.  0x161d90        NUMBER_OF_PROCESSORS    2
3064    SearchIndexer.  0x161d90        OS      Windows_NT
3064    SearchIndexer.  0x161d90        Path    C:\Windows\system32;C:\Windows;C:\Windows\System32\Wbem;C:\Windows\System32\WindowsPowerShell\v1.0\;C:\Windows\system32
3064    SearchIndexer.  0x161d90        PATHEXT .COM;.EXE;.BAT;.CMD;.VBS;.VBE;.JS;.JSE;.WSF;.WSH;.MSC
3064    SearchIndexer.  0x161d90        PROCESSOR_ARCHITECTURE  AMD64
3064    SearchIndexer.  0x161d90        PROCESSOR_IDENTIFIER    Intel64 Family 6 Model 60 Stepping 3, GenuineIntel
3064    SearchIndexer.  0x161d90        PROCESSOR_LEVEL 6
3064    SearchIndexer.  0x161d90        PROCESSOR_REVISION      3c03
3064    SearchIndexer.  0x161d90        ProgramData     C:\ProgramData
3064    SearchIndexer.  0x161d90        ProgramFiles    C:\Program Files
3064    SearchIndexer.  0x161d90        ProgramFiles(x86)       C:\Program Files (x86)
3064    SearchIndexer.  0x161d90        ProgramW6432    C:\Program Files
3064    SearchIndexer.  0x161d90        PSModulePath    C:\Windows\system32\WindowsPowerShell\v1.0\Modules\
3064    SearchIndexer.  0x161d90        PUBLIC  C:\Users\Public
3064    SearchIndexer.  0x161d90        SystemDrive     C:
3064    SearchIndexer.  0x161d90        SystemRoot      C:\Windows
3064    SearchIndexer.  0x161d90        TEMP    C:\ProgramData\Microsoft\Search\Data\Temp\usgthrsvc
3064    SearchIndexer.  0x161d90        TMP     C:\ProgramData\Microsoft\Search\Data\Temp\usgthrsvc
3064    SearchIndexer.  0x161d90        USERDOMAIN      WORKGROUP
3064    SearchIndexer.  0x161d90        USERNAME        WIN-LO6FAF3DTFE$
3064    SearchIndexer.  0x161d90        USERPROFILE     C:\Windows\system32\config\systemprofile
3064    SearchIndexer.  0x161d90        windir  C:\Windows
3064    SearchIndexer.  0x161d90        windows_tracing_flags   3
3064    SearchIndexer.  0x161d90        windows_tracing_logfile C:\BVTBin\Tests\installpackage\csilogfile.log
2308    bittorrentie.e  0x321e20        ALLUSERSPROFILE C:\ProgramData
2308    bittorrentie.e  0x321e20        APPDATA C:\Users\Rick\AppData\Roaming
2308    bittorrentie.e  0x321e20        CommonProgramFiles      C:\Program Files\Common Files
2308    bittorrentie.e  0x321e20        CommonProgramFiles(x86) C:\Program Files (x86)\Common Files
2308    bittorrentie.e  0x321e20        CommonProgramW6432      C:\Program Files\Common Files
2308    bittorrentie.e  0x321e20        COMPUTERNAME    WIN-LO6FAF3DTFE
2308    bittorrentie.e  0x321e20        ComSpec C:\Windows\system32\cmd.exe
2308    bittorrentie.e  0x321e20        FP_NO_HOST_CHECK        NO
2308    bittorrentie.e  0x321e20        HOMEDRIVE       C:
2308    bittorrentie.e  0x321e20        HOMEPATH        \Users\Rick
2308    bittorrentie.e  0x321e20        LOCALAPPDATA    C:\Users\Rick\AppData\Local
2308    bittorrentie.e  0x321e20        LOGONSERVER     \\WIN-LO6FAF3DTFE
2308    bittorrentie.e  0x321e20        NUMBER_OF_PROCESSORS    2
2308    bittorrentie.e  0x321e20        OS      Windows_NT
2308    bittorrentie.e  0x321e20        Path    C:\Windows\system32;C:\Windows;C:\Windows\System32\Wbem;C:\Windows\System32\WindowsPowerShell\v1.0\
2308    bittorrentie.e  0x321e20        PATHEXT .COM;.EXE;.BAT;.CMD;.VBS;.VBE;.JS;.JSE;.WSF;.WSH;.MSC
2308    bittorrentie.e  0x321e20        PROCESSOR_ARCHITECTURE  AMD64
2308    bittorrentie.e  0x321e20        PROCESSOR_IDENTIFIER    Intel64 Family 6 Model 60 Stepping 3, GenuineIntel
2308    bittorrentie.e  0x321e20        PROCESSOR_LEVEL 6
2308    bittorrentie.e  0x321e20        PROCESSOR_REVISION      3c03
2308    bittorrentie.e  0x321e20        ProgramData     C:\ProgramData
2308    bittorrentie.e  0x321e20        ProgramFiles    C:\Program Files
2308    bittorrentie.e  0x321e20        ProgramFiles(x86)       C:\Program Files (x86)
2308    bittorrentie.e  0x321e20        ProgramW6432    C:\Program Files
2308    bittorrentie.e  0x321e20        PSModulePath    C:\Windows\system32\WindowsPowerShell\v1.0\Modules\
2308    bittorrentie.e  0x321e20        PUBLIC  C:\Users\Public
2308    bittorrentie.e  0x321e20        SESSIONNAME     Console
2308    bittorrentie.e  0x321e20        SystemDrive     C:
2308    bittorrentie.e  0x321e20        SystemRoot      C:\Windows
2308    bittorrentie.e  0x321e20        TEMP    C:\Users\Rick\AppData\Local\Temp
2308    bittorrentie.e  0x321e20        TMP     C:\Users\Rick\AppData\Local\Temp
2308    bittorrentie.e  0x321e20        USERDOMAIN      WIN-LO6FAF3DTFE
2308    bittorrentie.e  0x321e20        USERNAME        Rick
2308    bittorrentie.e  0x321e20        USERPROFILE     C:\Users\Rick
2308    bittorrentie.e  0x321e20        windir  C:\Windows
2308    bittorrentie.e  0x321e20        windows_tracing_flags   3
2308    bittorrentie.e  0x321e20        windows_tracing_logfile C:\BVTBin\Tests\installpackage\csilogfile.log
2624    bittorrentie.e  0x531e20        ALLUSERSPROFILE C:\ProgramData
2624    bittorrentie.e  0x531e20        APPDATA C:\Users\Rick\AppData\Roaming
2624    bittorrentie.e  0x531e20        CommonProgramFiles      C:\Program Files\Common Files
2624    bittorrentie.e  0x531e20        CommonProgramFiles(x86) C:\Program Files (x86)\Common Files
2624    bittorrentie.e  0x531e20        CommonProgramW6432      C:\Program Files\Common Files
2624    bittorrentie.e  0x531e20        COMPUTERNAME    WIN-LO6FAF3DTFE
2624    bittorrentie.e  0x531e20        ComSpec C:\Windows\system32\cmd.exe
2624    bittorrentie.e  0x531e20        FP_NO_HOST_CHECK        NO
2624    bittorrentie.e  0x531e20        HOMEDRIVE       C:
2624    bittorrentie.e  0x531e20        HOMEPATH        \Users\Rick
2624    bittorrentie.e  0x531e20        LOCALAPPDATA    C:\Users\Rick\AppData\Local
2624    bittorrentie.e  0x531e20        LOGONSERVER     \\WIN-LO6FAF3DTFE
2624    bittorrentie.e  0x531e20        NUMBER_OF_PROCESSORS    2
2624    bittorrentie.e  0x531e20        OS      Windows_NT
2624    bittorrentie.e  0x531e20        Path    C:\Windows\system32;C:\Windows;C:\Windows\System32\Wbem;C:\Windows\System32\WindowsPowerShell\v1.0\
2624    bittorrentie.e  0x531e20        PATHEXT .COM;.EXE;.BAT;.CMD;.VBS;.VBE;.JS;.JSE;.WSF;.WSH;.MSC
2624    bittorrentie.e  0x531e20        PROCESSOR_ARCHITECTURE  AMD64
2624    bittorrentie.e  0x531e20        PROCESSOR_IDENTIFIER    Intel64 Family 6 Model 60 Stepping 3, GenuineIntel
2624    bittorrentie.e  0x531e20        PROCESSOR_LEVEL 6
2624    bittorrentie.e  0x531e20        PROCESSOR_REVISION      3c03
2624    bittorrentie.e  0x531e20        ProgramData     C:\ProgramData
2624    bittorrentie.e  0x531e20        ProgramFiles    C:\Program Files
2624    bittorrentie.e  0x531e20        ProgramFiles(x86)       C:\Program Files (x86)
2624    bittorrentie.e  0x531e20        ProgramW6432    C:\Program Files
2624    bittorrentie.e  0x531e20        PSModulePath    C:\Windows\system32\WindowsPowerShell\v1.0\Modules\
2624    bittorrentie.e  0x531e20        PUBLIC  C:\Users\Public
2624    bittorrentie.e  0x531e20        SESSIONNAME     Console
2624    bittorrentie.e  0x531e20        SystemDrive     C:
2624    bittorrentie.e  0x531e20        SystemRoot      C:\Windows
2624    bittorrentie.e  0x531e20        TEMP    C:\Users\Rick\AppData\Local\Temp
2624    bittorrentie.e  0x531e20        TMP     C:\Users\Rick\AppData\Local\Temp
2624    bittorrentie.e  0x531e20        USERDOMAIN      WIN-LO6FAF3DTFE
2624    bittorrentie.e  0x531e20        USERNAME        Rick
2624    bittorrentie.e  0x531e20        USERPROFILE     C:\Users\Rick
2624    bittorrentie.e  0x531e20        windir  C:\Windows
2624    bittorrentie.e  0x531e20        windows_tracing_flags   3
2624    bittorrentie.e  0x531e20        windows_tracing_logfile C:\BVTBin\Tests\installpackage\csilogfile.log
708     LunarMS.exe     0x2f1da0        ALLUSERSPROFILE C:\ProgramData
708     LunarMS.exe     0x2f1da0        APPDATA C:\Users\Rick\AppData\Roaming
708     LunarMS.exe     0x2f1da0        CommonProgramFiles      C:\Program Files\Common Files
708     LunarMS.exe     0x2f1da0        CommonProgramFiles(x86) C:\Program Files (x86)\Common Files
708     LunarMS.exe     0x2f1da0        CommonProgramW6432      C:\Program Files\Common Files
708     LunarMS.exe     0x2f1da0        COMPUTERNAME    WIN-LO6FAF3DTFE
708     LunarMS.exe     0x2f1da0        ComSpec C:\Windows\system32\cmd.exe
708     LunarMS.exe     0x2f1da0        FP_NO_HOST_CHECK        NO
708     LunarMS.exe     0x2f1da0        HOMEDRIVE       C:
708     LunarMS.exe     0x2f1da0        HOMEPATH        \Users\Rick
708     LunarMS.exe     0x2f1da0        LOCALAPPDATA    C:\Users\Rick\AppData\Local
708     LunarMS.exe     0x2f1da0        LOGONSERVER     \\WIN-LO6FAF3DTFE
708     LunarMS.exe     0x2f1da0        NUMBER_OF_PROCESSORS    2
708     LunarMS.exe     0x2f1da0        OS      Windows_NT
708     LunarMS.exe     0x2f1da0        Path    C:\Windows\system32;C:\Windows;C:\Windows\System32\Wbem;C:\Windows\System32\WindowsPowerShell\v1.0\
708     LunarMS.exe     0x2f1da0        PATHEXT .COM;.EXE;.BAT;.CMD;.VBS;.VBE;.JS;.JSE;.WSF;.WSH;.MSC
708     LunarMS.exe     0x2f1da0        PROCESSOR_ARCHITECTURE  AMD64
708     LunarMS.exe     0x2f1da0        PROCESSOR_IDENTIFIER    Intel64 Family 6 Model 60 Stepping 3, GenuineIntel
708     LunarMS.exe     0x2f1da0        PROCESSOR_LEVEL 6
708     LunarMS.exe     0x2f1da0        PROCESSOR_REVISION      3c03
708     LunarMS.exe     0x2f1da0        ProgramData     C:\ProgramData
708     LunarMS.exe     0x2f1da0        ProgramFiles    C:\Program Files
708     LunarMS.exe     0x2f1da0        ProgramFiles(x86)       C:\Program Files (x86)
708     LunarMS.exe     0x2f1da0        ProgramW6432    C:\Program Files
708     LunarMS.exe     0x2f1da0        PSModulePath    C:\Windows\system32\WindowsPowerShell\v1.0\Modules\
708     LunarMS.exe     0x2f1da0        PUBLIC  C:\Users\Public
708     LunarMS.exe     0x2f1da0        SystemDrive     C:
708     LunarMS.exe     0x2f1da0        SystemRoot      C:\Windows
708     LunarMS.exe     0x2f1da0        TEMP    C:\Users\Rick\AppData\Local\Temp
708     LunarMS.exe     0x2f1da0        TMP     C:\Users\Rick\AppData\Local\Temp
708     LunarMS.exe     0x2f1da0        USERDOMAIN      WIN-LO6FAF3DTFE
708     LunarMS.exe     0x2f1da0        USERNAME        Rick
708     LunarMS.exe     0x2f1da0        USERPROFILE     C:\Users\Rick
708     LunarMS.exe     0x2f1da0        windir  C:\Windows
708     LunarMS.exe     0x2f1da0        windows_tracing_flags   3
708     LunarMS.exe     0x2f1da0        windows_tracing_logfile C:\BVTBin\Tests\installpackage\csilogfile.log
724     PresentationFo  0x1a1e00        ALLUSERSPROFILE C:\ProgramData
724     PresentationFo  0x1a1e00        APPDATA C:\Windows\ServiceProfiles\LocalService\AppData\Roaming
724     PresentationFo  0x1a1e00        CommonProgramFiles      C:\Program Files\Common Files
724     PresentationFo  0x1a1e00        CommonProgramFiles(x86) C:\Program Files (x86)\Common Files
724     PresentationFo  0x1a1e00        CommonProgramW6432      C:\Program Files\Common Files
724     PresentationFo  0x1a1e00        COMPUTERNAME    WIN-LO6FAF3DTFE
724     PresentationFo  0x1a1e00        ComSpec C:\Windows\system32\cmd.exe
724     PresentationFo  0x1a1e00        FP_NO_HOST_CHECK        NO
724     PresentationFo  0x1a1e00        LOCALAPPDATA    C:\Windows\ServiceProfiles\LocalService\AppData\Local
724     PresentationFo  0x1a1e00        NUMBER_OF_PROCESSORS    2
724     PresentationFo  0x1a1e00        OS      Windows_NT
724     PresentationFo  0x1a1e00        Path    C:\Windows\system32;C:\Windows;C:\Windows\System32\Wbem;C:\Windows\System32\WindowsPowerShell\v1.0\
724     PresentationFo  0x1a1e00        PATHEXT .COM;.EXE;.BAT;.CMD;.VBS;.VBE;.JS;.JSE;.WSF;.WSH;.MSC
724     PresentationFo  0x1a1e00        PROCESSOR_ARCHITECTURE  AMD64
724     PresentationFo  0x1a1e00        PROCESSOR_IDENTIFIER    Intel64 Family 6 Model 60 Stepping 3, GenuineIntel
724     PresentationFo  0x1a1e00        PROCESSOR_LEVEL 6
724     PresentationFo  0x1a1e00        PROCESSOR_REVISION      3c03
724     PresentationFo  0x1a1e00        ProgramData     C:\ProgramData
724     PresentationFo  0x1a1e00        ProgramFiles    C:\Program Files
724     PresentationFo  0x1a1e00        ProgramFiles(x86)       C:\Program Files (x86)
724     PresentationFo  0x1a1e00        ProgramW6432    C:\Program Files
724     PresentationFo  0x1a1e00        PSModulePath    C:\Windows\system32\WindowsPowerShell\v1.0\Modules\
724     PresentationFo  0x1a1e00        PUBLIC  C:\Users\Public
724     PresentationFo  0x1a1e00        SystemDrive     C:
724     PresentationFo  0x1a1e00        SystemRoot      C:\Windows
724     PresentationFo  0x1a1e00        TEMP    C:\Windows\SERVIC~2\LOCALS~1\AppData\Local\Temp
724     PresentationFo  0x1a1e00        TMP     C:\Windows\SERVIC~2\LOCALS~1\AppData\Local\Temp
724     PresentationFo  0x1a1e00        USERDOMAIN      NT AUTHORITY
724     PresentationFo  0x1a1e00        USERNAME        LOCAL SERVICE
724     PresentationFo  0x1a1e00        USERPROFILE     C:\Windows\ServiceProfiles\LocalService
724     PresentationFo  0x1a1e00        windir  C:\Windows
724     PresentationFo  0x1a1e00        windows_tracing_flags   3
724     PresentationFo  0x1a1e00        windows_tracing_logfile C:\BVTBin\Tests\installpackage\csilogfile.log
412     mscorsvw.exe    0x371d90        ALLUSERSPROFILE C:\ProgramData
412     mscorsvw.exe    0x371d90        APPDATA C:\Windows\system32\config\systemprofile\AppData\Roaming
412     mscorsvw.exe    0x371d90        CommonProgramFiles      C:\Program Files\Common Files
412     mscorsvw.exe    0x371d90        CommonProgramFiles(x86) C:\Program Files (x86)\Common Files
412     mscorsvw.exe    0x371d90        CommonProgramW6432      C:\Program Files\Common Files
412     mscorsvw.exe    0x371d90        COMPUTERNAME    WIN-LO6FAF3DTFE
412     mscorsvw.exe    0x371d90        ComSpec C:\Windows\system32\cmd.exe
412     mscorsvw.exe    0x371d90        FP_NO_HOST_CHECK        NO
412     mscorsvw.exe    0x371d90        LOCALAPPDATA    C:\Windows\system32\config\systemprofile\AppData\Local
412     mscorsvw.exe    0x371d90        NUMBER_OF_PROCESSORS    2
412     mscorsvw.exe    0x371d90        OS      Windows_NT
412     mscorsvw.exe    0x371d90        Path    C:\Windows\system32;C:\Windows;C:\Windows\System32\Wbem;C:\Windows\System32\WindowsPowerShell\v1.0\;
412     mscorsvw.exe    0x371d90        PATHEXT .COM;.EXE;.BAT;.CMD;.VBS;.VBE;.JS;.JSE;.WSF;.WSH;.MSC
412     mscorsvw.exe    0x371d90        PROCESSOR_ARCHITECTURE  AMD64
412     mscorsvw.exe    0x371d90        PROCESSOR_IDENTIFIER    Intel64 Family 6 Model 60 Stepping 3, GenuineIntel
412     mscorsvw.exe    0x371d90        PROCESSOR_LEVEL 6
412     mscorsvw.exe    0x371d90        PROCESSOR_REVISION      3c03
412     mscorsvw.exe    0x371d90        ProgramData     C:\ProgramData
412     mscorsvw.exe    0x371d90        ProgramFiles    C:\Program Files
412     mscorsvw.exe    0x371d90        ProgramFiles(x86)       C:\Program Files (x86)
412     mscorsvw.exe    0x371d90        ProgramW6432    C:\Program Files
412     mscorsvw.exe    0x371d90        PSModulePath    C:\Windows\system32\WindowsPowerShell\v1.0\Modules\
412     mscorsvw.exe    0x371d90        PUBLIC  C:\Users\Public
412     mscorsvw.exe    0x371d90        SystemDrive     C:
412     mscorsvw.exe    0x371d90        SystemRoot      C:\Windows
412     mscorsvw.exe    0x371d90        TEMP    C:\Windows\TEMP
412     mscorsvw.exe    0x371d90        TMP     C:\Windows\TEMP
412     mscorsvw.exe    0x371d90        USERDOMAIN      WORKGROUP
412     mscorsvw.exe    0x371d90        USERNAME        WIN-LO6FAF3DTFE$
412     mscorsvw.exe    0x371d90        USERPROFILE     C:\Windows\system32\config\systemprofile
412     mscorsvw.exe    0x371d90        windir  C:\Windows
412     mscorsvw.exe    0x371d90        windows_tracing_flags   3
412     mscorsvw.exe    0x371d90        windows_tracing_logfile C:\BVTBin\Tests\installpackage\csilogfile.log
164     svchost.exe     0x241e00        ALLUSERSPROFILE C:\ProgramData
164     svchost.exe     0x241e00        APPDATA C:\Windows\ServiceProfiles\LocalService\AppData\Roaming
164     svchost.exe     0x241e00        CommonProgramFiles      C:\Program Files\Common Files
164     svchost.exe     0x241e00        CommonProgramFiles(x86) C:\Program Files (x86)\Common Files
164     svchost.exe     0x241e00        CommonProgramW6432      C:\Program Files\Common Files
164     svchost.exe     0x241e00        COMPUTERNAME    WIN-LO6FAF3DTFE
164     svchost.exe     0x241e00        ComSpec C:\Windows\system32\cmd.exe
164     svchost.exe     0x241e00        FP_NO_HOST_CHECK        NO
164     svchost.exe     0x241e00        LOCALAPPDATA    C:\Windows\ServiceProfiles\LocalService\AppData\Local
164     svchost.exe     0x241e00        NUMBER_OF_PROCESSORS    2
164     svchost.exe     0x241e00        OS      Windows_NT
164     svchost.exe     0x241e00        Path    C:\Windows\system32;C:\Windows;C:\Windows\System32\Wbem;C:\Windows\System32\WindowsPowerShell\v1.0\
164     svchost.exe     0x241e00        PATHEXT .COM;.EXE;.BAT;.CMD;.VBS;.VBE;.JS;.JSE;.WSF;.WSH;.MSC
164     svchost.exe     0x241e00        PROCESSOR_ARCHITECTURE  AMD64
164     svchost.exe     0x241e00        PROCESSOR_IDENTIFIER    Intel64 Family 6 Model 60 Stepping 3, GenuineIntel
164     svchost.exe     0x241e00        PROCESSOR_LEVEL 6
164     svchost.exe     0x241e00        PROCESSOR_REVISION      3c03
164     svchost.exe     0x241e00        ProgramData     C:\ProgramData
164     svchost.exe     0x241e00        ProgramFiles    C:\Program Files
164     svchost.exe     0x241e00        ProgramFiles(x86)       C:\Program Files (x86)
164     svchost.exe     0x241e00        ProgramW6432    C:\Program Files
164     svchost.exe     0x241e00        PSModulePath    C:\Windows\system32\WindowsPowerShell\v1.0\Modules\
164     svchost.exe     0x241e00        PUBLIC  C:\Users\Public
164     svchost.exe     0x241e00        SystemDrive     C:
164     svchost.exe     0x241e00        SystemRoot      C:\Windows
164     svchost.exe     0x241e00        TEMP    C:\Windows\SERVIC~2\LOCALS~1\AppData\Local\Temp
164     svchost.exe     0x241e00        TMP     C:\Windows\SERVIC~2\LOCALS~1\AppData\Local\Temp
164     svchost.exe     0x241e00        USERDOMAIN      NT AUTHORITY
164     svchost.exe     0x241e00        USERNAME        LOCAL SERVICE
164     svchost.exe     0x241e00        USERPROFILE     C:\Windows\ServiceProfiles\LocalService
164     svchost.exe     0x241e00        windir  C:\Windows
164     svchost.exe     0x241e00        windows_tracing_flags   3
164     svchost.exe     0x241e00        windows_tracing_logfile C:\BVTBin\Tests\installpackage\csilogfile.log
3124    mscorsvw.exe    0x361d90        ALLUSERSPROFILE C:\ProgramData
3124    mscorsvw.exe    0x361d90        APPDATA C:\Windows\system32\config\systemprofile\AppData\Roaming
3124    mscorsvw.exe    0x361d90        CommonProgramFiles      C:\Program Files\Common Files
3124    mscorsvw.exe    0x361d90        CommonProgramFiles(x86) C:\Program Files (x86)\Common Files
3124    mscorsvw.exe    0x361d90        CommonProgramW6432      C:\Program Files\Common Files
3124    mscorsvw.exe    0x361d90        COMPUTERNAME    WIN-LO6FAF3DTFE
3124    mscorsvw.exe    0x361d90        ComSpec C:\Windows\system32\cmd.exe
3124    mscorsvw.exe    0x361d90        FP_NO_HOST_CHECK        NO
3124    mscorsvw.exe    0x361d90        LOCALAPPDATA    C:\Windows\system32\config\systemprofile\AppData\Local
3124    mscorsvw.exe    0x361d90        NUMBER_OF_PROCESSORS    2
3124    mscorsvw.exe    0x361d90        OS      Windows_NT
3124    mscorsvw.exe    0x361d90        Path    C:\Windows\system32;C:\Windows;C:\Windows\System32\Wbem;C:\Windows\System32\WindowsPowerShell\v1.0\;
3124    mscorsvw.exe    0x361d90        PATHEXT .COM;.EXE;.BAT;.CMD;.VBS;.VBE;.JS;.JSE;.WSF;.WSH;.MSC
3124    mscorsvw.exe    0x361d90        PROCESSOR_ARCHITECTURE  AMD64
3124    mscorsvw.exe    0x361d90        PROCESSOR_IDENTIFIER    Intel64 Family 6 Model 60 Stepping 3, GenuineIntel
3124    mscorsvw.exe    0x361d90        PROCESSOR_LEVEL 6
3124    mscorsvw.exe    0x361d90        PROCESSOR_REVISION      3c03
3124    mscorsvw.exe    0x361d90        ProgramData     C:\ProgramData
3124    mscorsvw.exe    0x361d90        ProgramFiles    C:\Program Files
3124    mscorsvw.exe    0x361d90        ProgramFiles(x86)       C:\Program Files (x86)
3124    mscorsvw.exe    0x361d90        ProgramW6432    C:\Program Files
3124    mscorsvw.exe    0x361d90        PSModulePath    C:\Windows\system32\WindowsPowerShell\v1.0\Modules\
3124    mscorsvw.exe    0x361d90        PUBLIC  C:\Users\Public
3124    mscorsvw.exe    0x361d90        SystemDrive     C:
3124    mscorsvw.exe    0x361d90        SystemRoot      C:\Windows
3124    mscorsvw.exe    0x361d90        TEMP    C:\Windows\TEMP
3124    mscorsvw.exe    0x361d90        TMP     C:\Windows\TEMP
3124    mscorsvw.exe    0x361d90        USERDOMAIN      WORKGROUP
3124    mscorsvw.exe    0x361d90        USERNAME        WIN-LO6FAF3DTFE$
3124    mscorsvw.exe    0x361d90        USERPROFILE     C:\Windows\system32\config\systemprofile
3124    mscorsvw.exe    0x361d90        windir  C:\Windows
3124    mscorsvw.exe    0x361d90        windows_tracing_flags   3
3124    mscorsvw.exe    0x361d90        windows_tracing_logfile C:\BVTBin\Tests\installpackage\csilogfile.log
3196    svchost.exe     0x361d90        ALLUSERSPROFILE C:\ProgramData
3196    svchost.exe     0x361d90        APPDATA C:\Windows\system32\config\systemprofile\AppData\Roaming
3196    svchost.exe     0x361d90        CommonProgramFiles      C:\Program Files\Common Files
3196    svchost.exe     0x361d90        CommonProgramFiles(x86) C:\Program Files (x86)\Common Files
3196    svchost.exe     0x361d90        CommonProgramW6432      C:\Program Files\Common Files
3196    svchost.exe     0x361d90        COMPUTERNAME    WIN-LO6FAF3DTFE
3196    svchost.exe     0x361d90        ComSpec C:\Windows\system32\cmd.exe
3196    svchost.exe     0x361d90        FP_NO_HOST_CHECK        NO
3196    svchost.exe     0x361d90        LOCALAPPDATA    C:\Windows\system32\config\systemprofile\AppData\Local
3196    svchost.exe     0x361d90        MpConfig_ProductAppDataPath     C:\ProgramData\Microsoft\Windows Defender
3196    svchost.exe     0x361d90        MpConfig_ProductCodeName        AntiSpyware
3196    svchost.exe     0x361d90        MpConfig_ProductPath    c:\program files\windows defender
3196    svchost.exe     0x361d90        MpConfig_ProductUserAppDataPath C:\Windows\system32\config\systemprofile\AppData\Local\Microsoft\Windows Defender
3196    svchost.exe     0x361d90        MpConfig_ReportingGUID  E7E10F56-B6E7-46CA-8174-0B336724C50A
3196    svchost.exe     0x361d90        NUMBER_OF_PROCESSORS    2
3196    svchost.exe     0x361d90        OS      Windows_NT
3196    svchost.exe     0x361d90        Path    C:\Windows\system32;C:\Windows;C:\Windows\System32\Wbem;C:\Windows\System32\WindowsPowerShell\v1.0\
3196    svchost.exe     0x361d90        PATHEXT .COM;.EXE;.BAT;.CMD;.VBS;.VBE;.JS;.JSE;.WSF;.WSH;.MSC
3196    svchost.exe     0x361d90        PROCESSOR_ARCHITECTURE  AMD64
3196    svchost.exe     0x361d90        PROCESSOR_IDENTIFIER    Intel64 Family 6 Model 60 Stepping 3, GenuineIntel
3196    svchost.exe     0x361d90        PROCESSOR_LEVEL 6
3196    svchost.exe     0x361d90        PROCESSOR_REVISION      3c03
3196    svchost.exe     0x361d90        ProgramData     C:\ProgramData
3196    svchost.exe     0x361d90        ProgramFiles    C:\Program Files
3196    svchost.exe     0x361d90        ProgramFiles(x86)       C:\Program Files (x86)
3196    svchost.exe     0x361d90        ProgramW6432    C:\Program Files
3196    svchost.exe     0x361d90        PSModulePath    C:\Windows\system32\WindowsPowerShell\v1.0\Modules\
3196    svchost.exe     0x361d90        PUBLIC  C:\Users\Public
3196    svchost.exe     0x361d90        SystemDrive     C:
3196    svchost.exe     0x361d90        SystemRoot      C:\Windows
3196    svchost.exe     0x361d90        TEMP    C:\Windows\TEMP
3196    svchost.exe     0x361d90        TMP     C:\Windows\TEMP
3196    svchost.exe     0x361d90        USERDOMAIN      WORKGROUP
3196    svchost.exe     0x361d90        USERNAME        WIN-LO6FAF3DTFE$
3196    svchost.exe     0x361d90        USERPROFILE     C:\Windows\system32\config\systemprofile
3196    svchost.exe     0x361d90        windir  C:\Windows
3196    svchost.exe     0x361d90        windows_tracing_flags   3
3196    svchost.exe     0x361d90        windows_tracing_logfile C:\BVTBin\Tests\installpackage\csilogfile.log
4076    chrome.exe      0x401e40        ALLUSERSPROFILE C:\ProgramData
4076    chrome.exe      0x401e40        APPDATA C:\Users\Rick\AppData\Roaming
4076    chrome.exe      0x401e40        CHROME_CRASHPAD_PIPE_NAME       \\.\pipe\crashpad_4076_DAXLEIZKCFCTZZUS
4076    chrome.exe      0x401e40        CHROME_RESTART  Google Chrome|Whoa! Google Chrome has crashed. Relaunch now?|LEFT_TO_RIGHT
4076    chrome.exe      0x401e40        CommonProgramFiles      C:\Program Files\Common Files
4076    chrome.exe      0x401e40        CommonProgramFiles(x86) C:\Program Files (x86)\Common Files
4076    chrome.exe      0x401e40        CommonProgramW6432      C:\Program Files\Common Files
4076    chrome.exe      0x401e40        COMPUTERNAME    WIN-LO6FAF3DTFE
4076    chrome.exe      0x401e40        ComSpec C:\Windows\system32\cmd.exe
4076    chrome.exe      0x401e40        FP_NO_HOST_CHECK        NO
4076    chrome.exe      0x401e40        HOMEDRIVE       C:
4076    chrome.exe      0x401e40        HOMEPATH        \Users\Rick
4076    chrome.exe      0x401e40        LOCALAPPDATA    C:\Users\Rick\AppData\Local
4076    chrome.exe      0x401e40        LOGONSERVER     \\WIN-LO6FAF3DTFE
4076    chrome.exe      0x401e40        MpConfig_ProductAppDataPath     C:\ProgramData\Microsoft\Windows Defender
4076    chrome.exe      0x401e40        MpConfig_ProductCodeName        AntiSpyware
4076    chrome.exe      0x401e40        MpConfig_ProductPath    C:\Program Files\Windows Defender
4076    chrome.exe      0x401e40        MpConfig_ProductUserAppDataPath C:\Users\Rick\AppData\Local\Microsoft\Windows Defender
4076    chrome.exe      0x401e40        MpConfig_ReportingGUID  E7E10F56-B6E7-46CA-8174-0B336724C50A
4076    chrome.exe      0x401e40        NUMBER_OF_PROCESSORS    2
4076    chrome.exe      0x401e40        OS      Windows_NT
4076    chrome.exe      0x401e40        Path    C:\Program Files (x86)\Google\Chrome\Application;C:\Windows\system32;C:\Windows;C:\Windows\System32\Wbem;C:\Windows\System32\WindowsPowerShell\v1.0\
4076    chrome.exe      0x401e40        PATHEXT .COM;.EXE;.BAT;.CMD;.VBS;.VBE;.JS;.JSE;.WSF;.WSH;.MSC
4076    chrome.exe      0x401e40        PROCESSOR_ARCHITECTURE  AMD64
4076    chrome.exe      0x401e40        PROCESSOR_IDENTIFIER    Intel64 Family 6 Model 60 Stepping 3, GenuineIntel
4076    chrome.exe      0x401e40        PROCESSOR_LEVEL 6
4076    chrome.exe      0x401e40        PROCESSOR_REVISION      3c03
4076    chrome.exe      0x401e40        ProgramData     C:\ProgramData
4076    chrome.exe      0x401e40        ProgramFiles    C:\Program Files
4076    chrome.exe      0x401e40        ProgramFiles(x86)       C:\Program Files (x86)
4076    chrome.exe      0x401e40        ProgramW6432    C:\Program Files
4076    chrome.exe      0x401e40        PSModulePath    C:\Windows\system32\WindowsPowerShell\v1.0\Modules\
4076    chrome.exe      0x401e40        PUBLIC  C:\Users\Public
4076    chrome.exe      0x401e40        SESSIONNAME     Console
4076    chrome.exe      0x401e40        SystemDrive     C:
4076    chrome.exe      0x401e40        SystemRoot      C:\Windows
4076    chrome.exe      0x401e40        TEMP    C:\Users\Rick\AppData\Local\Temp
4076    chrome.exe      0x401e40        TMP     C:\Users\Rick\AppData\Local\Temp
4076    chrome.exe      0x401e40        USERDOMAIN      WIN-LO6FAF3DTFE
4076    chrome.exe      0x401e40        USERNAME        Rick
4076    chrome.exe      0x401e40        USERPROFILE     C:\Users\Rick
4076    chrome.exe      0x401e40        windir  C:\Windows
4076    chrome.exe      0x401e40        windows_tracing_flags   3
4076    chrome.exe      0x401e40        windows_tracing_logfile C:\BVTBin\Tests\installpackage\csilogfile.log
4084    chrome.exe      0x341e40        ALLUSERSPROFILE C:\ProgramData
4084    chrome.exe      0x341e40        APPDATA C:\Users\Rick\AppData\Roaming
4084    chrome.exe      0x341e40        CommonProgramFiles      C:\Program Files\Common Files
4084    chrome.exe      0x341e40        CommonProgramFiles(x86) C:\Program Files (x86)\Common Files
4084    chrome.exe      0x341e40        CommonProgramW6432      C:\Program Files\Common Files
4084    chrome.exe      0x341e40        COMPUTERNAME    WIN-LO6FAF3DTFE
4084    chrome.exe      0x341e40        ComSpec C:\Windows\system32\cmd.exe
4084    chrome.exe      0x341e40        FP_NO_HOST_CHECK        NO
4084    chrome.exe      0x341e40        HOMEDRIVE       C:
4084    chrome.exe      0x341e40        HOMEPATH        \Users\Rick
4084    chrome.exe      0x341e40        LOCALAPPDATA    C:\Users\Rick\AppData\Local
4084    chrome.exe      0x341e40        LOGONSERVER     \\WIN-LO6FAF3DTFE
4084    chrome.exe      0x341e40        NUMBER_OF_PROCESSORS    2
4084    chrome.exe      0x341e40        OS      Windows_NT
4084    chrome.exe      0x341e40        Path    C:\Program Files (x86)\Google\Chrome\Application;C:\Windows\system32;C:\Windows;C:\Windows\System32\Wbem;C:\Windows\System32\WindowsPowerShell\v1.0\
4084    chrome.exe      0x341e40        PATHEXT .COM;.EXE;.BAT;.CMD;.VBS;.VBE;.JS;.JSE;.WSF;.WSH;.MSC
4084    chrome.exe      0x341e40        PROCESSOR_ARCHITECTURE  AMD64
4084    chrome.exe      0x341e40        PROCESSOR_IDENTIFIER    Intel64 Family 6 Model 60 Stepping 3, GenuineIntel
4084    chrome.exe      0x341e40        PROCESSOR_LEVEL 6
4084    chrome.exe      0x341e40        PROCESSOR_REVISION      3c03
4084    chrome.exe      0x341e40        ProgramData     C:\ProgramData
4084    chrome.exe      0x341e40        ProgramFiles    C:\Program Files
4084    chrome.exe      0x341e40        ProgramFiles(x86)       C:\Program Files (x86)
4084    chrome.exe      0x341e40        ProgramW6432    C:\Program Files
4084    chrome.exe      0x341e40        PSModulePath    C:\Windows\system32\WindowsPowerShell\v1.0\Modules\
4084    chrome.exe      0x341e40        PUBLIC  C:\Users\Public
4084    chrome.exe      0x341e40        SESSIONNAME     Console
4084    chrome.exe      0x341e40        SystemDrive     C:
4084    chrome.exe      0x341e40        SystemRoot      C:\Windows
4084    chrome.exe      0x341e40        TEMP    C:\Users\Rick\AppData\Local\Temp
4084    chrome.exe      0x341e40        TMP     C:\Users\Rick\AppData\Local\Temp
4084    chrome.exe      0x341e40        USERDOMAIN      WIN-LO6FAF3DTFE
4084    chrome.exe      0x341e40        USERNAME        Rick
4084    chrome.exe      0x341e40        USERPROFILE     C:\Users\Rick
4084    chrome.exe      0x341e40        windir  C:\Windows
4084    chrome.exe      0x341e40        windows_tracing_flags   3
4084    chrome.exe      0x341e40        windows_tracing_logfile C:\BVTBin\Tests\installpackage\csilogfile.log
576     chrome.exe      0x471ec0        ALLUSERSPROFILE C:\ProgramData
576     chrome.exe      0x471ec0        APPDATA C:\Users\Rick\AppData\Roaming
576     chrome.exe      0x471ec0        CHROME_CRASHPAD_PIPE_NAME       \\.\pipe\crashpad_4076_DAXLEIZKCFCTZZUS
576     chrome.exe      0x471ec0        CommonProgramFiles      C:\Program Files\Common Files
576     chrome.exe      0x471ec0        CommonProgramFiles(x86) C:\Program Files (x86)\Common Files
576     chrome.exe      0x471ec0        CommonProgramW6432      C:\Program Files\Common Files
576     chrome.exe      0x471ec0        COMPUTERNAME    WIN-LO6FAF3DTFE
576     chrome.exe      0x471ec0        ComSpec C:\Windows\system32\cmd.exe
576     chrome.exe      0x471ec0        FP_NO_HOST_CHECK        NO
576     chrome.exe      0x471ec0        HOMEDRIVE       C:
576     chrome.exe      0x471ec0        HOMEPATH        \Users\Rick
576     chrome.exe      0x471ec0        LOCALAPPDATA    C:\Users\Rick\AppData\Local
576     chrome.exe      0x471ec0        LOGONSERVER     \\WIN-LO6FAF3DTFE
576     chrome.exe      0x471ec0        NUMBER_OF_PROCESSORS    2
576     chrome.exe      0x471ec0        OS      Windows_NT
576     chrome.exe      0x471ec0        Path    C:\Program Files (x86)\Google\Chrome\Application;C:\Windows\system32;C:\Windows;C:\Windows\System32\Wbem;C:\Windows\System32\WindowsPowerShell\v1.0\
576     chrome.exe      0x471ec0        PATHEXT .COM;.EXE;.BAT;.CMD;.VBS;.VBE;.JS;.JSE;.WSF;.WSH;.MSC
576     chrome.exe      0x471ec0        PROCESSOR_ARCHITECTURE  AMD64
576     chrome.exe      0x471ec0        PROCESSOR_IDENTIFIER    Intel64 Family 6 Model 60 Stepping 3, GenuineIntel
576     chrome.exe      0x471ec0        PROCESSOR_LEVEL 6
576     chrome.exe      0x471ec0        PROCESSOR_REVISION      3c03
576     chrome.exe      0x471ec0        ProgramData     C:\ProgramData
576     chrome.exe      0x471ec0        ProgramFiles    C:\Program Files
576     chrome.exe      0x471ec0        ProgramFiles(x86)       C:\Program Files (x86)
576     chrome.exe      0x471ec0        ProgramW6432    C:\Program Files
576     chrome.exe      0x471ec0        PSModulePath    C:\Windows\system32\WindowsPowerShell\v1.0\Modules\
576     chrome.exe      0x471ec0        PUBLIC  C:\Users\Public
576     chrome.exe      0x471ec0        SESSIONNAME     Console
576     chrome.exe      0x471ec0        SystemDrive     C:
576     chrome.exe      0x471ec0        SystemRoot      C:\Windows
576     chrome.exe      0x471ec0        TEMP    C:\Users\Rick\AppData\Local\Temp
576     chrome.exe      0x471ec0        TMP     C:\Users\Rick\AppData\Local\Temp
576     chrome.exe      0x471ec0        USERDOMAIN      WIN-LO6FAF3DTFE
576     chrome.exe      0x471ec0        USERNAME        Rick
576     chrome.exe      0x471ec0        USERPROFILE     C:\Users\Rick
576     chrome.exe      0x471ec0        windir  C:\Windows
576     chrome.exe      0x471ec0        windows_tracing_flags   3
576     chrome.exe      0x471ec0        windows_tracing_logfile C:\BVTBin\Tests\installpackage\csilogfile.log
1808    chrome.exe      0x3b1ec0        ALLUSERSPROFILE C:\ProgramData
1808    chrome.exe      0x3b1ec0        APPDATA C:\Users\Rick\AppData\Roaming
1808    chrome.exe      0x3b1ec0        CHROME_CRASHPAD_PIPE_NAME       \\.\pipe\crashpad_4076_DAXLEIZKCFCTZZUS
1808    chrome.exe      0x3b1ec0        CommonProgramFiles      C:\Program Files\Common Files
1808    chrome.exe      0x3b1ec0        CommonProgramFiles(x86) C:\Program Files (x86)\Common Files
1808    chrome.exe      0x3b1ec0        CommonProgramW6432      C:\Program Files\Common Files
1808    chrome.exe      0x3b1ec0        COMPUTERNAME    WIN-LO6FAF3DTFE
1808    chrome.exe      0x3b1ec0        ComSpec C:\Windows\system32\cmd.exe
1808    chrome.exe      0x3b1ec0        FP_NO_HOST_CHECK        NO
1808    chrome.exe      0x3b1ec0        HOMEDRIVE       C:
1808    chrome.exe      0x3b1ec0        HOMEPATH        \Users\Rick
1808    chrome.exe      0x3b1ec0        LOCALAPPDATA    C:\Users\Rick\AppData\Local
1808    chrome.exe      0x3b1ec0        LOGONSERVER     \\WIN-LO6FAF3DTFE
1808    chrome.exe      0x3b1ec0        NUMBER_OF_PROCESSORS    2
1808    chrome.exe      0x3b1ec0        OS      Windows_NT
1808    chrome.exe      0x3b1ec0        Path    C:\Program Files (x86)\Google\Chrome\Application;C:\Windows\system32;C:\Windows;C:\Windows\System32\Wbem;C:\Windows\System32\WindowsPowerShell\v1.0\
1808    chrome.exe      0x3b1ec0        PATHEXT .COM;.EXE;.BAT;.CMD;.VBS;.VBE;.JS;.JSE;.WSF;.WSH;.MSC
1808    chrome.exe      0x3b1ec0        PROCESSOR_ARCHITECTURE  AMD64
1808    chrome.exe      0x3b1ec0        PROCESSOR_IDENTIFIER    Intel64 Family 6 Model 60 Stepping 3, GenuineIntel
1808    chrome.exe      0x3b1ec0        PROCESSOR_LEVEL 6
1808    chrome.exe      0x3b1ec0        PROCESSOR_REVISION      3c03
1808    chrome.exe      0x3b1ec0        ProgramData     C:\ProgramData
1808    chrome.exe      0x3b1ec0        ProgramFiles    C:\Program Files
1808    chrome.exe      0x3b1ec0        ProgramFiles(x86)       C:\Program Files (x86)
1808    chrome.exe      0x3b1ec0        ProgramW6432    C:\Program Files
1808    chrome.exe      0x3b1ec0        PSModulePath    C:\Windows\system32\WindowsPowerShell\v1.0\Modules\
1808    chrome.exe      0x3b1ec0        PUBLIC  C:\Users\Public
1808    chrome.exe      0x3b1ec0        SESSIONNAME     Console
1808    chrome.exe      0x3b1ec0        SystemDrive     C:
1808    chrome.exe      0x3b1ec0        SystemRoot      C:\Windows
1808    chrome.exe      0x3b1ec0        TEMP    C:\Users\Rick\AppData\Local\Temp
1808    chrome.exe      0x3b1ec0        TMP     C:\Users\Rick\AppData\Local\Temp
1808    chrome.exe      0x3b1ec0        USERDOMAIN      WIN-LO6FAF3DTFE
1808    chrome.exe      0x3b1ec0        USERNAME        Rick
1808    chrome.exe      0x3b1ec0        USERPROFILE     C:\Users\Rick
1808    chrome.exe      0x3b1ec0        windir  C:\Windows
1808    chrome.exe      0x3b1ec0        windows_tracing_flags   3
1808    chrome.exe      0x3b1ec0        windows_tracing_logfile C:\BVTBin\Tests\installpackage\csilogfile.log
3924    chrome.exe      0x4a1f70        ALLUSERSPROFILE C:\ProgramData
3924    chrome.exe      0x4a1f70        APPDATA C:\Users\Rick\AppData\Roaming
3924    chrome.exe      0x4a1f70        CHROME_CRASHPAD_PIPE_NAME       \\.\pipe\crashpad_4076_DAXLEIZKCFCTZZUS
3924    chrome.exe      0x4a1f70        CHROME_RESTART  Google Chrome|Whoa! Google Chrome has crashed. Relaunch now?|LEFT_TO_RIGHT
3924    chrome.exe      0x4a1f70        CommonProgramFiles      C:\Program Files\Common Files
3924    chrome.exe      0x4a1f70        CommonProgramFiles(x86) C:\Program Files (x86)\Common Files
3924    chrome.exe      0x4a1f70        CommonProgramW6432      C:\Program Files\Common Files
3924    chrome.exe      0x4a1f70        COMPUTERNAME    WIN-LO6FAF3DTFE
3924    chrome.exe      0x4a1f70        ComSpec C:\Windows\system32\cmd.exe
3924    chrome.exe      0x4a1f70        FP_NO_HOST_CHECK        NO
3924    chrome.exe      0x4a1f70        HOMEDRIVE       C:
3924    chrome.exe      0x4a1f70        HOMEPATH        \Users\Rick
3924    chrome.exe      0x4a1f70        LOCALAPPDATA    C:\Users\Rick\AppData\Local
3924    chrome.exe      0x4a1f70        LOGONSERVER     \\WIN-LO6FAF3DTFE
3924    chrome.exe      0x4a1f70        NUMBER_OF_PROCESSORS    2
3924    chrome.exe      0x4a1f70        OS      Windows_NT
3924    chrome.exe      0x4a1f70        Path    C:\Program Files (x86)\Google\Chrome\Application;C:\Windows\system32;C:\Windows;C:\Windows\System32\Wbem;C:\Windows\System32\WindowsPowerShell\v1.0\
3924    chrome.exe      0x4a1f70        PATHEXT .COM;.EXE;.BAT;.CMD;.VBS;.VBE;.JS;.JSE;.WSF;.WSH;.MSC
3924    chrome.exe      0x4a1f70        PROCESSOR_ARCHITECTURE  AMD64
3924    chrome.exe      0x4a1f70        PROCESSOR_IDENTIFIER    Intel64 Family 6 Model 60 Stepping 3, GenuineIntel
3924    chrome.exe      0x4a1f70        PROCESSOR_LEVEL 6
3924    chrome.exe      0x4a1f70        PROCESSOR_REVISION      3c03
3924    chrome.exe      0x4a1f70        ProgramData     C:\ProgramData
3924    chrome.exe      0x4a1f70        ProgramFiles    C:\Program Files
3924    chrome.exe      0x4a1f70        ProgramFiles(x86)       C:\Program Files (x86)
3924    chrome.exe      0x4a1f70        ProgramW6432    C:\Program Files
3924    chrome.exe      0x4a1f70        PSModulePath    C:\Windows\system32\WindowsPowerShell\v1.0\Modules\
3924    chrome.exe      0x4a1f70        PUBLIC  C:\Users\Public
3924    chrome.exe      0x4a1f70        SESSIONNAME     Console
3924    chrome.exe      0x4a1f70        SystemDrive     C:
3924    chrome.exe      0x4a1f70        SystemRoot      C:\Windows
3924    chrome.exe      0x4a1f70        TEMP    C:\Users\Rick\AppData\Local\Temp
3924    chrome.exe      0x4a1f70        TMP     C:\Users\Rick\AppData\Local\Temp
3924    chrome.exe      0x4a1f70        USERDOMAIN      WIN-LO6FAF3DTFE
3924    chrome.exe      0x4a1f70        USERNAME        Rick
3924    chrome.exe      0x4a1f70        USERPROFILE     C:\Users\Rick
3924    chrome.exe      0x4a1f70        windir  C:\Windows
3924    chrome.exe      0x4a1f70        windows_tracing_flags   3
3924    chrome.exe      0x4a1f70        windows_tracing_logfile C:\BVTBin\Tests\installpackage\csilogfile.log
2748    chrome.exe      0x5721e0        ALLUSERSPROFILE C:\ProgramData
2748    chrome.exe      0x5721e0        APPDATA C:\Users\Rick\AppData\Roaming
2748    chrome.exe      0x5721e0        CHROME_CRASHPAD_PIPE_NAME       \\.\pipe\crashpad_4076_DAXLEIZKCFCTZZUS
2748    chrome.exe      0x5721e0        CHROME_RESTART  Google Chrome|Whoa! Google Chrome has crashed. Relaunch now?|LEFT_TO_RIGHT
2748    chrome.exe      0x5721e0        CommonProgramFiles      C:\Program Files\Common Files
2748    chrome.exe      0x5721e0        CommonProgramFiles(x86) C:\Program Files (x86)\Common Files
2748    chrome.exe      0x5721e0        CommonProgramW6432      C:\Program Files\Common Files
2748    chrome.exe      0x5721e0        COMPUTERNAME    WIN-LO6FAF3DTFE
2748    chrome.exe      0x5721e0        ComSpec C:\Windows\system32\cmd.exe
2748    chrome.exe      0x5721e0        FP_NO_HOST_CHECK        NO
2748    chrome.exe      0x5721e0        HOMEDRIVE       C:
2748    chrome.exe      0x5721e0        HOMEPATH        \Users\Rick
2748    chrome.exe      0x5721e0        LOCALAPPDATA    C:\Users\Rick\AppData\Local
2748    chrome.exe      0x5721e0        LOGONSERVER     \\WIN-LO6FAF3DTFE
2748    chrome.exe      0x5721e0        MpConfig_ProductAppDataPath     C:\ProgramData\Microsoft\Windows Defender
2748    chrome.exe      0x5721e0        MpConfig_ProductCodeName        AntiSpyware
2748    chrome.exe      0x5721e0        MpConfig_ProductPath    C:\Program Files\Windows Defender
2748    chrome.exe      0x5721e0        MpConfig_ProductUserAppDataPath C:\Users\Rick\AppData\Local\Microsoft\Windows Defender
2748    chrome.exe      0x5721e0        MpConfig_ReportingGUID  E7E10F56-B6E7-46CA-8174-0B336724C50A
2748    chrome.exe      0x5721e0        NUMBER_OF_PROCESSORS    2
2748    chrome.exe      0x5721e0        OS      Windows_NT
2748    chrome.exe      0x5721e0        Path    C:\Program Files (x86)\Google\Chrome\Application;C:\Windows\system32;C:\Windows;C:\Windows\System32\Wbem;C:\Windows\System32\WindowsPowerShell\v1.0\
2748    chrome.exe      0x5721e0        PATHEXT .COM;.EXE;.BAT;.CMD;.VBS;.VBE;.JS;.JSE;.WSF;.WSH;.MSC
2748    chrome.exe      0x5721e0        PROCESSOR_ARCHITECTURE  AMD64
2748    chrome.exe      0x5721e0        PROCESSOR_IDENTIFIER    Intel64 Family 6 Model 60 Stepping 3, GenuineIntel
2748    chrome.exe      0x5721e0        PROCESSOR_LEVEL 6
2748    chrome.exe      0x5721e0        PROCESSOR_REVISION      3c03
2748    chrome.exe      0x5721e0        ProgramData     C:\ProgramData
2748    chrome.exe      0x5721e0        ProgramFiles    C:\Program Files
2748    chrome.exe      0x5721e0        ProgramFiles(x86)       C:\Program Files (x86)
2748    chrome.exe      0x5721e0        ProgramW6432    C:\Program Files
2748    chrome.exe      0x5721e0        PSModulePath    C:\Windows\system32\WindowsPowerShell\v1.0\Modules\
2748    chrome.exe      0x5721e0        PUBLIC  C:\Users\Public
2748    chrome.exe      0x5721e0        SESSIONNAME     Console
2748    chrome.exe      0x5721e0        SystemDrive     C:
2748    chrome.exe      0x5721e0        SystemRoot      C:\Windows
2748    chrome.exe      0x5721e0        TEMP    C:\Users\Rick\AppData\Local\Temp
2748    chrome.exe      0x5721e0        TMP     C:\Users\Rick\AppData\Local\Temp
2748    chrome.exe      0x5721e0        USERDOMAIN      WIN-LO6FAF3DTFE
2748    chrome.exe      0x5721e0        USERNAME        Rick
2748    chrome.exe      0x5721e0        USERPROFILE     C:\Users\Rick
2748    chrome.exe      0x5721e0        windir  C:\Windows
2748    chrome.exe      0x5721e0        windows_tracing_flags   3
2748    chrome.exe      0x5721e0        windows_tracing_logfile C:\BVTBin\Tests\installpackage\csilogfile.log
3820    Rick And Morty  0x331dd0        ALLUSERSPROFILE C:\ProgramData
3820    Rick And Morty  0x331dd0        APPDATA C:\Users\Rick\AppData\Roaming
3820    Rick And Morty  0x331dd0        CommonProgramFiles      C:\Program Files\Common Files
3820    Rick And Morty  0x331dd0        CommonProgramFiles(x86) C:\Program Files (x86)\Common Files
3820    Rick And Morty  0x331dd0        CommonProgramW6432      C:\Program Files\Common Files
3820    Rick And Morty  0x331dd0        COMPUTERNAME    WIN-LO6FAF3DTFE
3820    Rick And Morty  0x331dd0        ComSpec C:\Windows\system32\cmd.exe
3820    Rick And Morty  0x331dd0        FP_NO_HOST_CHECK        NO
3820    Rick And Morty  0x331dd0        HOMEDRIVE       C:
3820    Rick And Morty  0x331dd0        HOMEPATH        \Users\Rick
3820    Rick And Morty  0x331dd0        LOCALAPPDATA    C:\Users\Rick\AppData\Local
3820    Rick And Morty  0x331dd0        LOGONSERVER     \\WIN-LO6FAF3DTFE
3820    Rick And Morty  0x331dd0        NUMBER_OF_PROCESSORS    2
3820    Rick And Morty  0x331dd0        OS      Windows_NT
3820    Rick And Morty  0x331dd0        Path    C:\Windows\system32;C:\Windows;C:\Windows\System32\Wbem;C:\Windows\System32\WindowsPowerShell\v1.0\
3820    Rick And Morty  0x331dd0        PATHEXT .COM;.EXE;.BAT;.CMD;.VBS;.VBE;.JS;.JSE;.WSF;.WSH;.MSC
3820    Rick And Morty  0x331dd0        PROCESSOR_ARCHITECTURE  AMD64
3820    Rick And Morty  0x331dd0        PROCESSOR_IDENTIFIER    Intel64 Family 6 Model 60 Stepping 3, GenuineIntel
3820    Rick And Morty  0x331dd0        PROCESSOR_LEVEL 6
3820    Rick And Morty  0x331dd0        PROCESSOR_REVISION      3c03
3820    Rick And Morty  0x331dd0        ProgramData     C:\ProgramData
3820    Rick And Morty  0x331dd0        ProgramFiles    C:\Program Files
3820    Rick And Morty  0x331dd0        ProgramFiles(x86)       C:\Program Files (x86)
3820    Rick And Morty  0x331dd0        ProgramW6432    C:\Program Files
3820    Rick And Morty  0x331dd0        PSModulePath    C:\Windows\system32\WindowsPowerShell\v1.0\Modules\
3820    Rick And Morty  0x331dd0        PUBLIC  C:\Users\Public
3820    Rick And Morty  0x331dd0        SESSIONNAME     Console
3820    Rick And Morty  0x331dd0        SystemDrive     C:
3820    Rick And Morty  0x331dd0        SystemRoot      C:\Windows
3820    Rick And Morty  0x331dd0        TEMP    C:\Users\Rick\AppData\Local\Temp
3820    Rick And Morty  0x331dd0        TMP     C:\Users\Rick\AppData\Local\Temp
3820    Rick And Morty  0x331dd0        USERDOMAIN      WIN-LO6FAF3DTFE
3820    Rick And Morty  0x331dd0        USERNAME        Rick
3820    Rick And Morty  0x331dd0        USERPROFILE     C:\Users\Rick
3820    Rick And Morty  0x331dd0        windir  C:\Windows
3820    Rick And Morty  0x331dd0        windows_tracing_flags   3
3820    Rick And Morty  0x331dd0        windows_tracing_logfile C:\BVTBin\Tests\installpackage\csilogfile.log
3720    vmware-tray.ex  0x331da0        ALLUSERSPROFILE C:\ProgramData
3720    vmware-tray.ex  0x331da0        APPDATA C:\Users\Rick\AppData\Roaming
3720    vmware-tray.ex  0x331da0        CommonProgramFiles      C:\Program Files\Common Files
3720    vmware-tray.ex  0x331da0        CommonProgramFiles(x86) C:\Program Files (x86)\Common Files
3720    vmware-tray.ex  0x331da0        CommonProgramW6432      C:\Program Files\Common Files
3720    vmware-tray.ex  0x331da0        COMPUTERNAME    WIN-LO6FAF3DTFE
3720    vmware-tray.ex  0x331da0        ComSpec C:\Windows\system32\cmd.exe
3720    vmware-tray.ex  0x331da0        FP_NO_HOST_CHECK        NO
3720    vmware-tray.ex  0x331da0        HOMEDRIVE       C:
3720    vmware-tray.ex  0x331da0        HOMEPATH        \Users\Rick
3720    vmware-tray.ex  0x331da0        LOCALAPPDATA    C:\Users\Rick\AppData\Local
3720    vmware-tray.ex  0x331da0        LOGONSERVER     \\WIN-LO6FAF3DTFE
3720    vmware-tray.ex  0x331da0        NUMBER_OF_PROCESSORS    2
3720    vmware-tray.ex  0x331da0        OS      Windows_NT
3720    vmware-tray.ex  0x331da0        Path    C:\Windows\system32;C:\Windows;C:\Windows\System32\Wbem;C:\Windows\System32\WindowsPowerShell\v1.0\
3720    vmware-tray.ex  0x331da0        PATHEXT .COM;.EXE;.BAT;.CMD;.VBS;.VBE;.JS;.JSE;.WSF;.WSH;.MSC
3720    vmware-tray.ex  0x331da0        PROCESSOR_ARCHITECTURE  AMD64
3720    vmware-tray.ex  0x331da0        PROCESSOR_IDENTIFIER    Intel64 Family 6 Model 60 Stepping 3, GenuineIntel
3720    vmware-tray.ex  0x331da0        PROCESSOR_LEVEL 6
3720    vmware-tray.ex  0x331da0        PROCESSOR_REVISION      3c03
3720    vmware-tray.ex  0x331da0        ProgramData     C:\ProgramData
3720    vmware-tray.ex  0x331da0        ProgramFiles    C:\Program Files
3720    vmware-tray.ex  0x331da0        ProgramFiles(x86)       C:\Program Files (x86)
3720    vmware-tray.ex  0x331da0        ProgramW6432    C:\Program Files
3720    vmware-tray.ex  0x331da0        PSModulePath    C:\Windows\system32\WindowsPowerShell\v1.0\Modules\
3720    vmware-tray.ex  0x331da0        PUBLIC  C:\Users\Public
3720    vmware-tray.ex  0x331da0        SystemDrive     C:
3720    vmware-tray.ex  0x331da0        SystemRoot      C:\Windows
3720    vmware-tray.ex  0x331da0        TEMP    C:\Users\Rick\AppData\Local\Temp
3720    vmware-tray.ex  0x331da0        TMP     C:\Users\Rick\AppData\Local\Temp
3720    vmware-tray.ex  0x331da0        USERDOMAIN      WIN-LO6FAF3DTFE
3720    vmware-tray.ex  0x331da0        USERNAME        Rick
3720    vmware-tray.ex  0x331da0        USERPROFILE     C:\Users\Rick
3720    vmware-tray.ex  0x331da0        windir  C:\Windows
3720    vmware-tray.ex  0x331da0        windows_tracing_flags   3
3720    vmware-tray.ex  0x331da0        windows_tracing_logfile C:\BVTBin\Tests\installpackage\csilogfile.log
3880    WebCompanionIn  0x401d90        ALLUSERSPROFILE C:\ProgramData
3880    WebCompanionIn  0x401d90        APPDATA C:\Windows\system32\config\systemprofile\AppData\Roaming
3880    WebCompanionIn  0x401d90        CommonProgramFiles      C:\Program Files\Common Files
3880    WebCompanionIn  0x401d90        CommonProgramFiles(x86) C:\Program Files (x86)\Common Files
3880    WebCompanionIn  0x401d90        CommonProgramW6432      C:\Program Files\Common Files
3880    WebCompanionIn  0x401d90        COMPUTERNAME    WIN-LO6FAF3DTFE
3880    WebCompanionIn  0x401d90        ComSpec C:\Windows\system32\cmd.exe
3880    WebCompanionIn  0x401d90        FP_NO_HOST_CHECK        NO
3880    WebCompanionIn  0x401d90        LOCALAPPDATA    C:\Windows\system32\config\systemprofile\AppData\Local
3880    WebCompanionIn  0x401d90        NUMBER_OF_PROCESSORS    2
3880    WebCompanionIn  0x401d90        OS      Windows_NT
3880    WebCompanionIn  0x401d90        Path    C:\Windows\system32;C:\Windows;C:\Windows\System32\Wbem;C:\Windows\System32\WindowsPowerShell\v1.0\;
3880    WebCompanionIn  0x401d90        PATHEXT .COM;.EXE;.BAT;.CMD;.VBS;.VBE;.JS;.JSE;.WSF;.WSH;.MSC
3880    WebCompanionIn  0x401d90        PROCESSOR_ARCHITECTURE  AMD64
3880    WebCompanionIn  0x401d90        PROCESSOR_IDENTIFIER    Intel64 Family 6 Model 60 Stepping 3, GenuineIntel
3880    WebCompanionIn  0x401d90        PROCESSOR_LEVEL 6
3880    WebCompanionIn  0x401d90        PROCESSOR_REVISION      3c03
3880    WebCompanionIn  0x401d90        ProgramData     C:\ProgramData
3880    WebCompanionIn  0x401d90        ProgramFiles    C:\Program Files
3880    WebCompanionIn  0x401d90        ProgramFiles(x86)       C:\Program Files (x86)
3880    WebCompanionIn  0x401d90        ProgramW6432    C:\Program Files
3880    WebCompanionIn  0x401d90        PSModulePath    C:\Windows\system32\WindowsPowerShell\v1.0\Modules\
3880    WebCompanionIn  0x401d90        PUBLIC  C:\Users\Public
3880    WebCompanionIn  0x401d90        SystemDrive     C:
3880    WebCompanionIn  0x401d90        SystemRoot      C:\Windows
3880    WebCompanionIn  0x401d90        TEMP    C:\Windows\TEMP
3880    WebCompanionIn  0x401d90        TMP     C:\Windows\TEMP
3880    WebCompanionIn  0x401d90        USERDOMAIN      WORKGROUP
3880    WebCompanionIn  0x401d90        USERNAME        WIN-LO6FAF3DTFE$
3880    WebCompanionIn  0x401d90        USERPROFILE     C:\Windows\system32\config\systemprofile
3880    WebCompanionIn  0x401d90        windir  C:\Windows
3880    WebCompanionIn  0x401d90        windows_tracing_flags   3
3880    WebCompanionIn  0x401d90        windows_tracing_logfile C:\BVTBin\Tests\installpackage\csilogfile.log
3648    chrome.exe      0x5421e0        ALLUSERSPROFILE C:\ProgramData
3648    chrome.exe      0x5421e0        APPDATA C:\Users\Rick\AppData\Roaming
3648    chrome.exe      0x5421e0        CHROME_CRASHPAD_PIPE_NAME       \\.\pipe\crashpad_4076_DAXLEIZKCFCTZZUS
3648    chrome.exe      0x5421e0        CHROME_RESTART  Google Chrome|Whoa! Google Chrome has crashed. Relaunch now?|LEFT_TO_RIGHT
3648    chrome.exe      0x5421e0        CommonProgramFiles      C:\Program Files\Common Files
3648    chrome.exe      0x5421e0        CommonProgramFiles(x86) C:\Program Files (x86)\Common Files
3648    chrome.exe      0x5421e0        CommonProgramW6432      C:\Program Files\Common Files
3648    chrome.exe      0x5421e0        COMPUTERNAME    WIN-LO6FAF3DTFE
3648    chrome.exe      0x5421e0        ComSpec C:\Windows\system32\cmd.exe
3648    chrome.exe      0x5421e0        FP_NO_HOST_CHECK        NO
3648    chrome.exe      0x5421e0        HOMEDRIVE       C:
3648    chrome.exe      0x5421e0        HOMEPATH        \Users\Rick
3648    chrome.exe      0x5421e0        LOCALAPPDATA    C:\Users\Rick\AppData\Local
3648    chrome.exe      0x5421e0        LOGONSERVER     \\WIN-LO6FAF3DTFE
3648    chrome.exe      0x5421e0        MpConfig_ProductAppDataPath     C:\ProgramData\Microsoft\Windows Defender
3648    chrome.exe      0x5421e0        MpConfig_ProductCodeName        AntiSpyware
3648    chrome.exe      0x5421e0        MpConfig_ProductPath    C:\Program Files\Windows Defender
3648    chrome.exe      0x5421e0        MpConfig_ProductUserAppDataPath C:\Users\Rick\AppData\Local\Microsoft\Windows Defender
3648    chrome.exe      0x5421e0        MpConfig_ReportingGUID  E7E10F56-B6E7-46CA-8174-0B336724C50A
3648    chrome.exe      0x5421e0        NUMBER_OF_PROCESSORS    2
3648    chrome.exe      0x5421e0        OS      Windows_NT
3648    chrome.exe      0x5421e0        Path    C:\Program Files (x86)\Google\Chrome\Application;C:\Windows\system32;C:\Windows;C:\Windows\System32\Wbem;C:\Windows\System32\WindowsPowerShell\v1.0\
3648    chrome.exe      0x5421e0        PATHEXT .COM;.EXE;.BAT;.CMD;.VBS;.VBE;.JS;.JSE;.WSF;.WSH;.MSC
3648    chrome.exe      0x5421e0        PROCESSOR_ARCHITECTURE  AMD64
3648    chrome.exe      0x5421e0        PROCESSOR_IDENTIFIER    Intel64 Family 6 Model 60 Stepping 3, GenuineIntel
3648    chrome.exe      0x5421e0        PROCESSOR_LEVEL 6
3648    chrome.exe      0x5421e0        PROCESSOR_REVISION      3c03
3648    chrome.exe      0x5421e0        ProgramData     C:\ProgramData
3648    chrome.exe      0x5421e0        ProgramFiles    C:\Program Files
3648    chrome.exe      0x5421e0        ProgramFiles(x86)       C:\Program Files (x86)
3648    chrome.exe      0x5421e0        ProgramW6432    C:\Program Files
3648    chrome.exe      0x5421e0        PSModulePath    C:\Windows\system32\WindowsPowerShell\v1.0\Modules\
3648    chrome.exe      0x5421e0        PUBLIC  C:\Users\Public
3648    chrome.exe      0x5421e0        SESSIONNAME     Console
3648    chrome.exe      0x5421e0        SystemDrive     C:
3648    chrome.exe      0x5421e0        SystemRoot      C:\Windows
3648    chrome.exe      0x5421e0        TEMP    C:\Users\Rick\AppData\Local\Temp
3648    chrome.exe      0x5421e0        TMP     C:\Users\Rick\AppData\Local\Temp
3648    chrome.exe      0x5421e0        USERDOMAIN      WIN-LO6FAF3DTFE
3648    chrome.exe      0x5421e0        USERNAME        Rick
3648    chrome.exe      0x5421e0        USERPROFILE     C:\Users\Rick
3648    chrome.exe      0x5421e0        windir  C:\Windows
3648    chrome.exe      0x5421e0        windows_tracing_flags   3
3648    chrome.exe      0x5421e0        windows_tracing_logfile C:\BVTBin\Tests\installpackage\csilogfile.log
1796    chrome.exe      0x2a21e0        ALLUSERSPROFILE C:\ProgramData
1796    chrome.exe      0x2a21e0        APPDATA C:\Users\Rick\AppData\Roaming
1796    chrome.exe      0x2a21e0        CHROME_CRASHPAD_PIPE_NAME       \\.\pipe\crashpad_4076_DAXLEIZKCFCTZZUS
1796    chrome.exe      0x2a21e0        CHROME_RESTART  Google Chrome|Whoa! Google Chrome has crashed. Relaunch now?|LEFT_TO_RIGHT
1796    chrome.exe      0x2a21e0        CommonProgramFiles      C:\Program Files\Common Files
1796    chrome.exe      0x2a21e0        CommonProgramFiles(x86) C:\Program Files (x86)\Common Files
1796    chrome.exe      0x2a21e0        CommonProgramW6432      C:\Program Files\Common Files
1796    chrome.exe      0x2a21e0        COMPUTERNAME    WIN-LO6FAF3DTFE
1796    chrome.exe      0x2a21e0        ComSpec C:\Windows\system32\cmd.exe
1796    chrome.exe      0x2a21e0        FP_NO_HOST_CHECK        NO
1796    chrome.exe      0x2a21e0        HOMEDRIVE       C:
1796    chrome.exe      0x2a21e0        HOMEPATH        \Users\Rick
1796    chrome.exe      0x2a21e0        LOCALAPPDATA    C:\Users\Rick\AppData\Local
1796    chrome.exe      0x2a21e0        LOGONSERVER     \\WIN-LO6FAF3DTFE
1796    chrome.exe      0x2a21e0        MpConfig_ProductAppDataPath     C:\ProgramData\Microsoft\Windows Defender
1796    chrome.exe      0x2a21e0        MpConfig_ProductCodeName        AntiSpyware
1796    chrome.exe      0x2a21e0        MpConfig_ProductPath    C:\Program Files\Windows Defender
1796    chrome.exe      0x2a21e0        MpConfig_ProductUserAppDataPath C:\Users\Rick\AppData\Local\Microsoft\Windows Defender
1796    chrome.exe      0x2a21e0        MpConfig_ReportingGUID  E7E10F56-B6E7-46CA-8174-0B336724C50A
1796    chrome.exe      0x2a21e0        NUMBER_OF_PROCESSORS    2
1796    chrome.exe      0x2a21e0        OS      Windows_NT
1796    chrome.exe      0x2a21e0        Path    C:\Program Files (x86)\Google\Chrome\Application;C:\Windows\system32;C:\Windows;C:\Windows\System32\Wbem;C:\Windows\System32\WindowsPowerShell\v1.0\
1796    chrome.exe      0x2a21e0        PATHEXT .COM;.EXE;.BAT;.CMD;.VBS;.VBE;.JS;.JSE;.WSF;.WSH;.MSC
1796    chrome.exe      0x2a21e0        PROCESSOR_ARCHITECTURE  AMD64
1796    chrome.exe      0x2a21e0        PROCESSOR_IDENTIFIER    Intel64 Family 6 Model 60 Stepping 3, GenuineIntel
1796    chrome.exe      0x2a21e0        PROCESSOR_LEVEL 6
1796    chrome.exe      0x2a21e0        PROCESSOR_REVISION      3c03
1796    chrome.exe      0x2a21e0        ProgramData     C:\ProgramData
1796    chrome.exe      0x2a21e0        ProgramFiles    C:\Program Files
1796    chrome.exe      0x2a21e0        ProgramFiles(x86)       C:\Program Files (x86)
1796    chrome.exe      0x2a21e0        ProgramW6432    C:\Program Files
1796    chrome.exe      0x2a21e0        PSModulePath    C:\Windows\system32\WindowsPowerShell\v1.0\Modules\
1796    chrome.exe      0x2a21e0        PUBLIC  C:\Users\Public
1796    chrome.exe      0x2a21e0        SESSIONNAME     Console
1796    chrome.exe      0x2a21e0        SystemDrive     C:
1796    chrome.exe      0x2a21e0        SystemRoot      C:\Windows
1796    chrome.exe      0x2a21e0        TEMP    C:\Users\Rick\AppData\Local\Temp
1796    chrome.exe      0x2a21e0        TMP     C:\Users\Rick\AppData\Local\Temp
1796    chrome.exe      0x2a21e0        USERDOMAIN      WIN-LO6FAF3DTFE
1796    chrome.exe      0x2a21e0        USERNAME        Rick
1796    chrome.exe      0x2a21e0        USERPROFILE     C:\Users\Rick
1796    chrome.exe      0x2a21e0        windir  C:\Windows
1796    chrome.exe      0x2a21e0        windows_tracing_flags   3
1796    chrome.exe      0x2a21e0        windows_tracing_logfile C:\BVTBin\Tests\installpackage\csilogfile.log
3496    Lavasoft.WCAss  0x311d90        ALLUSERSPROFILE C:\ProgramData
3496    Lavasoft.WCAss  0x311d90        APPDATA C:\Windows\system32\config\systemprofile\AppData\Roaming
3496    Lavasoft.WCAss  0x311d90        CommonProgramFiles      C:\Program Files\Common Files
3496    Lavasoft.WCAss  0x311d90        CommonProgramFiles(x86) C:\Program Files (x86)\Common Files
3496    Lavasoft.WCAss  0x311d90        CommonProgramW6432      C:\Program Files\Common Files
3496    Lavasoft.WCAss  0x311d90        COMPUTERNAME    WIN-LO6FAF3DTFE
3496    Lavasoft.WCAss  0x311d90        ComSpec C:\Windows\system32\cmd.exe
3496    Lavasoft.WCAss  0x311d90        FP_NO_HOST_CHECK        NO
3496    Lavasoft.WCAss  0x311d90        LOCALAPPDATA    C:\Windows\system32\config\systemprofile\AppData\Local
3496    Lavasoft.WCAss  0x311d90        NUMBER_OF_PROCESSORS    2
3496    Lavasoft.WCAss  0x311d90        OS      Windows_NT
3496    Lavasoft.WCAss  0x311d90        Path    C:\Windows\system32;C:\Windows;C:\Windows\System32\Wbem;C:\Windows\System32\WindowsPowerShell\v1.0\;
3496    Lavasoft.WCAss  0x311d90        PATHEXT .COM;.EXE;.BAT;.CMD;.VBS;.VBE;.JS;.JSE;.WSF;.WSH;.MSC
3496    Lavasoft.WCAss  0x311d90        PROCESSOR_ARCHITECTURE  AMD64
3496    Lavasoft.WCAss  0x311d90        PROCESSOR_IDENTIFIER    Intel64 Family 6 Model 60 Stepping 3, GenuineIntel
3496    Lavasoft.WCAss  0x311d90        PROCESSOR_LEVEL 6
3496    Lavasoft.WCAss  0x311d90        PROCESSOR_REVISION      3c03
3496    Lavasoft.WCAss  0x311d90        ProgramData     C:\ProgramData
3496    Lavasoft.WCAss  0x311d90        ProgramFiles    C:\Program Files
3496    Lavasoft.WCAss  0x311d90        ProgramFiles(x86)       C:\Program Files (x86)
3496    Lavasoft.WCAss  0x311d90        ProgramW6432    C:\Program Files
3496    Lavasoft.WCAss  0x311d90        PSModulePath    C:\Windows\system32\WindowsPowerShell\v1.0\Modules\
3496    Lavasoft.WCAss  0x311d90        PUBLIC  C:\Users\Public
3496    Lavasoft.WCAss  0x311d90        SystemDrive     C:
3496    Lavasoft.WCAss  0x311d90        SystemRoot      C:\Windows
3496    Lavasoft.WCAss  0x311d90        TEMP    C:\Windows\TEMP
3496    Lavasoft.WCAss  0x311d90        TMP     C:\Windows\TEMP
3496    Lavasoft.WCAss  0x311d90        USERDOMAIN      WORKGROUP
3496    Lavasoft.WCAss  0x311d90        USERNAME        WIN-LO6FAF3DTFE$
3496    Lavasoft.WCAss  0x311d90        USERPROFILE     C:\Windows\system32\config\systemprofile
3496    Lavasoft.WCAss  0x311d90        windir  C:\Windows
3496    Lavasoft.WCAss  0x311d90        windows_tracing_flags   3
3496    Lavasoft.WCAss  0x311d90        windows_tracing_logfile C:\BVTBin\Tests\installpackage\csilogfile.log
3856    WebCompanion.e  0x151de0        ALLUSERSPROFILE C:\ProgramData
3856    WebCompanion.e  0x151de0        APPDATA C:\Windows\system32\config\systemprofile\AppData\Roaming
3856    WebCompanion.e  0x151de0        CommonProgramFiles      C:\Program Files\Common Files
3856    WebCompanion.e  0x151de0        CommonProgramFiles(x86) C:\Program Files (x86)\Common Files
3856    WebCompanion.e  0x151de0        CommonProgramW6432      C:\Program Files\Common Files
3856    WebCompanion.e  0x151de0        COMPUTERNAME    WIN-LO6FAF3DTFE
3856    WebCompanion.e  0x151de0        ComSpec C:\Windows\system32\cmd.exe
3856    WebCompanion.e  0x151de0        FP_NO_HOST_CHECK        NO
3856    WebCompanion.e  0x151de0        LOCALAPPDATA    C:\Windows\system32\config\systemprofile\AppData\Local
3856    WebCompanion.e  0x151de0        NUMBER_OF_PROCESSORS    2
3856    WebCompanion.e  0x151de0        OS      Windows_NT
3856    WebCompanion.e  0x151de0        Path    C:\Windows\system32;C:\Windows;C:\Windows\System32\Wbem;C:\Windows\System32\WindowsPowerShell\v1.0\;
3856    WebCompanion.e  0x151de0        PATHEXT .COM;.EXE;.BAT;.CMD;.VBS;.VBE;.JS;.JSE;.WSF;.WSH;.MSC
3856    WebCompanion.e  0x151de0        PROCESSOR_ARCHITECTURE  AMD64
3856    WebCompanion.e  0x151de0        PROCESSOR_IDENTIFIER    Intel64 Family 6 Model 60 Stepping 3, GenuineIntel
3856    WebCompanion.e  0x151de0        PROCESSOR_LEVEL 6
3856    WebCompanion.e  0x151de0        PROCESSOR_REVISION      3c03
3856    WebCompanion.e  0x151de0        ProgramData     C:\ProgramData
3856    WebCompanion.e  0x151de0        ProgramFiles    C:\Program Files
3856    WebCompanion.e  0x151de0        ProgramFiles(x86)       C:\Program Files (x86)
3856    WebCompanion.e  0x151de0        ProgramW6432    C:\Program Files
3856    WebCompanion.e  0x151de0        PSModulePath    C:\Windows\system32\WindowsPowerShell\v1.0\Modules\
3856    WebCompanion.e  0x151de0        PUBLIC  C:\Users\Public
3856    WebCompanion.e  0x151de0        SystemDrive     C:
3856    WebCompanion.e  0x151de0        SystemRoot      C:\Windows
3856    WebCompanion.e  0x151de0        TEMP    C:\Windows\TEMP
3856    WebCompanion.e  0x151de0        TMP     C:\Windows\TEMP
3856    WebCompanion.e  0x151de0        USERDOMAIN      WORKGROUP
3856    WebCompanion.e  0x151de0        USERNAME        WIN-LO6FAF3DTFE$
3856    WebCompanion.e  0x151de0        USERPROFILE     C:\Windows\system32\config\systemprofile
3856    WebCompanion.e  0x151de0        windir  C:\Windows
3856    WebCompanion.e  0x151de0        windows_tracing_flags   3
3856    WebCompanion.e  0x151de0        windows_tracing_logfile C:\BVTBin\Tests\installpackage\csilogfile.log
3304    notepad.exe     0x301dd0        ALLUSERSPROFILE C:\ProgramData
3304    notepad.exe     0x301dd0        APPDATA C:\Users\Rick\AppData\Roaming
3304    notepad.exe     0x301dd0        CommonProgramFiles      C:\Program Files\Common Files
3304    notepad.exe     0x301dd0        CommonProgramFiles(x86) C:\Program Files (x86)\Common Files
3304    notepad.exe     0x301dd0        CommonProgramW6432      C:\Program Files\Common Files
3304    notepad.exe     0x301dd0        COMPUTERNAME    WIN-LO6FAF3DTFE
3304    notepad.exe     0x301dd0        ComSpec C:\Windows\system32\cmd.exe
3304    notepad.exe     0x301dd0        FP_NO_HOST_CHECK        NO
3304    notepad.exe     0x301dd0        HOMEDRIVE       C:
3304    notepad.exe     0x301dd0        HOMEPATH        \Users\Rick
3304    notepad.exe     0x301dd0        LOCALAPPDATA    C:\Users\Rick\AppData\Local
3304    notepad.exe     0x301dd0        LOGONSERVER     \\WIN-LO6FAF3DTFE
3304    notepad.exe     0x301dd0        NUMBER_OF_PROCESSORS    2
3304    notepad.exe     0x301dd0        OS      Windows_NT
3304    notepad.exe     0x301dd0        Path    C:\Windows\system32;C:\Windows;C:\Windows\System32\Wbem;C:\Windows\System32\WindowsPowerShell\v1.0\
3304    notepad.exe     0x301dd0        PATHEXT .COM;.EXE;.BAT;.CMD;.VBS;.VBE;.JS;.JSE;.WSF;.WSH;.MSC
3304    notepad.exe     0x301dd0        PROCESSOR_ARCHITECTURE  AMD64
3304    notepad.exe     0x301dd0        PROCESSOR_IDENTIFIER    Intel64 Family 6 Model 60 Stepping 3, GenuineIntel
3304    notepad.exe     0x301dd0        PROCESSOR_LEVEL 6
3304    notepad.exe     0x301dd0        PROCESSOR_REVISION      3c03
3304    notepad.exe     0x301dd0        ProgramData     C:\ProgramData
3304    notepad.exe     0x301dd0        ProgramFiles    C:\Program Files
3304    notepad.exe     0x301dd0        ProgramFiles(x86)       C:\Program Files (x86)
3304    notepad.exe     0x301dd0        ProgramW6432    C:\Program Files
3304    notepad.exe     0x301dd0        PSModulePath    C:\Windows\system32\WindowsPowerShell\v1.0\Modules\
3304    notepad.exe     0x301dd0        PUBLIC  C:\Users\Public
3304    notepad.exe     0x301dd0        SESSIONNAME     Console
3304    notepad.exe     0x301dd0        SystemDrive     C:
3304    notepad.exe     0x301dd0        SystemRoot      C:\Windows
3304    notepad.exe     0x301dd0        TEMP    C:\Users\Rick\AppData\Local\Temp
3304    notepad.exe     0x301dd0        TMP     C:\Users\Rick\AppData\Local\Temp
3304    notepad.exe     0x301dd0        USERDOMAIN      WIN-LO6FAF3DTFE
3304    notepad.exe     0x301dd0        USERNAME        Rick
3304    notepad.exe     0x301dd0        USERPROFILE     C:\Users\Rick
3304    notepad.exe     0x301dd0        windir  C:\Windows
3304    notepad.exe     0x301dd0        windows_tracing_flags   3
3304    notepad.exe     0x301dd0        windows_tracing_logfile C:\BVTBin\Tests\installpackage\csilogfile.log
2420    conhost.exe     0x1a18f0        ComSpec C:\Windows\system32\cmd.exe
2420    conhost.exe     0x1a18f0        FP_NO_HOST_CHECK        NO
2420    conhost.exe     0x1a18f0        NUMBER_OF_PROCESSORS    2
2420    conhost.exe     0x1a18f0        OS      Windows_NT
2420    conhost.exe     0x1a18f0        Path    C:\Windows\system32;C:\Windows;C:\Windows\System32\Wbem;C:\Windows\System32\WindowsPowerShell\v1.0\
2420    conhost.exe     0x1a18f0        PATHEXT .COM;.EXE;.BAT;.CMD;.VBS;.VBE;.JS;.JSE;.WSF;.WSH;.MSC
2420    conhost.exe     0x1a18f0        PROCESSOR_ARCHITECTURE  AMD64
2420    conhost.exe     0x1a18f0        PROCESSOR_IDENTIFIER    Intel64 Family 6 Model 60 Stepping 3, GenuineIntel
2420    conhost.exe     0x1a18f0        PROCESSOR_LEVEL 6
2420    conhost.exe     0x1a18f0        PROCESSOR_REVISION      3c03
2420    conhost.exe     0x1a18f0        PSModulePath    C:\Windows\system32\WindowsPowerShell\v1.0\Modules\
2420    conhost.exe     0x1a18f0        SystemDrive     C:
2420    conhost.exe     0x1a18f0        SystemRoot      C:\Windows
2420    conhost.exe     0x1a18f0        TEMP    C:\Windows\TEMP
2420    conhost.exe     0x1a18f0        TMP     C:\Windows\TEMP
2420    conhost.exe     0x1a18f0        USERNAME        SYSTEM
2420    conhost.exe     0x1a18f0        windir  C:\Windows
2420    conhost.exe     0x1a18f0        windows_tracing_flags   3
2420    conhost.exe     0x1a18f0        windows_tracing_logfile C:\BVTBin\Tests\installpackage\csilogfile.log
```


# windows.envars.Envars 分析

## 1. 執行指令

```bash
.\vol.exe -f .\OtterCTF.vmem windows.envars.Envars
```

---

## 2. Plugin 功能簡述

`windows.envars.Envars` 用來列出各 Process 的環境變數。

它可以協助確認：

* Process 所屬使用者
* 使用者目錄
* TEMP / TMP 暫存路徑
* APPDATA / LOCALAPPDATA 路徑
* 系統名稱
* 系統路徑與 PowerShell 路徑
* Process 是在使用者環境還是 SYSTEM 環境執行

---

## 3. 重要欄位簡單說明

| 欄位             | 說明                         |
| -------------- | -------------------------- |
| `COMPUTERNAME` | 電腦名稱                       |
| `USERNAME`     | 執行該 Process 的使用者           |
| `USERPROFILE`  | 使用者資料夾                     |
| `HOMEPATH`     | 使用者家目錄路徑                   |
| `APPDATA`      | 使用者 Roaming AppData 路徑     |
| `LOCALAPPDATA` | 使用者 Local AppData 路徑       |
| `TEMP` / `TMP` | 暫存資料夾                      |
| `Path`         | Process 可搜尋執行檔的路徑          |
| `SESSIONNAME`  | 使用者登入 Session，例如 `Console` |

---

## 4. 系統環境資訊

本次結果中，多個 Process 顯示相同系統資訊：

| 項目              | 結果                                                    |
| --------------- | ----------------------------------------------------- |
| 電腦名稱            | `WIN-LO6FAF3DTFE`                                     |
| 作業系統            | `Windows_NT`                                          |
| 系統磁碟            | `C:`                                                  |
| 系統目錄            | `C:\Windows`                                          |
| 處理器架構           | `AMD64`                                               |
| CPU 數量          | `2`                                                   |
| PowerShell 模組路徑 | `C:\Windows\system32\WindowsPowerShell\v1.0\Modules\` |

這些資訊與前面 `windows.info.Info`、`pslist` 的分析結果一致。

---

## 5. 使用者環境確認

本次最重要的使用者是：

```text
Rick
```

多個使用者層 Process 都顯示：

```text
USERNAME = Rick
USERPROFILE = C:\Users\Rick
HOMEPATH = \Users\Rick
APPDATA = C:\Users\Rick\AppData\Roaming
LOCALAPPDATA = C:\Users\Rick\AppData\Local
TEMP = C:\Users\Rick\AppData\Local\Temp
```

代表這些 Process 是在 `Rick` 使用者環境下執行。

---

## 6. 重要 Process 環境整理

|  PID | Process            | USERNAME           | USERPROFILE / TEMP                         | 判斷                   |
| ---: | ------------------ | ------------------ | ------------------------------------------ | -------------------- |
| 2728 | `explorer.exe`     | `Rick`             | `C:\Users\Rick`                            | 使用者桌面環境              |
| 2836 | `BitTorrent.exe`   | `Rick`             | `C:\Users\Rick\AppData\Local\Temp`         | 使用者下載活動相關            |
|  708 | `LunarMS.exe`      | `Rick`             | `C:\Users\Rick\AppData\Local\Temp`         | 使用者執行的程式             |
| 3820 | `Rick And Morty`   | `Rick`             | `C:\Users\Rick\AppData\Local\Temp`         | 高度可疑程式               |
| 3720 | `vmware-tray.exe`  | `Rick`             | `C:\Users\Rick\AppData\Local\Temp`         | 可疑子行程                |
| 3304 | `notepad.exe`      | `Rick`             | `C:\Users\Rick\AppData\Local\Temp`         | 開啟 Flag 檔案           |
| 3880 | `WebCompanionIn`   | `WIN-LO6FAF3DTFE$` | `C:\Windows\system32\config\systemprofile` | SYSTEM / service 類環境 |
| 3496 | `Lavasoft.WCAss`   | `WIN-LO6FAF3DTFE$` | `C:\Windows\system32\config\systemprofile` | WebCompanion 服務      |
| 3856 | `WebCompanion.exe` | `WIN-LO6FAF3DTFE$` | `C:\Windows\system32\config\systemprofile` | WebCompanion 更新行為    |

---

## 7. 關鍵發現

### 7.1 使用者 Rick 是主要操作帳號

`explorer.exe`、`BitTorrent.exe`、`LunarMS.exe`、`Rick And Morty`、`notepad.exe` 都在 `Rick` 的使用者環境下執行。

這代表本次可疑活動主要與使用者：

```text
Rick
```

有關。

---

### 7.2 Rick And Morty 執行於 Rick 使用者環境

`Rick And Morty` 的環境變數顯示：

```text
USERNAME = Rick
USERPROFILE = C:\Users\Rick
TEMP = C:\Users\Rick\AppData\Local\Temp
SESSIONNAME = Console
```

這代表該可疑程式是在使用者登入桌面環境中執行，而不是系統服務自動啟動。

搭配前面 `cmdline` 結果：

```text
C:\Torrents\Rick And Morty season 1 download.exe
```

可判斷此程式很可能是使用者下載後執行的可疑 EXE。

---

### 7.3 vmware-tray.exe 也在 Rick 使用者環境下

`vmware-tray.exe` 的環境變數同樣顯示 `USERNAME = Rick`，而且 TEMP 指向：

```text
C:\Users\Rick\AppData\Local\Temp
```

搭配前面 `cmdline` 的路徑：

```text
C:\Users\Rick\AppData\Local\Temp\RarSFX0\vmware-tray.exe
```

可以判斷它與 `Rick And Morty` 的可疑執行鏈有關。

---

### 7.4 WebCompanionIn 屬於 SYSTEM 類環境

`WebCompanionIn` 的環境變數顯示：

```text
USERNAME = WIN-LO6FAF3DTFE$
USERPROFILE = C:\Windows\system32\config\systemprofile
TEMP = C:\Windows\TEMP
```

這代表它不是一般 Rick 使用者環境，而是偏向系統或服務環境。

搭配前面 `pstree` 中 `WebCompanionIn → sc.exe`，可推測它可能正在進行服務建立、更新或操作。

---

### 7.5 notepad.exe 確認與 Rick 使用者有關

`notepad.exe` 的環境變數顯示：

```text
USERNAME = Rick
USERPROFILE = C:\Users\Rick
```

前面 `cmdline` 已顯示它開啟：

```text
C:\Users\Rick\Desktop\Flag.txt.WINDOWS
```

因此可以確認 `Flag.txt.WINDOWS` 與 Rick 使用者桌面環境有關。

---

## 8. 本次 Envars 鑑識重點

本次 `envars` 的主要價值是確認可疑 Process 的執行環境。

重要發現如下：

1. 主要使用者帳號為 `Rick`。
2. 電腦名稱為 `WIN-LO6FAF3DTFE`。
3. `Rick And Morty` 是在 Rick 使用者環境下執行。
4. `vmware-tray.exe` 也在 Rick 使用者環境下執行，且與 Temp 路徑有關。
5. `notepad.exe` 在 Rick 使用者環境下執行，與 `Flag.txt.WINDOWS` 線索吻合。
6. `WebCompanionIn` 與 `Lavasoft.WCAss` 則偏向 system profile / service 環境。

---

## 9. 後續建議分析

### 9.1 搜尋 Rick 使用者桌面 Flag 檔案

```bash
.\vol.exe -f .\OtterCTF.vmem windows.filescan.FileScan > filescan.txt
findstr /i "Flag" filescan.txt
findstr /i "Desktop" filescan.txt
```

### 9.2 分析 Rick And Morty

```bash
.\vol.exe -f .\OtterCTF.vmem windows.dlllist.DllList --pid 3820
.\vol.exe -f .\OtterCTF.vmem windows.malfind.Malfind --pid 3820
```

### 9.3 分析可疑 Temp 子行程

```bash
.\vol.exe -f .\OtterCTF.vmem windows.dlllist.DllList --pid 3720
.\vol.exe -f .\OtterCTF.vmem windows.malfind.Malfind --pid 3720
```

### 9.4 分析網路連線

```bash
.\vol.exe -f .\OtterCTF.vmem windows.netscan.NetScan
```

---

## 10. 報告用結論

本次使用 `windows.envars.Envars` 分析各 Process 的環境變數。

結果顯示，主要使用者帳號為 `Rick`，使用者目錄為：

```text
C:\Users\Rick
```

其中 `explorer.exe`、`BitTorrent.exe`、`LunarMS.exe`、`Rick And Morty`、`vmware-tray.exe` 與 `notepad.exe` 都在 Rick 使用者環境下執行。這表示本次可疑活動主要發生在 Rick 的登入桌面環境中。

`Rick And Morty` 的環境變數顯示其使用 `Rick` 使用者的 TEMP、APPDATA 與 USERPROFILE，搭配前面 `cmdline` 中的 `C:\Torrents\Rick And Morty season 1 download.exe`，可判斷該程式很可能是使用者下載並執行的可疑檔案。

另外，`WebCompanionIn`、`Lavasoft.WCAss` 與 `WebCompanion.exe` 則顯示為 `WIN-LO6FAF3DTFE$` 與 system profile 環境，代表其行為較接近服務或系統層級操作。這與前面觀察到的 `WebCompanionIn → sc.exe` 服務操作線索一致。

綜合判斷，`envars` 結果確認了可疑程式的使用者環境，並補強 `Rick` 使用者、`Temp` 目錄、`Flag.txt.WINDOWS` 與 `WebCompanion` 服務行為之間的關聯。

---

## 11. 簡短結論

`windows.envars.Envars` 顯示本次主要使用者為：

```text
Rick
```

重要可疑環境關係為：

```text
Rick → BitTorrent.exe
Rick → Rick And Morty
Rick → vmware-tray.exe
Rick → notepad.exe → Flag.txt.WINDOWS
```

其中 `Rick And Morty` 和 `vmware-tray.exe` 都使用 Rick 的使用者環境與 Temp 路徑，需列為後續分析重點。

`WebCompanionIn` 則屬於 system profile 環境，可能與服務操作有關。
