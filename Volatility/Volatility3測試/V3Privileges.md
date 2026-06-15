# 測試內容

- .\vol.exe -f .\OtterCTF.vmem windows.privileges.Privs

```
:\Forensic\G140A006\VolatilityWorkbench>.\vol.exe -f .\OtterCTF.vmem windows.privileges.Privs
Volatility 3 Framework 2.5.0
Progress:  100.00               PDB scanning finished
PID     Process Value   Privilege       Attributes      Description

4       System  2       SeCreateTokenPrivilege  Present Create a token object
4       System  3       SeAssignPrimaryTokenPrivilege   Present Replace a process-level token
4       System  4       SeLockMemoryPrivilege   Present,Enabled,Default Lock pages in memory
4       System  5       SeIncreaseQuotaPrivilege        Present Increase quotas
4       System  6       SeMachineAccountPrivilege               Add workstations to the domain
4       System  7       SeTcbPrivilege  Present,Enabled,Default Act as part of the operating system
4       System  8       SeSecurityPrivilege     Present Manage auditing and security log
4       System  9       SeTakeOwnershipPrivilege        Present Take ownership of files/objects
4       System  10      SeLoadDriverPrivilege   Present Load and unload device drivers
4       System  11      SeSystemProfilePrivilege        Present,Enabled,Default Profile system performance
4       System  12      SeSystemtimePrivilege   Present Change the system time
4       System  13      SeProfileSingleProcessPrivilege Present,Enabled,Default Profile a single process
4       System  14      SeIncreaseBasePriorityPrivilege Present,Enabled,Default Increase scheduling priority
4       System  15      SeCreatePagefilePrivilege       Present,Enabled,Default Create a pagefile
4       System  16      SeCreatePermanentPrivilege      Present,Enabled,Default Create permanent shared objects
4       System  17      SeBackupPrivilege       Present Backup files and directories
4       System  18      SeRestorePrivilege      Present Restore files and directories
4       System  19      SeShutdownPrivilege     Present Shut down the system
4       System  20      SeDebugPrivilege        Present,Enabled,Default Debug programs
4       System  21      SeAuditPrivilege        Present,Enabled,Default Generate security audits
4       System  22      SeSystemEnvironmentPrivilege    Present Edit firmware environment values
4       System  23      SeChangeNotifyPrivilege Present,Enabled,Default Receive notifications of changes to files or directories
4       System  24      SeRemoteShutdownPrivilege               Force shutdown from a remote system
4       System  25      SeUndockPrivilege       Present Remove computer from docking station
4       System  26      SeSyncAgentPrivilege            Synch directory service data
4       System  27      SeEnableDelegationPrivilege             Enable user accounts to be trusted for delegation
4       System  28      SeManageVolumePrivilege Present Manage the files on a volume
4       System  29      SeImpersonatePrivilege  Present,Enabled,Default Impersonate a client after authentication
4       System  30      SeCreateGlobalPrivilege Present,Enabled,Default Create global objects
4       System  31      SeTrustedCredManAccessPrivilege Present Access Credential Manager as a trusted caller
4       System  32      SeRelabelPrivilege      Present Modify the mandatory integrity level of an object
4       System  33      SeIncreaseWorkingSetPrivilege   Present,Enabled,Default Allocate more memory for user applications
4       System  34      SeTimeZonePrivilege     Present,Enabled,Default Adjust the time zone of the computer's internal clock
4       System  35      SeCreateSymbolicLinkPrivilege   Present,Enabled,Default Required to create a symbolic link
4       System  36      SeDelegateSessionUserImpersonatePrivilege               Obtain an impersonation token for another user in the same session.
260     smss.exe        2       SeCreateTokenPrivilege  Present Create a token object
260     smss.exe        3       SeAssignPrimaryTokenPrivilege   Present Replace a process-level token
260     smss.exe        4       SeLockMemoryPrivilege   Present,Enabled,Default Lock pages in memory
260     smss.exe        5       SeIncreaseQuotaPrivilege        Present Increase quotas
260     smss.exe        6       SeMachineAccountPrivilege               Add workstations to the domain
260     smss.exe        7       SeTcbPrivilege  Present,Enabled,Default Act as part of the operating system
260     smss.exe        8       SeSecurityPrivilege     Present Manage auditing and security log
260     smss.exe        9       SeTakeOwnershipPrivilege        Present Take ownership of files/objects
260     smss.exe        10      SeLoadDriverPrivilege   Present Load and unload device drivers
260     smss.exe        11      SeSystemProfilePrivilege        Present,Enabled,Default Profile system performance
260     smss.exe        12      SeSystemtimePrivilege   Present Change the system time
260     smss.exe        13      SeProfileSingleProcessPrivilege Present,Enabled,Default Profile a single process
260     smss.exe        14      SeIncreaseBasePriorityPrivilege Present,Enabled,Default Increase scheduling priority
260     smss.exe        15      SeCreatePagefilePrivilege       Present,Enabled,Default Create a pagefile
260     smss.exe        16      SeCreatePermanentPrivilege      Present,Enabled,Default Create permanent shared objects
260     smss.exe        17      SeBackupPrivilege       Present Backup files and directories
260     smss.exe        18      SeRestorePrivilege      Present Restore files and directories
260     smss.exe        19      SeShutdownPrivilege     Present Shut down the system
260     smss.exe        20      SeDebugPrivilege        Present,Enabled,Default Debug programs
260     smss.exe        21      SeAuditPrivilege        Present,Enabled,Default Generate security audits
260     smss.exe        22      SeSystemEnvironmentPrivilege    Present Edit firmware environment values
260     smss.exe        23      SeChangeNotifyPrivilege Present,Enabled,Default Receive notifications of changes to files or directories
260     smss.exe        24      SeRemoteShutdownPrivilege               Force shutdown from a remote system
260     smss.exe        25      SeUndockPrivilege       Present Remove computer from docking station
260     smss.exe        26      SeSyncAgentPrivilege            Synch directory service data
260     smss.exe        27      SeEnableDelegationPrivilege             Enable user accounts to be trusted for delegation
260     smss.exe        28      SeManageVolumePrivilege Present Manage the files on a volume
260     smss.exe        29      SeImpersonatePrivilege  Present,Enabled,Default Impersonate a client after authentication
260     smss.exe        30      SeCreateGlobalPrivilege Present,Enabled,Default Create global objects
260     smss.exe        31      SeTrustedCredManAccessPrivilege Present Access Credential Manager as a trusted caller
260     smss.exe        32      SeRelabelPrivilege      Present Modify the mandatory integrity level of an object
260     smss.exe        33      SeIncreaseWorkingSetPrivilege   Present,Enabled,Default Allocate more memory for user applications
260     smss.exe        34      SeTimeZonePrivilege     Present,Enabled,Default Adjust the time zone of the computer's internal clock
260     smss.exe        35      SeCreateSymbolicLinkPrivilege   Present,Enabled,Default Required to create a symbolic link
260     smss.exe        36      SeDelegateSessionUserImpersonatePrivilege               Obtain an impersonation token for another user in the same session.
348     csrss.exe       2       SeCreateTokenPrivilege  Present Create a token object
348     csrss.exe       3       SeAssignPrimaryTokenPrivilege   Present Replace a process-level token
348     csrss.exe       4       SeLockMemoryPrivilege   Present,Enabled,Default Lock pages in memory
348     csrss.exe       5       SeIncreaseQuotaPrivilege        Present Increase quotas
348     csrss.exe       6       SeMachineAccountPrivilege               Add workstations to the domain
348     csrss.exe       7       SeTcbPrivilege  Present,Enabled,Default Act as part of the operating system
348     csrss.exe       8       SeSecurityPrivilege     Present Manage auditing and security log
348     csrss.exe       9       SeTakeOwnershipPrivilege        Present Take ownership of files/objects
348     csrss.exe       10      SeLoadDriverPrivilege   Present Load and unload device drivers
348     csrss.exe       11      SeSystemProfilePrivilege        Present,Enabled,Default Profile system performance
348     csrss.exe       12      SeSystemtimePrivilege   Present Change the system time
348     csrss.exe       13      SeProfileSingleProcessPrivilege Present,Enabled,Default Profile a single process
348     csrss.exe       14      SeIncreaseBasePriorityPrivilege Present,Enabled,Default Increase scheduling priority
348     csrss.exe       15      SeCreatePagefilePrivilege       Present,Enabled,Default Create a pagefile
348     csrss.exe       16      SeCreatePermanentPrivilege      Present,Enabled,Default Create permanent shared objects
348     csrss.exe       17      SeBackupPrivilege       Present Backup files and directories
348     csrss.exe       18      SeRestorePrivilege      Present Restore files and directories
348     csrss.exe       19      SeShutdownPrivilege     Present Shut down the system
348     csrss.exe       20      SeDebugPrivilege        Present,Enabled,Default Debug programs
348     csrss.exe       21      SeAuditPrivilege        Present,Enabled,Default Generate security audits
348     csrss.exe       22      SeSystemEnvironmentPrivilege    Present Edit firmware environment values
348     csrss.exe       23      SeChangeNotifyPrivilege Present,Enabled,Default Receive notifications of changes to files or directories
348     csrss.exe       24      SeRemoteShutdownPrivilege               Force shutdown from a remote system
348     csrss.exe       25      SeUndockPrivilege       Present Remove computer from docking station
348     csrss.exe       26      SeSyncAgentPrivilege            Synch directory service data
348     csrss.exe       27      SeEnableDelegationPrivilege             Enable user accounts to be trusted for delegation
348     csrss.exe       28      SeManageVolumePrivilege Present Manage the files on a volume
348     csrss.exe       29      SeImpersonatePrivilege  Present,Enabled,Default Impersonate a client after authentication
348     csrss.exe       30      SeCreateGlobalPrivilege Present,Enabled,Default Create global objects
348     csrss.exe       31      SeTrustedCredManAccessPrivilege         Access Credential Manager as a trusted caller
348     csrss.exe       32      SeRelabelPrivilege      Present Modify the mandatory integrity level of an object
348     csrss.exe       33      SeIncreaseWorkingSetPrivilege   Present,Enabled,Default Allocate more memory for user applications
348     csrss.exe       34      SeTimeZonePrivilege     Present,Enabled,Default Adjust the time zone of the computer's internal clock
348     csrss.exe       35      SeCreateSymbolicLinkPrivilege   Present,Enabled,Default Required to create a symbolic link
348     csrss.exe       36      SeDelegateSessionUserImpersonatePrivilege               Obtain an impersonation token for another user in the same session.
388     csrss.exe       2       SeCreateTokenPrivilege  Present Create a token object
388     csrss.exe       3       SeAssignPrimaryTokenPrivilege   Present Replace a process-level token
388     csrss.exe       4       SeLockMemoryPrivilege   Present,Enabled,Default Lock pages in memory
388     csrss.exe       5       SeIncreaseQuotaPrivilege        Present Increase quotas
388     csrss.exe       6       SeMachineAccountPrivilege               Add workstations to the domain
388     csrss.exe       7       SeTcbPrivilege  Present,Enabled,Default Act as part of the operating system
388     csrss.exe       8       SeSecurityPrivilege     Present Manage auditing and security log
388     csrss.exe       9       SeTakeOwnershipPrivilege        Present Take ownership of files/objects
388     csrss.exe       10      SeLoadDriverPrivilege   Present Load and unload device drivers
388     csrss.exe       11      SeSystemProfilePrivilege        Present,Enabled,Default Profile system performance
388     csrss.exe       12      SeSystemtimePrivilege   Present Change the system time
388     csrss.exe       13      SeProfileSingleProcessPrivilege Present,Enabled,Default Profile a single process
388     csrss.exe       14      SeIncreaseBasePriorityPrivilege Present,Enabled,Default Increase scheduling priority
388     csrss.exe       15      SeCreatePagefilePrivilege       Present,Enabled,Default Create a pagefile
388     csrss.exe       16      SeCreatePermanentPrivilege      Present,Enabled,Default Create permanent shared objects
388     csrss.exe       17      SeBackupPrivilege       Present Backup files and directories
388     csrss.exe       18      SeRestorePrivilege      Present Restore files and directories
388     csrss.exe       19      SeShutdownPrivilege     Present Shut down the system
388     csrss.exe       20      SeDebugPrivilege        Present,Enabled,Default Debug programs
388     csrss.exe       21      SeAuditPrivilege        Present,Enabled,Default Generate security audits
388     csrss.exe       22      SeSystemEnvironmentPrivilege    Present Edit firmware environment values
388     csrss.exe       23      SeChangeNotifyPrivilege Present,Enabled,Default Receive notifications of changes to files or directories
388     csrss.exe       24      SeRemoteShutdownPrivilege               Force shutdown from a remote system
388     csrss.exe       25      SeUndockPrivilege       Present Remove computer from docking station
388     csrss.exe       26      SeSyncAgentPrivilege            Synch directory service data
388     csrss.exe       27      SeEnableDelegationPrivilege             Enable user accounts to be trusted for delegation
388     csrss.exe       28      SeManageVolumePrivilege Present Manage the files on a volume
388     csrss.exe       29      SeImpersonatePrivilege  Present,Enabled,Default Impersonate a client after authentication
388     csrss.exe       30      SeCreateGlobalPrivilege Present,Enabled,Default Create global objects
388     csrss.exe       31      SeTrustedCredManAccessPrivilege         Access Credential Manager as a trusted caller
388     csrss.exe       32      SeRelabelPrivilege      Present Modify the mandatory integrity level of an object
388     csrss.exe       33      SeIncreaseWorkingSetPrivilege   Present,Enabled,Default Allocate more memory for user applications
388     csrss.exe       34      SeTimeZonePrivilege     Present,Enabled,Default Adjust the time zone of the computer's internal clock
388     csrss.exe       35      SeCreateSymbolicLinkPrivilege   Present,Enabled,Default Required to create a symbolic link
388     csrss.exe       36      SeDelegateSessionUserImpersonatePrivilege               Obtain an impersonation token for another user in the same session.
396     wininit.exe     2       SeCreateTokenPrivilege          Create a token object
396     wininit.exe     3       SeAssignPrimaryTokenPrivilege   Present Replace a process-level token
396     wininit.exe     4       SeLockMemoryPrivilege   Default Lock pages in memory
396     wininit.exe     5       SeIncreaseQuotaPrivilege        Present Increase quotas
396     wininit.exe     6       SeMachineAccountPrivilege               Add workstations to the domain
396     wininit.exe     7       SeTcbPrivilege  Present,Enabled,Default Act as part of the operating system
396     wininit.exe     8       SeSecurityPrivilege     Present Manage auditing and security log
396     wininit.exe     9       SeTakeOwnershipPrivilege        Present Take ownership of files/objects
396     wininit.exe     10      SeLoadDriverPrivilege   Present Load and unload device drivers
396     wininit.exe     11      SeSystemProfilePrivilege        Default Profile system performance
396     wininit.exe     12      SeSystemtimePrivilege           Change the system time
396     wininit.exe     13      SeProfileSingleProcessPrivilege Default Profile a single process
396     wininit.exe     14      SeIncreaseBasePriorityPrivilege Present,Enabled,Default Increase scheduling priority
396     wininit.exe     15      SeCreatePagefilePrivilege       Default Create a pagefile
396     wininit.exe     16      SeCreatePermanentPrivilege      Present,Enabled,Default Create permanent shared objects
396     wininit.exe     17      SeBackupPrivilege       Present Backup files and directories
396     wininit.exe     18      SeRestorePrivilege      Present Restore files and directories
396     wininit.exe     19      SeShutdownPrivilege     Present Shut down the system
396     wininit.exe     20      SeDebugPrivilege        Present,Enabled,Default Debug programs
396     wininit.exe     21      SeAuditPrivilege        Present,Enabled,Default Generate security audits
396     wininit.exe     22      SeSystemEnvironmentPrivilege    Present Edit firmware environment values
396     wininit.exe     23      SeChangeNotifyPrivilege Present,Enabled,Default Receive notifications of changes to files or directories
396     wininit.exe     24      SeRemoteShutdownPrivilege               Force shutdown from a remote system
396     wininit.exe     25      SeUndockPrivilege       Present Remove computer from docking station
396     wininit.exe     26      SeSyncAgentPrivilege            Synch directory service data
396     wininit.exe     27      SeEnableDelegationPrivilege             Enable user accounts to be trusted for delegation
396     wininit.exe     28      SeManageVolumePrivilege Present Manage the files on a volume
396     wininit.exe     29      SeImpersonatePrivilege  Present,Enabled,Default Impersonate a client after authentication
396     wininit.exe     30      SeCreateGlobalPrivilege Present,Enabled,Default Create global objects
396     wininit.exe     31      SeTrustedCredManAccessPrivilege         Access Credential Manager as a trusted caller
396     wininit.exe     32      SeRelabelPrivilege              Modify the mandatory integrity level of an object
396     wininit.exe     33      SeIncreaseWorkingSetPrivilege   Default Allocate more memory for user applications
396     wininit.exe     34      SeTimeZonePrivilege     Default Adjust the time zone of the computer's internal clock
396     wininit.exe     35      SeCreateSymbolicLinkPrivilege   Present,Enabled,Default Required to create a symbolic link
396     wininit.exe     36      SeDelegateSessionUserImpersonatePrivilege               Obtain an impersonation token for another user in the same session.
432     winlogon.exe    2       SeCreateTokenPrivilege          Create a token object
432     winlogon.exe    3       SeAssignPrimaryTokenPrivilege   Present Replace a process-level token
432     winlogon.exe    4       SeLockMemoryPrivilege   Default Lock pages in memory
432     winlogon.exe    5       SeIncreaseQuotaPrivilege        Present Increase quotas
432     winlogon.exe    6       SeMachineAccountPrivilege               Add workstations to the domain
432     winlogon.exe    7       SeTcbPrivilege  Present,Enabled,Default Act as part of the operating system
432     winlogon.exe    8       SeSecurityPrivilege     Present Manage auditing and security log
432     winlogon.exe    9       SeTakeOwnershipPrivilege        Present Take ownership of files/objects
432     winlogon.exe    10      SeLoadDriverPrivilege   Present Load and unload device drivers
432     winlogon.exe    11      SeSystemProfilePrivilege        Default Profile system performance
432     winlogon.exe    12      SeSystemtimePrivilege           Change the system time
432     winlogon.exe    13      SeProfileSingleProcessPrivilege Present,Enabled,Default Profile a single process
432     winlogon.exe    14      SeIncreaseBasePriorityPrivilege Present,Enabled,Default Increase scheduling priority
432     winlogon.exe    15      SeCreatePagefilePrivilege       Default Create a pagefile
432     winlogon.exe    16      SeCreatePermanentPrivilege      Present,Enabled,Default Create permanent shared objects
432     winlogon.exe    17      SeBackupPrivilege       Present Backup files and directories
432     winlogon.exe    18      SeRestorePrivilege      Present Restore files and directories
432     winlogon.exe    19      SeShutdownPrivilege     Present Shut down the system
432     winlogon.exe    20      SeDebugPrivilege        Present,Enabled,Default Debug programs
432     winlogon.exe    21      SeAuditPrivilege        Present,Enabled,Default Generate security audits
432     winlogon.exe    22      SeSystemEnvironmentPrivilege    Present Edit firmware environment values
432     winlogon.exe    23      SeChangeNotifyPrivilege Present,Enabled,Default Receive notifications of changes to files or directories
432     winlogon.exe    24      SeRemoteShutdownPrivilege               Force shutdown from a remote system
432     winlogon.exe    25      SeUndockPrivilege       Present Remove computer from docking station
432     winlogon.exe    26      SeSyncAgentPrivilege            Synch directory service data
432     winlogon.exe    27      SeEnableDelegationPrivilege             Enable user accounts to be trusted for delegation
432     winlogon.exe    28      SeManageVolumePrivilege Present Manage the files on a volume
432     winlogon.exe    29      SeImpersonatePrivilege  Present,Enabled,Default Impersonate a client after authentication
432     winlogon.exe    30      SeCreateGlobalPrivilege Present,Enabled,Default Create global objects
432     winlogon.exe    31      SeTrustedCredManAccessPrivilege Present Access Credential Manager as a trusted caller
432     winlogon.exe    32      SeRelabelPrivilege              Modify the mandatory integrity level of an object
432     winlogon.exe    33      SeIncreaseWorkingSetPrivilege   Default Allocate more memory for user applications
432     winlogon.exe    34      SeTimeZonePrivilege     Default Adjust the time zone of the computer's internal clock
432     winlogon.exe    35      SeCreateSymbolicLinkPrivilege   Default Required to create a symbolic link
432     winlogon.exe    36      SeDelegateSessionUserImpersonatePrivilege               Obtain an impersonation token for another user in the same session.
492     services.exe    2       SeCreateTokenPrivilege          Create a token object
492     services.exe    3       SeAssignPrimaryTokenPrivilege   Present Replace a process-level token
492     services.exe    4       SeLockMemoryPrivilege   Present,Enabled,Default Lock pages in memory
492     services.exe    5       SeIncreaseQuotaPrivilege        Present Increase quotas
492     services.exe    6       SeMachineAccountPrivilege               Add workstations to the domain
492     services.exe    7       SeTcbPrivilege  Present,Enabled,Default Act as part of the operating system
492     services.exe    8       SeSecurityPrivilege     Present Manage auditing and security log
492     services.exe    9       SeTakeOwnershipPrivilege        Present Take ownership of files/objects
492     services.exe    10      SeLoadDriverPrivilege   Present Load and unload device drivers
492     services.exe    11      SeSystemProfilePrivilege        Present,Enabled,Default Profile system performance
492     services.exe    12      SeSystemtimePrivilege   Present Change the system time
492     services.exe    13      SeProfileSingleProcessPrivilege Present,Enabled,Default Profile a single process
492     services.exe    14      SeIncreaseBasePriorityPrivilege Present,Enabled,Default Increase scheduling priority
492     services.exe    15      SeCreatePagefilePrivilege       Present,Enabled,Default Create a pagefile
492     services.exe    16      SeCreatePermanentPrivilege      Present,Enabled,Default Create permanent shared objects
492     services.exe    17      SeBackupPrivilege       Present Backup files and directories
492     services.exe    18      SeRestorePrivilege      Present Restore files and directories
492     services.exe    19      SeShutdownPrivilege     Present Shut down the system
492     services.exe    20      SeDebugPrivilege        Present,Enabled,Default Debug programs
492     services.exe    21      SeAuditPrivilege        Present,Enabled,Default Generate security audits
492     services.exe    22      SeSystemEnvironmentPrivilege    Present Edit firmware environment values
492     services.exe    23      SeChangeNotifyPrivilege Present,Enabled,Default Receive notifications of changes to files or directories
492     services.exe    24      SeRemoteShutdownPrivilege               Force shutdown from a remote system
492     services.exe    25      SeUndockPrivilege       Present Remove computer from docking station
492     services.exe    26      SeSyncAgentPrivilege            Synch directory service data
492     services.exe    27      SeEnableDelegationPrivilege             Enable user accounts to be trusted for delegation
492     services.exe    28      SeManageVolumePrivilege Present Manage the files on a volume
492     services.exe    29      SeImpersonatePrivilege  Present,Enabled,Default Impersonate a client after authentication
492     services.exe    30      SeCreateGlobalPrivilege Present,Enabled,Default Create global objects
492     services.exe    31      SeTrustedCredManAccessPrivilege         Access Credential Manager as a trusted caller
492     services.exe    32      SeRelabelPrivilege              Modify the mandatory integrity level of an object
492     services.exe    33      SeIncreaseWorkingSetPrivilege   Present,Enabled,Default Allocate more memory for user applications
492     services.exe    34      SeTimeZonePrivilege     Present,Enabled,Default Adjust the time zone of the computer's internal clock
492     services.exe    35      SeCreateSymbolicLinkPrivilege   Present,Enabled,Default Required to create a symbolic link
492     services.exe    36      SeDelegateSessionUserImpersonatePrivilege               Obtain an impersonation token for another user in the same session.
500     lsass.exe       2       SeCreateTokenPrivilege  Present,Enabled Create a token object
500     lsass.exe       3       SeAssignPrimaryTokenPrivilege   Present Replace a process-level token
500     lsass.exe       4       SeLockMemoryPrivilege   Present,Enabled,Default Lock pages in memory
500     lsass.exe       5       SeIncreaseQuotaPrivilege        Present Increase quotas
500     lsass.exe       6       SeMachineAccountPrivilege               Add workstations to the domain
500     lsass.exe       7       SeTcbPrivilege  Present,Enabled,Default Act as part of the operating system
500     lsass.exe       8       SeSecurityPrivilege     Present Manage auditing and security log
500     lsass.exe       9       SeTakeOwnershipPrivilege        Present Take ownership of files/objects
500     lsass.exe       10      SeLoadDriverPrivilege   Present Load and unload device drivers
500     lsass.exe       11      SeSystemProfilePrivilege        Present,Enabled,Default Profile system performance
500     lsass.exe       12      SeSystemtimePrivilege   Present Change the system time
500     lsass.exe       13      SeProfileSingleProcessPrivilege Present,Enabled,Default Profile a single process
500     lsass.exe       14      SeIncreaseBasePriorityPrivilege Present,Enabled,Default Increase scheduling priority
500     lsass.exe       15      SeCreatePagefilePrivilege       Present,Enabled,Default Create a pagefile
500     lsass.exe       16      SeCreatePermanentPrivilege      Present,Enabled,Default Create permanent shared objects
500     lsass.exe       17      SeBackupPrivilege       Present Backup files and directories
500     lsass.exe       18      SeRestorePrivilege      Present Restore files and directories
500     lsass.exe       19      SeShutdownPrivilege     Present Shut down the system
500     lsass.exe       20      SeDebugPrivilege        Present,Enabled,Default Debug programs
500     lsass.exe       21      SeAuditPrivilege        Present,Enabled,Default Generate security audits
500     lsass.exe       22      SeSystemEnvironmentPrivilege    Present Edit firmware environment values
500     lsass.exe       23      SeChangeNotifyPrivilege Present,Enabled,Default Receive notifications of changes to files or directories
500     lsass.exe       24      SeRemoteShutdownPrivilege               Force shutdown from a remote system
500     lsass.exe       25      SeUndockPrivilege       Present Remove computer from docking station
500     lsass.exe       26      SeSyncAgentPrivilege            Synch directory service data
500     lsass.exe       27      SeEnableDelegationPrivilege             Enable user accounts to be trusted for delegation
500     lsass.exe       28      SeManageVolumePrivilege Present Manage the files on a volume
500     lsass.exe       29      SeImpersonatePrivilege  Present,Enabled,Default Impersonate a client after authentication
500     lsass.exe       30      SeCreateGlobalPrivilege Present,Enabled,Default Create global objects
500     lsass.exe       31      SeTrustedCredManAccessPrivilege Present Access Credential Manager as a trusted caller
500     lsass.exe       32      SeRelabelPrivilege      Present Modify the mandatory integrity level of an object
500     lsass.exe       33      SeIncreaseWorkingSetPrivilege   Present,Enabled,Default Allocate more memory for user applications
500     lsass.exe       34      SeTimeZonePrivilege     Present,Enabled,Default Adjust the time zone of the computer's internal clock
500     lsass.exe       35      SeCreateSymbolicLinkPrivilege   Present,Enabled,Default Required to create a symbolic link
500     lsass.exe       36      SeDelegateSessionUserImpersonatePrivilege               Obtain an impersonation token for another user in the same session.
508     lsm.exe 2       SeCreateTokenPrivilege          Create a token object
508     lsm.exe 3       SeAssignPrimaryTokenPrivilege   Present Replace a process-level token
508     lsm.exe 4       SeLockMemoryPrivilege   Present,Enabled,Default Lock pages in memory
508     lsm.exe 5       SeIncreaseQuotaPrivilege        Present Increase quotas
508     lsm.exe 6       SeMachineAccountPrivilege               Add workstations to the domain
508     lsm.exe 7       SeTcbPrivilege  Present,Enabled,Default Act as part of the operating system
508     lsm.exe 8       SeSecurityPrivilege     Present Manage auditing and security log
508     lsm.exe 9       SeTakeOwnershipPrivilege        Present Take ownership of files/objects
508     lsm.exe 10      SeLoadDriverPrivilege   Present Load and unload device drivers
508     lsm.exe 11      SeSystemProfilePrivilege        Present,Enabled,Default Profile system performance
508     lsm.exe 12      SeSystemtimePrivilege   Present Change the system time
508     lsm.exe 13      SeProfileSingleProcessPrivilege Present,Enabled,Default Profile a single process
508     lsm.exe 14      SeIncreaseBasePriorityPrivilege Present,Enabled,Default Increase scheduling priority
508     lsm.exe 15      SeCreatePagefilePrivilege       Present,Enabled,Default Create a pagefile
508     lsm.exe 16      SeCreatePermanentPrivilege      Present,Enabled,Default Create permanent shared objects
508     lsm.exe 17      SeBackupPrivilege       Present Backup files and directories
508     lsm.exe 18      SeRestorePrivilege      Present Restore files and directories
508     lsm.exe 19      SeShutdownPrivilege     Present Shut down the system
508     lsm.exe 20      SeDebugPrivilege        Present,Enabled,Default Debug programs
508     lsm.exe 21      SeAuditPrivilege        Present,Enabled,Default Generate security audits
508     lsm.exe 22      SeSystemEnvironmentPrivilege    Present Edit firmware environment values
508     lsm.exe 23      SeChangeNotifyPrivilege Present,Enabled,Default Receive notifications of changes to files or directories
508     lsm.exe 24      SeRemoteShutdownPrivilege               Force shutdown from a remote system
508     lsm.exe 25      SeUndockPrivilege       Present Remove computer from docking station
508     lsm.exe 26      SeSyncAgentPrivilege            Synch directory service data
508     lsm.exe 27      SeEnableDelegationPrivilege             Enable user accounts to be trusted for delegation
508     lsm.exe 28      SeManageVolumePrivilege Present Manage the files on a volume
508     lsm.exe 29      SeImpersonatePrivilege  Present,Enabled,Default Impersonate a client after authentication
508     lsm.exe 30      SeCreateGlobalPrivilege Present,Enabled,Default Create global objects
508     lsm.exe 31      SeTrustedCredManAccessPrivilege         Access Credential Manager as a trusted caller
508     lsm.exe 32      SeRelabelPrivilege      Present Modify the mandatory integrity level of an object
508     lsm.exe 33      SeIncreaseWorkingSetPrivilege   Present,Enabled,Default Allocate more memory for user applications
508     lsm.exe 34      SeTimeZonePrivilege     Present,Enabled,Default Adjust the time zone of the computer's internal clock
508     lsm.exe 35      SeCreateSymbolicLinkPrivilege   Present,Enabled,Default Required to create a symbolic link
508     lsm.exe 36      SeDelegateSessionUserImpersonatePrivilege               Obtain an impersonation token for another user in the same session.
604     svchost.exe     2       SeCreateTokenPrivilege          Create a token object
604     svchost.exe     3       SeAssignPrimaryTokenPrivilege   Present Replace a process-level token
604     svchost.exe     4       SeLockMemoryPrivilege   Default Lock pages in memory
604     svchost.exe     5       SeIncreaseQuotaPrivilege        Present Increase quotas
604     svchost.exe     6       SeMachineAccountPrivilege               Add workstations to the domain
604     svchost.exe     7       SeTcbPrivilege  Present,Enabled,Default Act as part of the operating system
604     svchost.exe     8       SeSecurityPrivilege     Present Manage auditing and security log
604     svchost.exe     9       SeTakeOwnershipPrivilege        Present Take ownership of files/objects
604     svchost.exe     10      SeLoadDriverPrivilege   Present Load and unload device drivers
604     svchost.exe     11      SeSystemProfilePrivilege        Default Profile system performance
604     svchost.exe     12      SeSystemtimePrivilege           Change the system time
604     svchost.exe     13      SeProfileSingleProcessPrivilege Default Profile a single process
604     svchost.exe     14      SeIncreaseBasePriorityPrivilege Default Increase scheduling priority
604     svchost.exe     15      SeCreatePagefilePrivilege       Default Create a pagefile
604     svchost.exe     16      SeCreatePermanentPrivilege      Default Create permanent shared objects
604     svchost.exe     17      SeBackupPrivilege       Present Backup files and directories
604     svchost.exe     18      SeRestorePrivilege      Present Restore files and directories
604     svchost.exe     19      SeShutdownPrivilege     Present Shut down the system
604     svchost.exe     20      SeDebugPrivilege        Present,Enabled,Default Debug programs
604     svchost.exe     21      SeAuditPrivilege        Present,Enabled,Default Generate security audits
604     svchost.exe     22      SeSystemEnvironmentPrivilege            Edit firmware environment values
604     svchost.exe     23      SeChangeNotifyPrivilege Present,Enabled,Default Receive notifications of changes to files or directories
604     svchost.exe     24      SeRemoteShutdownPrivilege               Force shutdown from a remote system
604     svchost.exe     25      SeUndockPrivilege       Present Remove computer from docking station
604     svchost.exe     26      SeSyncAgentPrivilege            Synch directory service data
604     svchost.exe     27      SeEnableDelegationPrivilege             Enable user accounts to be trusted for delegation
604     svchost.exe     28      SeManageVolumePrivilege         Manage the files on a volume
604     svchost.exe     29      SeImpersonatePrivilege  Present,Enabled,Default Impersonate a client after authentication
604     svchost.exe     30      SeCreateGlobalPrivilege Present,Enabled,Default Create global objects
604     svchost.exe     31      SeTrustedCredManAccessPrivilege         Access Credential Manager as a trusted caller
604     svchost.exe     32      SeRelabelPrivilege              Modify the mandatory integrity level of an object
604     svchost.exe     33      SeIncreaseWorkingSetPrivilege   Default Allocate more memory for user applications
604     svchost.exe     34      SeTimeZonePrivilege     Default Adjust the time zone of the computer's internal clock
604     svchost.exe     35      SeCreateSymbolicLinkPrivilege   Default Required to create a symbolic link
604     svchost.exe     36      SeDelegateSessionUserImpersonatePrivilege               Obtain an impersonation token for another user in the same session.
668     vmacthlp.exe    2       SeCreateTokenPrivilege          Create a token object
668     vmacthlp.exe    3       SeAssignPrimaryTokenPrivilege   Present Replace a process-level token
668     vmacthlp.exe    4       SeLockMemoryPrivilege   Present,Enabled,Default Lock pages in memory
668     vmacthlp.exe    5       SeIncreaseQuotaPrivilege        Present Increase quotas
668     vmacthlp.exe    6       SeMachineAccountPrivilege               Add workstations to the domain
668     vmacthlp.exe    7       SeTcbPrivilege  Present,Enabled,Default Act as part of the operating system
668     vmacthlp.exe    8       SeSecurityPrivilege     Present Manage auditing and security log
668     vmacthlp.exe    9       SeTakeOwnershipPrivilege        Present Take ownership of files/objects
668     vmacthlp.exe    10      SeLoadDriverPrivilege   Present Load and unload device drivers
668     vmacthlp.exe    11      SeSystemProfilePrivilege        Present,Enabled,Default Profile system performance
668     vmacthlp.exe    12      SeSystemtimePrivilege   Present Change the system time
668     vmacthlp.exe    13      SeProfileSingleProcessPrivilege Present,Enabled,Default Profile a single process
668     vmacthlp.exe    14      SeIncreaseBasePriorityPrivilege Present,Enabled,Default Increase scheduling priority
668     vmacthlp.exe    15      SeCreatePagefilePrivilege       Present,Enabled,Default Create a pagefile
668     vmacthlp.exe    16      SeCreatePermanentPrivilege      Present,Enabled,Default Create permanent shared objects
668     vmacthlp.exe    17      SeBackupPrivilege       Present Backup files and directories
668     vmacthlp.exe    18      SeRestorePrivilege      Present Restore files and directories
668     vmacthlp.exe    19      SeShutdownPrivilege     Present Shut down the system
668     vmacthlp.exe    20      SeDebugPrivilege        Present,Enabled,Default Debug programs
668     vmacthlp.exe    21      SeAuditPrivilege        Present,Enabled,Default Generate security audits
668     vmacthlp.exe    22      SeSystemEnvironmentPrivilege    Present Edit firmware environment values
668     vmacthlp.exe    23      SeChangeNotifyPrivilege Present,Enabled,Default Receive notifications of changes to files or directories
668     vmacthlp.exe    24      SeRemoteShutdownPrivilege               Force shutdown from a remote system
668     vmacthlp.exe    25      SeUndockPrivilege       Present Remove computer from docking station
668     vmacthlp.exe    26      SeSyncAgentPrivilege            Synch directory service data
668     vmacthlp.exe    27      SeEnableDelegationPrivilege             Enable user accounts to be trusted for delegation
668     vmacthlp.exe    28      SeManageVolumePrivilege Present Manage the files on a volume
668     vmacthlp.exe    29      SeImpersonatePrivilege  Present,Enabled,Default Impersonate a client after authentication
668     vmacthlp.exe    30      SeCreateGlobalPrivilege Present,Enabled,Default Create global objects
668     vmacthlp.exe    31      SeTrustedCredManAccessPrivilege         Access Credential Manager as a trusted caller
668     vmacthlp.exe    32      SeRelabelPrivilege              Modify the mandatory integrity level of an object
668     vmacthlp.exe    33      SeIncreaseWorkingSetPrivilege   Present,Enabled,Default Allocate more memory for user applications
668     vmacthlp.exe    34      SeTimeZonePrivilege     Present,Enabled,Default Adjust the time zone of the computer's internal clock
668     vmacthlp.exe    35      SeCreateSymbolicLinkPrivilege   Present,Enabled,Default Required to create a symbolic link
668     vmacthlp.exe    36      SeDelegateSessionUserImpersonatePrivilege               Obtain an impersonation token for another user in the same session.
712     svchost.exe     2       SeCreateTokenPrivilege          Create a token object
712     svchost.exe     3       SeAssignPrimaryTokenPrivilege           Replace a process-level token
712     svchost.exe     4       SeLockMemoryPrivilege           Lock pages in memory
712     svchost.exe     5       SeIncreaseQuotaPrivilege                Increase quotas
712     svchost.exe     6       SeMachineAccountPrivilege               Add workstations to the domain
712     svchost.exe     7       SeTcbPrivilege          Act as part of the operating system
712     svchost.exe     8       SeSecurityPrivilege             Manage auditing and security log
712     svchost.exe     9       SeTakeOwnershipPrivilege                Take ownership of files/objects
712     svchost.exe     10      SeLoadDriverPrivilege           Load and unload device drivers
712     svchost.exe     11      SeSystemProfilePrivilege                Profile system performance
712     svchost.exe     12      SeSystemtimePrivilege           Change the system time
712     svchost.exe     13      SeProfileSingleProcessPrivilege         Profile a single process
712     svchost.exe     14      SeIncreaseBasePriorityPrivilege         Increase scheduling priority
712     svchost.exe     15      SeCreatePagefilePrivilege               Create a pagefile
712     svchost.exe     16      SeCreatePermanentPrivilege              Create permanent shared objects
712     svchost.exe     17      SeBackupPrivilege               Backup files and directories
712     svchost.exe     18      SeRestorePrivilege              Restore files and directories
712     svchost.exe     19      SeShutdownPrivilege             Shut down the system
712     svchost.exe     20      SeDebugPrivilege                Debug programs
712     svchost.exe     21      SeAuditPrivilege                Generate security audits
712     svchost.exe     22      SeSystemEnvironmentPrivilege            Edit firmware environment values
712     svchost.exe     23      SeChangeNotifyPrivilege Present,Enabled,Default Receive notifications of changes to files or directories
712     svchost.exe     24      SeRemoteShutdownPrivilege               Force shutdown from a remote system
712     svchost.exe     25      SeUndockPrivilege               Remove computer from docking station
712     svchost.exe     26      SeSyncAgentPrivilege            Synch directory service data
712     svchost.exe     27      SeEnableDelegationPrivilege             Enable user accounts to be trusted for delegation
712     svchost.exe     28      SeManageVolumePrivilege         Manage the files on a volume
712     svchost.exe     29      SeImpersonatePrivilege  Present,Enabled,Default Impersonate a client after authentication
712     svchost.exe     30      SeCreateGlobalPrivilege Present,Enabled,Default Create global objects
712     svchost.exe     31      SeTrustedCredManAccessPrivilege         Access Credential Manager as a trusted caller
712     svchost.exe     32      SeRelabelPrivilege              Modify the mandatory integrity level of an object
712     svchost.exe     33      SeIncreaseWorkingSetPrivilege           Allocate more memory for user applications
712     svchost.exe     34      SeTimeZonePrivilege             Adjust the time zone of the computer's internal clock
712     svchost.exe     35      SeCreateSymbolicLinkPrivilege           Required to create a symbolic link
712     svchost.exe     36      SeDelegateSessionUserImpersonatePrivilege               Obtain an impersonation token for another user in the same session.
808     svchost.exe     2       SeCreateTokenPrivilege          Create a token object
808     svchost.exe     3       SeAssignPrimaryTokenPrivilege           Replace a process-level token
808     svchost.exe     4       SeLockMemoryPrivilege           Lock pages in memory
808     svchost.exe     5       SeIncreaseQuotaPrivilege                Increase quotas
808     svchost.exe     6       SeMachineAccountPrivilege               Add workstations to the domain
808     svchost.exe     7       SeTcbPrivilege          Act as part of the operating system
808     svchost.exe     8       SeSecurityPrivilege             Manage auditing and security log
808     svchost.exe     9       SeTakeOwnershipPrivilege                Take ownership of files/objects
808     svchost.exe     10      SeLoadDriverPrivilege           Load and unload device drivers
808     svchost.exe     11      SeSystemProfilePrivilege                Profile system performance
808     svchost.exe     12      SeSystemtimePrivilege           Change the system time
808     svchost.exe     13      SeProfileSingleProcessPrivilege         Profile a single process
808     svchost.exe     14      SeIncreaseBasePriorityPrivilege         Increase scheduling priority
808     svchost.exe     15      SeCreatePagefilePrivilege               Create a pagefile
808     svchost.exe     16      SeCreatePermanentPrivilege              Create permanent shared objects
808     svchost.exe     17      SeBackupPrivilege               Backup files and directories
808     svchost.exe     18      SeRestorePrivilege              Restore files and directories
808     svchost.exe     19      SeShutdownPrivilege             Shut down the system
808     svchost.exe     20      SeDebugPrivilege                Debug programs
808     svchost.exe     21      SeAuditPrivilege                Generate security audits
808     svchost.exe     22      SeSystemEnvironmentPrivilege            Edit firmware environment values
808     svchost.exe     23      SeChangeNotifyPrivilege Present,Enabled,Default Receive notifications of changes to files or directories
808     svchost.exe     24      SeRemoteShutdownPrivilege               Force shutdown from a remote system
808     svchost.exe     25      SeUndockPrivilege               Remove computer from docking station
808     svchost.exe     26      SeSyncAgentPrivilege            Synch directory service data
808     svchost.exe     27      SeEnableDelegationPrivilege             Enable user accounts to be trusted for delegation
808     svchost.exe     28      SeManageVolumePrivilege         Manage the files on a volume
808     svchost.exe     29      SeImpersonatePrivilege  Present,Enabled,Default Impersonate a client after authentication
808     svchost.exe     30      SeCreateGlobalPrivilege Present,Enabled,Default Create global objects
808     svchost.exe     31      SeTrustedCredManAccessPrivilege         Access Credential Manager as a trusted caller
808     svchost.exe     32      SeRelabelPrivilege              Modify the mandatory integrity level of an object
808     svchost.exe     33      SeIncreaseWorkingSetPrivilege   Present Allocate more memory for user applications
808     svchost.exe     34      SeTimeZonePrivilege             Adjust the time zone of the computer's internal clock
808     svchost.exe     35      SeCreateSymbolicLinkPrivilege           Required to create a symbolic link
808     svchost.exe     36      SeDelegateSessionUserImpersonatePrivilege               Obtain an impersonation token for another user in the same session.
844     svchost.exe     2       SeCreateTokenPrivilege          Create a token object
844     svchost.exe     3       SeAssignPrimaryTokenPrivilege   Present Replace a process-level token
844     svchost.exe     4       SeLockMemoryPrivilege   Default Lock pages in memory
844     svchost.exe     5       SeIncreaseQuotaPrivilege        Present Increase quotas
844     svchost.exe     6       SeMachineAccountPrivilege               Add workstations to the domain
844     svchost.exe     7       SeTcbPrivilege  Present,Enabled,Default Act as part of the operating system
844     svchost.exe     8       SeSecurityPrivilege     Present Manage auditing and security log
844     svchost.exe     9       SeTakeOwnershipPrivilege        Present Take ownership of files/objects
844     svchost.exe     10      SeLoadDriverPrivilege   Present Load and unload device drivers
844     svchost.exe     11      SeSystemProfilePrivilege        Default Profile system performance
844     svchost.exe     12      SeSystemtimePrivilege           Change the system time
844     svchost.exe     13      SeProfileSingleProcessPrivilege Present,Enabled,Default Profile a single process
844     svchost.exe     14      SeIncreaseBasePriorityPrivilege Present,Enabled,Default Increase scheduling priority
844     svchost.exe     15      SeCreatePagefilePrivilege       Default Create a pagefile
844     svchost.exe     16      SeCreatePermanentPrivilege      Present,Enabled,Default Create permanent shared objects
844     svchost.exe     17      SeBackupPrivilege               Backup files and directories
844     svchost.exe     18      SeRestorePrivilege      Present Restore files and directories
844     svchost.exe     19      SeShutdownPrivilege             Shut down the system
844     svchost.exe     20      SeDebugPrivilege        Present,Enabled,Default Debug programs
844     svchost.exe     21      SeAuditPrivilege        Present,Enabled,Default Generate security audits
844     svchost.exe     22      SeSystemEnvironmentPrivilege    Present Edit firmware environment values
844     svchost.exe     23      SeChangeNotifyPrivilege Present,Enabled,Default Receive notifications of changes to files or directories
844     svchost.exe     24      SeRemoteShutdownPrivilege               Force shutdown from a remote system
844     svchost.exe     25      SeUndockPrivilege               Remove computer from docking station
844     svchost.exe     26      SeSyncAgentPrivilege            Synch directory service data
844     svchost.exe     27      SeEnableDelegationPrivilege             Enable user accounts to be trusted for delegation
844     svchost.exe     28      SeManageVolumePrivilege         Manage the files on a volume
844     svchost.exe     29      SeImpersonatePrivilege  Present,Enabled,Default Impersonate a client after authentication
844     svchost.exe     30      SeCreateGlobalPrivilege Present,Enabled,Default Create global objects
844     svchost.exe     31      SeTrustedCredManAccessPrivilege         Access Credential Manager as a trusted caller
844     svchost.exe     32      SeRelabelPrivilege              Modify the mandatory integrity level of an object
844     svchost.exe     33      SeIncreaseWorkingSetPrivilege   Default Allocate more memory for user applications
844     svchost.exe     34      SeTimeZonePrivilege     Default Adjust the time zone of the computer's internal clock
844     svchost.exe     35      SeCreateSymbolicLinkPrivilege   Default Required to create a symbolic link
844     svchost.exe     36      SeDelegateSessionUserImpersonatePrivilege               Obtain an impersonation token for another user in the same session.
868     svchost.exe     2       SeCreateTokenPrivilege          Create a token object
868     svchost.exe     3       SeAssignPrimaryTokenPrivilege   Present Replace a process-level token
868     svchost.exe     4       SeLockMemoryPrivilege   Present,Enabled,Default Lock pages in memory
868     svchost.exe     5       SeIncreaseQuotaPrivilege        Present Increase quotas
868     svchost.exe     6       SeMachineAccountPrivilege               Add workstations to the domain
868     svchost.exe     7       SeTcbPrivilege  Present,Enabled,Default Act as part of the operating system
868     svchost.exe     8       SeSecurityPrivilege     Present Manage auditing and security log
868     svchost.exe     9       SeTakeOwnershipPrivilege        Present Take ownership of files/objects
868     svchost.exe     10      SeLoadDriverPrivilege   Present Load and unload device drivers
868     svchost.exe     11      SeSystemProfilePrivilege        Present,Enabled,Default Profile system performance
868     svchost.exe     12      SeSystemtimePrivilege   Present Change the system time
868     svchost.exe     13      SeProfileSingleProcessPrivilege Present,Enabled,Default Profile a single process
868     svchost.exe     14      SeIncreaseBasePriorityPrivilege Present,Enabled,Default Increase scheduling priority
868     svchost.exe     15      SeCreatePagefilePrivilege       Present,Enabled,Default Create a pagefile
868     svchost.exe     16      SeCreatePermanentPrivilege      Present,Enabled,Default Create permanent shared objects
868     svchost.exe     17      SeBackupPrivilege       Present Backup files and directories
868     svchost.exe     18      SeRestorePrivilege      Present Restore files and directories
868     svchost.exe     19      SeShutdownPrivilege     Present Shut down the system
868     svchost.exe     20      SeDebugPrivilege        Present,Enabled,Default Debug programs
868     svchost.exe     21      SeAuditPrivilege        Present,Enabled,Default Generate security audits
868     svchost.exe     22      SeSystemEnvironmentPrivilege    Present Edit firmware environment values
868     svchost.exe     23      SeChangeNotifyPrivilege Present,Enabled,Default Receive notifications of changes to files or directories
868     svchost.exe     24      SeRemoteShutdownPrivilege               Force shutdown from a remote system
868     svchost.exe     25      SeUndockPrivilege       Present Remove computer from docking station
868     svchost.exe     26      SeSyncAgentPrivilege            Synch directory service data
868     svchost.exe     27      SeEnableDelegationPrivilege             Enable user accounts to be trusted for delegation
868     svchost.exe     28      SeManageVolumePrivilege Present Manage the files on a volume
868     svchost.exe     29      SeImpersonatePrivilege  Present,Enabled,Default Impersonate a client after authentication
868     svchost.exe     30      SeCreateGlobalPrivilege Present,Enabled,Default Create global objects
868     svchost.exe     31      SeTrustedCredManAccessPrivilege         Access Credential Manager as a trusted caller
868     svchost.exe     32      SeRelabelPrivilege              Modify the mandatory integrity level of an object
868     svchost.exe     33      SeIncreaseWorkingSetPrivilege   Present,Enabled,Default Allocate more memory for user applications
868     svchost.exe     34      SeTimeZonePrivilege     Present,Enabled,Default Adjust the time zone of the computer's internal clock
868     svchost.exe     35      SeCreateSymbolicLinkPrivilege   Present,Enabled,Default Required to create a symbolic link
868     svchost.exe     36      SeDelegateSessionUserImpersonatePrivilege               Obtain an impersonation token for another user in the same session.
960     audiodg.exe     2       SeCreateTokenPrivilege          Create a token object
960     audiodg.exe     3       SeAssignPrimaryTokenPrivilege           Replace a process-level token
960     audiodg.exe     4       SeLockMemoryPrivilege           Lock pages in memory
960     audiodg.exe     5       SeIncreaseQuotaPrivilege                Increase quotas
960     audiodg.exe     6       SeMachineAccountPrivilege               Add workstations to the domain
960     audiodg.exe     7       SeTcbPrivilege          Act as part of the operating system
960     audiodg.exe     8       SeSecurityPrivilege             Manage auditing and security log
960     audiodg.exe     9       SeTakeOwnershipPrivilege                Take ownership of files/objects
960     audiodg.exe     10      SeLoadDriverPrivilege           Load and unload device drivers
960     audiodg.exe     11      SeSystemProfilePrivilege                Profile system performance
960     audiodg.exe     12      SeSystemtimePrivilege           Change the system time
960     audiodg.exe     13      SeProfileSingleProcessPrivilege         Profile a single process
960     audiodg.exe     14      SeIncreaseBasePriorityPrivilege         Increase scheduling priority
960     audiodg.exe     15      SeCreatePagefilePrivilege               Create a pagefile
960     audiodg.exe     16      SeCreatePermanentPrivilege              Create permanent shared objects
960     audiodg.exe     17      SeBackupPrivilege               Backup files and directories
960     audiodg.exe     18      SeRestorePrivilege              Restore files and directories
960     audiodg.exe     19      SeShutdownPrivilege             Shut down the system
960     audiodg.exe     20      SeDebugPrivilege                Debug programs
960     audiodg.exe     21      SeAuditPrivilege                Generate security audits
960     audiodg.exe     22      SeSystemEnvironmentPrivilege            Edit firmware environment values
960     audiodg.exe     23      SeChangeNotifyPrivilege Present,Enabled,Default Receive notifications of changes to files or directories
960     audiodg.exe     24      SeRemoteShutdownPrivilege               Force shutdown from a remote system
960     audiodg.exe     25      SeUndockPrivilege               Remove computer from docking station
960     audiodg.exe     26      SeSyncAgentPrivilege            Synch directory service data
960     audiodg.exe     27      SeEnableDelegationPrivilege             Enable user accounts to be trusted for delegation
960     audiodg.exe     28      SeManageVolumePrivilege         Manage the files on a volume
960     audiodg.exe     29      SeImpersonatePrivilege  Present,Enabled,Default Impersonate a client after authentication
960     audiodg.exe     30      SeCreateGlobalPrivilege Present,Enabled,Default Create global objects
960     audiodg.exe     31      SeTrustedCredManAccessPrivilege         Access Credential Manager as a trusted caller
960     audiodg.exe     32      SeRelabelPrivilege              Modify the mandatory integrity level of an object
960     audiodg.exe     33      SeIncreaseWorkingSetPrivilege   Present Allocate more memory for user applications
960     audiodg.exe     34      SeTimeZonePrivilege             Adjust the time zone of the computer's internal clock
960     audiodg.exe     35      SeCreateSymbolicLinkPrivilege           Required to create a symbolic link
960     audiodg.exe     36      SeDelegateSessionUserImpersonatePrivilege               Obtain an impersonation token for another user in the same session.
1012    svchost.exe     2       SeCreateTokenPrivilege          Create a token object
1012    svchost.exe     3       SeAssignPrimaryTokenPrivilege           Replace a process-level token
1012    svchost.exe     4       SeLockMemoryPrivilege           Lock pages in memory
1012    svchost.exe     5       SeIncreaseQuotaPrivilege                Increase quotas
1012    svchost.exe     6       SeMachineAccountPrivilege               Add workstations to the domain
1012    svchost.exe     7       SeTcbPrivilege          Act as part of the operating system
1012    svchost.exe     8       SeSecurityPrivilege             Manage auditing and security log
1012    svchost.exe     9       SeTakeOwnershipPrivilege                Take ownership of files/objects
1012    svchost.exe     10      SeLoadDriverPrivilege           Load and unload device drivers
1012    svchost.exe     11      SeSystemProfilePrivilege        Present Profile system performance
1012    svchost.exe     12      SeSystemtimePrivilege   Present Change the system time
1012    svchost.exe     13      SeProfileSingleProcessPrivilege         Profile a single process
1012    svchost.exe     14      SeIncreaseBasePriorityPrivilege         Increase scheduling priority
1012    svchost.exe     15      SeCreatePagefilePrivilege               Create a pagefile
1012    svchost.exe     16      SeCreatePermanentPrivilege              Create permanent shared objects
1012    svchost.exe     17      SeBackupPrivilege               Backup files and directories
1012    svchost.exe     18      SeRestorePrivilege              Restore files and directories
1012    svchost.exe     19      SeShutdownPrivilege             Shut down the system
1012    svchost.exe     20      SeDebugPrivilege                Debug programs
1012    svchost.exe     21      SeAuditPrivilege        Present Generate security audits
1012    svchost.exe     22      SeSystemEnvironmentPrivilege            Edit firmware environment values
1012    svchost.exe     23      SeChangeNotifyPrivilege Present,Enabled,Default Receive notifications of changes to files or directories
1012    svchost.exe     24      SeRemoteShutdownPrivilege               Force shutdown from a remote system
1012    svchost.exe     25      SeUndockPrivilege               Remove computer from docking station
1012    svchost.exe     26      SeSyncAgentPrivilege            Synch directory service data
1012    svchost.exe     27      SeEnableDelegationPrivilege             Enable user accounts to be trusted for delegation
1012    svchost.exe     28      SeManageVolumePrivilege         Manage the files on a volume
1012    svchost.exe     29      SeImpersonatePrivilege  Present,Enabled,Default Impersonate a client after authentication
1012    svchost.exe     30      SeCreateGlobalPrivilege Present,Enabled,Default Create global objects
1012    svchost.exe     31      SeTrustedCredManAccessPrivilege         Access Credential Manager as a trusted caller
1012    svchost.exe     32      SeRelabelPrivilege              Modify the mandatory integrity level of an object
1012    svchost.exe     33      SeIncreaseWorkingSetPrivilege           Allocate more memory for user applications
1012    svchost.exe     34      SeTimeZonePrivilege             Adjust the time zone of the computer's internal clock
1012    svchost.exe     35      SeCreateSymbolicLinkPrivilege           Required to create a symbolic link
1012    svchost.exe     36      SeDelegateSessionUserImpersonatePrivilege               Obtain an impersonation token for another user in the same session.
620     svchost.exe     2       SeCreateTokenPrivilege          Create a token object
620     svchost.exe     3       SeAssignPrimaryTokenPrivilege   Present Replace a process-level token
620     svchost.exe     4       SeLockMemoryPrivilege           Lock pages in memory
620     svchost.exe     5       SeIncreaseQuotaPrivilege        Present Increase quotas
620     svchost.exe     6       SeMachineAccountPrivilege               Add workstations to the domain
620     svchost.exe     7       SeTcbPrivilege          Act as part of the operating system
620     svchost.exe     8       SeSecurityPrivilege             Manage auditing and security log
620     svchost.exe     9       SeTakeOwnershipPrivilege                Take ownership of files/objects
620     svchost.exe     10      SeLoadDriverPrivilege           Load and unload device drivers
620     svchost.exe     11      SeSystemProfilePrivilege                Profile system performance
620     svchost.exe     12      SeSystemtimePrivilege           Change the system time
620     svchost.exe     13      SeProfileSingleProcessPrivilege         Profile a single process
620     svchost.exe     14      SeIncreaseBasePriorityPrivilege         Increase scheduling priority
620     svchost.exe     15      SeCreatePagefilePrivilege               Create a pagefile
620     svchost.exe     16      SeCreatePermanentPrivilege              Create permanent shared objects
620     svchost.exe     17      SeBackupPrivilege               Backup files and directories
620     svchost.exe     18      SeRestorePrivilege              Restore files and directories
620     svchost.exe     19      SeShutdownPrivilege             Shut down the system
620     svchost.exe     20      SeDebugPrivilege                Debug programs
620     svchost.exe     21      SeAuditPrivilege        Present,Enabled Generate security audits
620     svchost.exe     22      SeSystemEnvironmentPrivilege            Edit firmware environment values
620     svchost.exe     23      SeChangeNotifyPrivilege Present,Enabled,Default Receive notifications of changes to files or directories
620     svchost.exe     24      SeRemoteShutdownPrivilege               Force shutdown from a remote system
620     svchost.exe     25      SeUndockPrivilege               Remove computer from docking station
620     svchost.exe     26      SeSyncAgentPrivilege            Synch directory service data
620     svchost.exe     27      SeEnableDelegationPrivilege             Enable user accounts to be trusted for delegation
620     svchost.exe     28      SeManageVolumePrivilege         Manage the files on a volume
620     svchost.exe     29      SeImpersonatePrivilege  Present,Enabled,Default Impersonate a client after authentication
620     svchost.exe     30      SeCreateGlobalPrivilege Present,Enabled,Default Create global objects
620     svchost.exe     31      SeTrustedCredManAccessPrivilege         Access Credential Manager as a trusted caller
620     svchost.exe     32      SeRelabelPrivilege              Modify the mandatory integrity level of an object
620     svchost.exe     33      SeIncreaseWorkingSetPrivilege           Allocate more memory for user applications
620     svchost.exe     34      SeTimeZonePrivilege             Adjust the time zone of the computer's internal clock
620     svchost.exe     35      SeCreateSymbolicLinkPrivilege           Required to create a symbolic link
620     svchost.exe     36      SeDelegateSessionUserImpersonatePrivilege               Obtain an impersonation token for another user in the same session.
1120    spoolsv.exe     2       SeCreateTokenPrivilege          Create a token object
1120    spoolsv.exe     3       SeAssignPrimaryTokenPrivilege   Present Replace a process-level token
1120    spoolsv.exe     4       SeLockMemoryPrivilege   Default Lock pages in memory
1120    spoolsv.exe     5       SeIncreaseQuotaPrivilege                Increase quotas
1120    spoolsv.exe     6       SeMachineAccountPrivilege               Add workstations to the domain
1120    spoolsv.exe     7       SeTcbPrivilege  Present,Enabled,Default Act as part of the operating system
1120    spoolsv.exe     8       SeSecurityPrivilege             Manage auditing and security log
1120    spoolsv.exe     9       SeTakeOwnershipPrivilege                Take ownership of files/objects
1120    spoolsv.exe     10      SeLoadDriverPrivilege           Load and unload device drivers
1120    spoolsv.exe     11      SeSystemProfilePrivilege        Default Profile system performance
1120    spoolsv.exe     12      SeSystemtimePrivilege           Change the system time
1120    spoolsv.exe     13      SeProfileSingleProcessPrivilege Default Profile a single process
1120    spoolsv.exe     14      SeIncreaseBasePriorityPrivilege Default Increase scheduling priority
1120    spoolsv.exe     15      SeCreatePagefilePrivilege       Default Create a pagefile
1120    spoolsv.exe     16      SeCreatePermanentPrivilege      Default Create permanent shared objects
1120    spoolsv.exe     17      SeBackupPrivilege               Backup files and directories
1120    spoolsv.exe     18      SeRestorePrivilege              Restore files and directories
1120    spoolsv.exe     19      SeShutdownPrivilege             Shut down the system
1120    spoolsv.exe     20      SeDebugPrivilege        Default Debug programs
1120    spoolsv.exe     21      SeAuditPrivilege        Present,Enabled,Default Generate security audits
1120    spoolsv.exe     22      SeSystemEnvironmentPrivilege            Edit firmware environment values
1120    spoolsv.exe     23      SeChangeNotifyPrivilege Present,Enabled,Default Receive notifications of changes to files or directories
1120    spoolsv.exe     24      SeRemoteShutdownPrivilege               Force shutdown from a remote system
1120    spoolsv.exe     25      SeUndockPrivilege               Remove computer from docking station
1120    spoolsv.exe     26      SeSyncAgentPrivilege            Synch directory service data
1120    spoolsv.exe     27      SeEnableDelegationPrivilege             Enable user accounts to be trusted for delegation
1120    spoolsv.exe     28      SeManageVolumePrivilege         Manage the files on a volume
1120    spoolsv.exe     29      SeImpersonatePrivilege  Present,Enabled,Default Impersonate a client after authentication
1120    spoolsv.exe     30      SeCreateGlobalPrivilege Default Create global objects
1120    spoolsv.exe     31      SeTrustedCredManAccessPrivilege         Access Credential Manager as a trusted caller
1120    spoolsv.exe     32      SeRelabelPrivilege              Modify the mandatory integrity level of an object
1120    spoolsv.exe     33      SeIncreaseWorkingSetPrivilege   Default Allocate more memory for user applications
1120    spoolsv.exe     34      SeTimeZonePrivilege     Default Adjust the time zone of the computer's internal clock
1120    spoolsv.exe     35      SeCreateSymbolicLinkPrivilege   Default Required to create a symbolic link
1120    spoolsv.exe     36      SeDelegateSessionUserImpersonatePrivilege               Obtain an impersonation token for another user in the same session.
1164    svchost.exe     2       SeCreateTokenPrivilege          Create a token object
1164    svchost.exe     3       SeAssignPrimaryTokenPrivilege   Present Replace a process-level token
1164    svchost.exe     4       SeLockMemoryPrivilege           Lock pages in memory
1164    svchost.exe     5       SeIncreaseQuotaPrivilege        Present Increase quotas
1164    svchost.exe     6       SeMachineAccountPrivilege               Add workstations to the domain
1164    svchost.exe     7       SeTcbPrivilege          Act as part of the operating system
1164    svchost.exe     8       SeSecurityPrivilege             Manage auditing and security log
1164    svchost.exe     9       SeTakeOwnershipPrivilege                Take ownership of files/objects
1164    svchost.exe     10      SeLoadDriverPrivilege           Load and unload device drivers
1164    svchost.exe     11      SeSystemProfilePrivilege                Profile system performance
1164    svchost.exe     12      SeSystemtimePrivilege           Change the system time
1164    svchost.exe     13      SeProfileSingleProcessPrivilege         Profile a single process
1164    svchost.exe     14      SeIncreaseBasePriorityPrivilege         Increase scheduling priority
1164    svchost.exe     15      SeCreatePagefilePrivilege               Create a pagefile
1164    svchost.exe     16      SeCreatePermanentPrivilege              Create permanent shared objects
1164    svchost.exe     17      SeBackupPrivilege               Backup files and directories
1164    svchost.exe     18      SeRestorePrivilege              Restore files and directories
1164    svchost.exe     19      SeShutdownPrivilege             Shut down the system
1164    svchost.exe     20      SeDebugPrivilege                Debug programs
1164    svchost.exe     21      SeAuditPrivilege        Present,Enabled Generate security audits
1164    svchost.exe     22      SeSystemEnvironmentPrivilege            Edit firmware environment values
1164    svchost.exe     23      SeChangeNotifyPrivilege Present,Enabled,Default Receive notifications of changes to files or directories
1164    svchost.exe     24      SeRemoteShutdownPrivilege               Force shutdown from a remote system
1164    svchost.exe     25      SeUndockPrivilege               Remove computer from docking station
1164    svchost.exe     26      SeSyncAgentPrivilege            Synch directory service data
1164    svchost.exe     27      SeEnableDelegationPrivilege             Enable user accounts to be trusted for delegation
1164    svchost.exe     28      SeManageVolumePrivilege         Manage the files on a volume
1164    svchost.exe     29      SeImpersonatePrivilege  Present,Enabled,Default Impersonate a client after authentication
1164    svchost.exe     30      SeCreateGlobalPrivilege Present,Enabled,Default Create global objects
1164    svchost.exe     31      SeTrustedCredManAccessPrivilege         Access Credential Manager as a trusted caller
1164    svchost.exe     32      SeRelabelPrivilege              Modify the mandatory integrity level of an object
1164    svchost.exe     33      SeIncreaseWorkingSetPrivilege           Allocate more memory for user applications
1164    svchost.exe     34      SeTimeZonePrivilege             Adjust the time zone of the computer's internal clock
1164    svchost.exe     35      SeCreateSymbolicLinkPrivilege           Required to create a symbolic link
1164    svchost.exe     36      SeDelegateSessionUserImpersonatePrivilege               Obtain an impersonation token for another user in the same session.
1356    VGAuthService.  2       SeCreateTokenPrivilege          Create a token object
1356    VGAuthService.  3       SeAssignPrimaryTokenPrivilege   Present Replace a process-level token
1356    VGAuthService.  4       SeLockMemoryPrivilege   Present,Enabled,Default Lock pages in memory
1356    VGAuthService.  5       SeIncreaseQuotaPrivilege        Present Increase quotas
1356    VGAuthService.  6       SeMachineAccountPrivilege               Add workstations to the domain
1356    VGAuthService.  7       SeTcbPrivilege  Present,Enabled,Default Act as part of the operating system
1356    VGAuthService.  8       SeSecurityPrivilege     Present Manage auditing and security log
1356    VGAuthService.  9       SeTakeOwnershipPrivilege        Present Take ownership of files/objects
1356    VGAuthService.  10      SeLoadDriverPrivilege   Present Load and unload device drivers
1356    VGAuthService.  11      SeSystemProfilePrivilege        Present,Enabled,Default Profile system performance
1356    VGAuthService.  12      SeSystemtimePrivilege   Present Change the system time
1356    VGAuthService.  13      SeProfileSingleProcessPrivilege Present,Enabled,Default Profile a single process
1356    VGAuthService.  14      SeIncreaseBasePriorityPrivilege Present,Enabled,Default Increase scheduling priority
1356    VGAuthService.  15      SeCreatePagefilePrivilege       Present,Enabled,Default Create a pagefile
1356    VGAuthService.  16      SeCreatePermanentPrivilege      Present,Enabled,Default Create permanent shared objects
1356    VGAuthService.  17      SeBackupPrivilege       Present Backup files and directories
1356    VGAuthService.  18      SeRestorePrivilege      Present Restore files and directories
1356    VGAuthService.  19      SeShutdownPrivilege     Present Shut down the system
1356    VGAuthService.  20      SeDebugPrivilege        Present,Enabled,Default Debug programs
1356    VGAuthService.  21      SeAuditPrivilege        Present,Enabled,Default Generate security audits
1356    VGAuthService.  22      SeSystemEnvironmentPrivilege    Present Edit firmware environment values
1356    VGAuthService.  23      SeChangeNotifyPrivilege Present,Enabled,Default Receive notifications of changes to files or directories
1356    VGAuthService.  24      SeRemoteShutdownPrivilege               Force shutdown from a remote system
1356    VGAuthService.  25      SeUndockPrivilege       Present Remove computer from docking station
1356    VGAuthService.  26      SeSyncAgentPrivilege            Synch directory service data
1356    VGAuthService.  27      SeEnableDelegationPrivilege             Enable user accounts to be trusted for delegation
1356    VGAuthService.  28      SeManageVolumePrivilege Present Manage the files on a volume
1356    VGAuthService.  29      SeImpersonatePrivilege  Present,Enabled,Default Impersonate a client after authentication
1356    VGAuthService.  30      SeCreateGlobalPrivilege Present,Enabled,Default Create global objects
1356    VGAuthService.  31      SeTrustedCredManAccessPrivilege         Access Credential Manager as a trusted caller
1356    VGAuthService.  32      SeRelabelPrivilege              Modify the mandatory integrity level of an object
1356    VGAuthService.  33      SeIncreaseWorkingSetPrivilege   Present,Enabled,Default Allocate more memory for user applications
1356    VGAuthService.  34      SeTimeZonePrivilege     Present,Enabled,Default Adjust the time zone of the computer's internal clock
1356    VGAuthService.  35      SeCreateSymbolicLinkPrivilege   Present,Enabled,Default Required to create a symbolic link
1356    VGAuthService.  36      SeDelegateSessionUserImpersonatePrivilege               Obtain an impersonation token for another user in the same session.
1428    vmtoolsd.exe    2       SeCreateTokenPrivilege          Create a token object
1428    vmtoolsd.exe    3       SeAssignPrimaryTokenPrivilege   Present Replace a process-level token
1428    vmtoolsd.exe    4       SeLockMemoryPrivilege   Present,Enabled,Default Lock pages in memory
1428    vmtoolsd.exe    5       SeIncreaseQuotaPrivilege        Present Increase quotas
1428    vmtoolsd.exe    6       SeMachineAccountPrivilege               Add workstations to the domain
1428    vmtoolsd.exe    7       SeTcbPrivilege  Present,Enabled,Default Act as part of the operating system
1428    vmtoolsd.exe    8       SeSecurityPrivilege     Present Manage auditing and security log
1428    vmtoolsd.exe    9       SeTakeOwnershipPrivilege        Present Take ownership of files/objects
1428    vmtoolsd.exe    10      SeLoadDriverPrivilege   Present Load and unload device drivers
1428    vmtoolsd.exe    11      SeSystemProfilePrivilege        Present,Enabled,Default Profile system performance
1428    vmtoolsd.exe    12      SeSystemtimePrivilege   Present Change the system time
1428    vmtoolsd.exe    13      SeProfileSingleProcessPrivilege Present,Enabled,Default Profile a single process
1428    vmtoolsd.exe    14      SeIncreaseBasePriorityPrivilege Present,Enabled,Default Increase scheduling priority
1428    vmtoolsd.exe    15      SeCreatePagefilePrivilege       Present,Enabled,Default Create a pagefile
1428    vmtoolsd.exe    16      SeCreatePermanentPrivilege      Present,Enabled,Default Create permanent shared objects
1428    vmtoolsd.exe    17      SeBackupPrivilege       Present Backup files and directories
1428    vmtoolsd.exe    18      SeRestorePrivilege      Present Restore files and directories
1428    vmtoolsd.exe    19      SeShutdownPrivilege     Present Shut down the system
1428    vmtoolsd.exe    20      SeDebugPrivilege        Present,Enabled,Default Debug programs
1428    vmtoolsd.exe    21      SeAuditPrivilege        Present,Enabled,Default Generate security audits
1428    vmtoolsd.exe    22      SeSystemEnvironmentPrivilege    Present Edit firmware environment values
1428    vmtoolsd.exe    23      SeChangeNotifyPrivilege Present,Enabled,Default Receive notifications of changes to files or directories
1428    vmtoolsd.exe    24      SeRemoteShutdownPrivilege               Force shutdown from a remote system
1428    vmtoolsd.exe    25      SeUndockPrivilege       Present Remove computer from docking station
1428    vmtoolsd.exe    26      SeSyncAgentPrivilege            Synch directory service data
1428    vmtoolsd.exe    27      SeEnableDelegationPrivilege             Enable user accounts to be trusted for delegation
1428    vmtoolsd.exe    28      SeManageVolumePrivilege Present Manage the files on a volume
1428    vmtoolsd.exe    29      SeImpersonatePrivilege  Present,Enabled,Default Impersonate a client after authentication
1428    vmtoolsd.exe    30      SeCreateGlobalPrivilege Present,Enabled,Default Create global objects
1428    vmtoolsd.exe    31      SeTrustedCredManAccessPrivilege         Access Credential Manager as a trusted caller
1428    vmtoolsd.exe    32      SeRelabelPrivilege              Modify the mandatory integrity level of an object
1428    vmtoolsd.exe    33      SeIncreaseWorkingSetPrivilege   Present,Enabled,Default Allocate more memory for user applications
1428    vmtoolsd.exe    34      SeTimeZonePrivilege     Present,Enabled,Default Adjust the time zone of the computer's internal clock
1428    vmtoolsd.exe    35      SeCreateSymbolicLinkPrivilege   Present,Enabled,Default Required to create a symbolic link
1428    vmtoolsd.exe    36      SeDelegateSessionUserImpersonatePrivilege               Obtain an impersonation token for another user in the same session.
1800    WmiPrvSE.exe    2       SeCreateTokenPrivilege          Create a token object
1800    WmiPrvSE.exe    3       SeAssignPrimaryTokenPrivilege   Present Replace a process-level token
1800    WmiPrvSE.exe    4       SeLockMemoryPrivilege           Lock pages in memory
1800    WmiPrvSE.exe    5       SeIncreaseQuotaPrivilege        Present Increase quotas
1800    WmiPrvSE.exe    6       SeMachineAccountPrivilege               Add workstations to the domain
1800    WmiPrvSE.exe    7       SeTcbPrivilege          Act as part of the operating system
1800    WmiPrvSE.exe    8       SeSecurityPrivilege             Manage auditing and security log
1800    WmiPrvSE.exe    9       SeTakeOwnershipPrivilege                Take ownership of files/objects
1800    WmiPrvSE.exe    10      SeLoadDriverPrivilege           Load and unload device drivers
1800    WmiPrvSE.exe    11      SeSystemProfilePrivilege                Profile system performance
1800    WmiPrvSE.exe    12      SeSystemtimePrivilege           Change the system time
1800    WmiPrvSE.exe    13      SeProfileSingleProcessPrivilege         Profile a single process
1800    WmiPrvSE.exe    14      SeIncreaseBasePriorityPrivilege         Increase scheduling priority
1800    WmiPrvSE.exe    15      SeCreatePagefilePrivilege               Create a pagefile
1800    WmiPrvSE.exe    16      SeCreatePermanentPrivilege              Create permanent shared objects
1800    WmiPrvSE.exe    17      SeBackupPrivilege               Backup files and directories
1800    WmiPrvSE.exe    18      SeRestorePrivilege              Restore files and directories
1800    WmiPrvSE.exe    19      SeShutdownPrivilege     Present Shut down the system
1800    WmiPrvSE.exe    20      SeDebugPrivilege                Debug programs
1800    WmiPrvSE.exe    21      SeAuditPrivilege        Present Generate security audits
1800    WmiPrvSE.exe    22      SeSystemEnvironmentPrivilege            Edit firmware environment values
1800    WmiPrvSE.exe    23      SeChangeNotifyPrivilege Present,Enabled,Default Receive notifications of changes to files or directories
1800    WmiPrvSE.exe    24      SeRemoteShutdownPrivilege               Force shutdown from a remote system
1800    WmiPrvSE.exe    25      SeUndockPrivilege       Present Remove computer from docking station
1800    WmiPrvSE.exe    26      SeSyncAgentPrivilege            Synch directory service data
1800    WmiPrvSE.exe    27      SeEnableDelegationPrivilege             Enable user accounts to be trusted for delegation
1800    WmiPrvSE.exe    28      SeManageVolumePrivilege         Manage the files on a volume
1800    WmiPrvSE.exe    29      SeImpersonatePrivilege  Present,Enabled,Default Impersonate a client after authentication
1800    WmiPrvSE.exe    30      SeCreateGlobalPrivilege Present,Enabled,Default Create global objects
1800    WmiPrvSE.exe    31      SeTrustedCredManAccessPrivilege         Access Credential Manager as a trusted caller
1800    WmiPrvSE.exe    32      SeRelabelPrivilege              Modify the mandatory integrity level of an object
1800    WmiPrvSE.exe    33      SeIncreaseWorkingSetPrivilege   Present Allocate more memory for user applications
1800    WmiPrvSE.exe    34      SeTimeZonePrivilege     Present Adjust the time zone of the computer's internal clock
1800    WmiPrvSE.exe    35      SeCreateSymbolicLinkPrivilege           Required to create a symbolic link
1800    WmiPrvSE.exe    36      SeDelegateSessionUserImpersonatePrivilege               Obtain an impersonation token for another user in the same session.
1948    svchost.exe     2       SeCreateTokenPrivilege          Create a token object
1948    svchost.exe     3       SeAssignPrimaryTokenPrivilege           Replace a process-level token
1948    svchost.exe     4       SeLockMemoryPrivilege           Lock pages in memory
1948    svchost.exe     5       SeIncreaseQuotaPrivilege                Increase quotas
1948    svchost.exe     6       SeMachineAccountPrivilege               Add workstations to the domain
1948    svchost.exe     7       SeTcbPrivilege          Act as part of the operating system
1948    svchost.exe     8       SeSecurityPrivilege             Manage auditing and security log
1948    svchost.exe     9       SeTakeOwnershipPrivilege                Take ownership of files/objects
1948    svchost.exe     10      SeLoadDriverPrivilege           Load and unload device drivers
1948    svchost.exe     11      SeSystemProfilePrivilege                Profile system performance
1948    svchost.exe     12      SeSystemtimePrivilege           Change the system time
1948    svchost.exe     13      SeProfileSingleProcessPrivilege         Profile a single process
1948    svchost.exe     14      SeIncreaseBasePriorityPrivilege         Increase scheduling priority
1948    svchost.exe     15      SeCreatePagefilePrivilege               Create a pagefile
1948    svchost.exe     16      SeCreatePermanentPrivilege              Create permanent shared objects
1948    svchost.exe     17      SeBackupPrivilege               Backup files and directories
1948    svchost.exe     18      SeRestorePrivilege              Restore files and directories
1948    svchost.exe     19      SeShutdownPrivilege             Shut down the system
1948    svchost.exe     20      SeDebugPrivilege                Debug programs
1948    svchost.exe     21      SeAuditPrivilege                Generate security audits
1948    svchost.exe     22      SeSystemEnvironmentPrivilege            Edit firmware environment values
1948    svchost.exe     23      SeChangeNotifyPrivilege Present,Enabled,Default Receive notifications of changes to files or directories
1948    svchost.exe     24      SeRemoteShutdownPrivilege               Force shutdown from a remote system
1948    svchost.exe     25      SeUndockPrivilege               Remove computer from docking station
1948    svchost.exe     26      SeSyncAgentPrivilege            Synch directory service data
1948    svchost.exe     27      SeEnableDelegationPrivilege             Enable user accounts to be trusted for delegation
1948    svchost.exe     28      SeManageVolumePrivilege         Manage the files on a volume
1948    svchost.exe     29      SeImpersonatePrivilege  Present,Enabled,Default Impersonate a client after authentication
1948    svchost.exe     30      SeCreateGlobalPrivilege Present,Enabled,Default Create global objects
1948    svchost.exe     31      SeTrustedCredManAccessPrivilege         Access Credential Manager as a trusted caller
1948    svchost.exe     32      SeRelabelPrivilege              Modify the mandatory integrity level of an object
1948    svchost.exe     33      SeIncreaseWorkingSetPrivilege           Allocate more memory for user applications
1948    svchost.exe     34      SeTimeZonePrivilege             Adjust the time zone of the computer's internal clock
1948    svchost.exe     35      SeCreateSymbolicLinkPrivilege           Required to create a symbolic link
1948    svchost.exe     36      SeDelegateSessionUserImpersonatePrivilege               Obtain an impersonation token for another user in the same session.
1324    dllhost.exe     2       SeCreateTokenPrivilege          Create a token object
1324    dllhost.exe     3       SeAssignPrimaryTokenPrivilege   Present Replace a process-level token
1324    dllhost.exe     4       SeLockMemoryPrivilege   Default Lock pages in memory
1324    dllhost.exe     5       SeIncreaseQuotaPrivilege        Present Increase quotas
1324    dllhost.exe     6       SeMachineAccountPrivilege               Add workstations to the domain
1324    dllhost.exe     7       SeTcbPrivilege  Default Act as part of the operating system
1324    dllhost.exe     8       SeSecurityPrivilege             Manage auditing and security log
1324    dllhost.exe     9       SeTakeOwnershipPrivilege                Take ownership of files/objects
1324    dllhost.exe     10      SeLoadDriverPrivilege           Load and unload device drivers
1324    dllhost.exe     11      SeSystemProfilePrivilege        Default Profile system performance
1324    dllhost.exe     12      SeSystemtimePrivilege           Change the system time
1324    dllhost.exe     13      SeProfileSingleProcessPrivilege Default Profile a single process
1324    dllhost.exe     14      SeIncreaseBasePriorityPrivilege Default Increase scheduling priority
1324    dllhost.exe     15      SeCreatePagefilePrivilege       Default Create a pagefile
1324    dllhost.exe     16      SeCreatePermanentPrivilege      Default Create permanent shared objects
1324    dllhost.exe     17      SeBackupPrivilege               Backup files and directories
1324    dllhost.exe     18      SeRestorePrivilege              Restore files and directories
1324    dllhost.exe     19      SeShutdownPrivilege             Shut down the system
1324    dllhost.exe     20      SeDebugPrivilege        Present,Enabled,Default Debug programs
1324    dllhost.exe     21      SeAuditPrivilege        Present,Enabled,Default Generate security audits
1324    dllhost.exe     22      SeSystemEnvironmentPrivilege            Edit firmware environment values
1324    dllhost.exe     23      SeChangeNotifyPrivilege Present,Enabled,Default Receive notifications of changes to files or directories
1324    dllhost.exe     24      SeRemoteShutdownPrivilege               Force shutdown from a remote system
1324    dllhost.exe     25      SeUndockPrivilege               Remove computer from docking station
1324    dllhost.exe     26      SeSyncAgentPrivilege            Synch directory service data
1324    dllhost.exe     27      SeEnableDelegationPrivilege             Enable user accounts to be trusted for delegation
1324    dllhost.exe     28      SeManageVolumePrivilege         Manage the files on a volume
1324    dllhost.exe     29      SeImpersonatePrivilege  Present,Enabled,Default Impersonate a client after authentication
1324    dllhost.exe     30      SeCreateGlobalPrivilege Present,Enabled,Default Create global objects
1324    dllhost.exe     31      SeTrustedCredManAccessPrivilege         Access Credential Manager as a trusted caller
1324    dllhost.exe     32      SeRelabelPrivilege              Modify the mandatory integrity level of an object
1324    dllhost.exe     33      SeIncreaseWorkingSetPrivilege   Default Allocate more memory for user applications
1324    dllhost.exe     34      SeTimeZonePrivilege     Default Adjust the time zone of the computer's internal clock
1324    dllhost.exe     35      SeCreateSymbolicLinkPrivilege   Default Required to create a symbolic link
1324    dllhost.exe     36      SeDelegateSessionUserImpersonatePrivilege               Obtain an impersonation token for another user in the same session.
1436    msdtc.exe       2       SeCreateTokenPrivilege          Create a token object
1436    msdtc.exe       3       SeAssignPrimaryTokenPrivilege           Replace a process-level token
1436    msdtc.exe       4       SeLockMemoryPrivilege           Lock pages in memory
1436    msdtc.exe       5       SeIncreaseQuotaPrivilege                Increase quotas
1436    msdtc.exe       6       SeMachineAccountPrivilege               Add workstations to the domain
1436    msdtc.exe       7       SeTcbPrivilege          Act as part of the operating system
1436    msdtc.exe       8       SeSecurityPrivilege             Manage auditing and security log
1436    msdtc.exe       9       SeTakeOwnershipPrivilege                Take ownership of files/objects
1436    msdtc.exe       10      SeLoadDriverPrivilege           Load and unload device drivers
1436    msdtc.exe       11      SeSystemProfilePrivilege                Profile system performance
1436    msdtc.exe       12      SeSystemtimePrivilege           Change the system time
1436    msdtc.exe       13      SeProfileSingleProcessPrivilege         Profile a single process
1436    msdtc.exe       14      SeIncreaseBasePriorityPrivilege         Increase scheduling priority
1436    msdtc.exe       15      SeCreatePagefilePrivilege               Create a pagefile
1436    msdtc.exe       16      SeCreatePermanentPrivilege              Create permanent shared objects
1436    msdtc.exe       17      SeBackupPrivilege               Backup files and directories
1436    msdtc.exe       18      SeRestorePrivilege              Restore files and directories
1436    msdtc.exe       19      SeShutdownPrivilege             Shut down the system
1436    msdtc.exe       20      SeDebugPrivilege                Debug programs
1436    msdtc.exe       21      SeAuditPrivilege                Generate security audits
1436    msdtc.exe       22      SeSystemEnvironmentPrivilege            Edit firmware environment values
1436    msdtc.exe       23      SeChangeNotifyPrivilege Present,Enabled,Default Receive notifications of changes to files or directories
1436    msdtc.exe       24      SeRemoteShutdownPrivilege               Force shutdown from a remote system
1436    msdtc.exe       25      SeUndockPrivilege               Remove computer from docking station
1436    msdtc.exe       26      SeSyncAgentPrivilege            Synch directory service data
1436    msdtc.exe       27      SeEnableDelegationPrivilege             Enable user accounts to be trusted for delegation
1436    msdtc.exe       28      SeManageVolumePrivilege         Manage the files on a volume
1436    msdtc.exe       29      SeImpersonatePrivilege  Default Impersonate a client after authentication
1436    msdtc.exe       30      SeCreateGlobalPrivilege Present,Enabled,Default Create global objects
1436    msdtc.exe       31      SeTrustedCredManAccessPrivilege         Access Credential Manager as a trusted caller
1436    msdtc.exe       32      SeRelabelPrivilege              Modify the mandatory integrity level of an object
1436    msdtc.exe       33      SeIncreaseWorkingSetPrivilege           Allocate more memory for user applications
1436    msdtc.exe       34      SeTimeZonePrivilege             Adjust the time zone of the computer's internal clock
1436    msdtc.exe       35      SeCreateSymbolicLinkPrivilege           Required to create a symbolic link
1436    msdtc.exe       36      SeDelegateSessionUserImpersonatePrivilege               Obtain an impersonation token for another user in the same session.
2136    WmiPrvSE.exe    2       SeCreateTokenPrivilege          Create a token object
2136    WmiPrvSE.exe    3       SeAssignPrimaryTokenPrivilege   Present Replace a process-level token
2136    WmiPrvSE.exe    4       SeLockMemoryPrivilege   Present,Enabled,Default Lock pages in memory
2136    WmiPrvSE.exe    5       SeIncreaseQuotaPrivilege        Present Increase quotas
2136    WmiPrvSE.exe    6       SeMachineAccountPrivilege               Add workstations to the domain
2136    WmiPrvSE.exe    7       SeTcbPrivilege  Present,Enabled,Default Act as part of the operating system
2136    WmiPrvSE.exe    8       SeSecurityPrivilege     Present Manage auditing and security log
2136    WmiPrvSE.exe    9       SeTakeOwnershipPrivilege        Present Take ownership of files/objects
2136    WmiPrvSE.exe    10      SeLoadDriverPrivilege   Present Load and unload device drivers
2136    WmiPrvSE.exe    11      SeSystemProfilePrivilege        Present,Enabled,Default Profile system performance
2136    WmiPrvSE.exe    12      SeSystemtimePrivilege   Present Change the system time
2136    WmiPrvSE.exe    13      SeProfileSingleProcessPrivilege Present,Enabled,Default Profile a single process
2136    WmiPrvSE.exe    14      SeIncreaseBasePriorityPrivilege Present,Enabled,Default Increase scheduling priority
2136    WmiPrvSE.exe    15      SeCreatePagefilePrivilege       Present,Enabled,Default Create a pagefile
2136    WmiPrvSE.exe    16      SeCreatePermanentPrivilege      Present,Enabled,Default Create permanent shared objects
2136    WmiPrvSE.exe    17      SeBackupPrivilege       Present Backup files and directories
2136    WmiPrvSE.exe    18      SeRestorePrivilege      Present Restore files and directories
2136    WmiPrvSE.exe    19      SeShutdownPrivilege     Present Shut down the system
2136    WmiPrvSE.exe    20      SeDebugPrivilege        Present,Default Debug programs
2136    WmiPrvSE.exe    21      SeAuditPrivilege        Present,Enabled,Default Generate security audits
2136    WmiPrvSE.exe    22      SeSystemEnvironmentPrivilege    Present Edit firmware environment values
2136    WmiPrvSE.exe    23      SeChangeNotifyPrivilege Present,Enabled,Default Receive notifications of changes to files or directories
2136    WmiPrvSE.exe    24      SeRemoteShutdownPrivilege               Force shutdown from a remote system
2136    WmiPrvSE.exe    25      SeUndockPrivilege       Present Remove computer from docking station
2136    WmiPrvSE.exe    26      SeSyncAgentPrivilege            Synch directory service data
2136    WmiPrvSE.exe    27      SeEnableDelegationPrivilege             Enable user accounts to be trusted for delegation
2136    WmiPrvSE.exe    28      SeManageVolumePrivilege Present Manage the files on a volume
2136    WmiPrvSE.exe    29      SeImpersonatePrivilege  Present,Enabled,Default Impersonate a client after authentication
2136    WmiPrvSE.exe    30      SeCreateGlobalPrivilege Present,Enabled,Default Create global objects
2136    WmiPrvSE.exe    31      SeTrustedCredManAccessPrivilege         Access Credential Manager as a trusted caller
2136    WmiPrvSE.exe    32      SeRelabelPrivilege              Modify the mandatory integrity level of an object
2136    WmiPrvSE.exe    33      SeIncreaseWorkingSetPrivilege   Present,Enabled,Default Allocate more memory for user applications
2136    WmiPrvSE.exe    34      SeTimeZonePrivilege     Present,Enabled,Default Adjust the time zone of the computer's internal clock
2136    WmiPrvSE.exe    35      SeCreateSymbolicLinkPrivilege   Present,Enabled,Default Required to create a symbolic link
2136    WmiPrvSE.exe    36      SeDelegateSessionUserImpersonatePrivilege               Obtain an impersonation token for another user in the same session.
2344    taskhost.exe    2       SeCreateTokenPrivilege          Create a token object
2344    taskhost.exe    3       SeAssignPrimaryTokenPrivilege           Replace a process-level token
2344    taskhost.exe    4       SeLockMemoryPrivilege           Lock pages in memory
2344    taskhost.exe    5       SeIncreaseQuotaPrivilege                Increase quotas
2344    taskhost.exe    6       SeMachineAccountPrivilege               Add workstations to the domain
2344    taskhost.exe    7       SeTcbPrivilege          Act as part of the operating system
2344    taskhost.exe    8       SeSecurityPrivilege             Manage auditing and security log
2344    taskhost.exe    9       SeTakeOwnershipPrivilege                Take ownership of files/objects
2344    taskhost.exe    10      SeLoadDriverPrivilege           Load and unload device drivers
2344    taskhost.exe    11      SeSystemProfilePrivilege                Profile system performance
2344    taskhost.exe    12      SeSystemtimePrivilege           Change the system time
2344    taskhost.exe    13      SeProfileSingleProcessPrivilege         Profile a single process
2344    taskhost.exe    14      SeIncreaseBasePriorityPrivilege         Increase scheduling priority
2344    taskhost.exe    15      SeCreatePagefilePrivilege               Create a pagefile
2344    taskhost.exe    16      SeCreatePermanentPrivilege              Create permanent shared objects
2344    taskhost.exe    17      SeBackupPrivilege               Backup files and directories
2344    taskhost.exe    18      SeRestorePrivilege              Restore files and directories
2344    taskhost.exe    19      SeShutdownPrivilege     Present Shut down the system
2344    taskhost.exe    20      SeDebugPrivilege                Debug programs
2344    taskhost.exe    21      SeAuditPrivilege                Generate security audits
2344    taskhost.exe    22      SeSystemEnvironmentPrivilege            Edit firmware environment values
2344    taskhost.exe    23      SeChangeNotifyPrivilege Present,Enabled,Default Receive notifications of changes to files or directories
2344    taskhost.exe    24      SeRemoteShutdownPrivilege               Force shutdown from a remote system
2344    taskhost.exe    25      SeUndockPrivilege       Present Remove computer from docking station
2344    taskhost.exe    26      SeSyncAgentPrivilege            Synch directory service data
2344    taskhost.exe    27      SeEnableDelegationPrivilege             Enable user accounts to be trusted for delegation
2344    taskhost.exe    28      SeManageVolumePrivilege         Manage the files on a volume
2344    taskhost.exe    29      SeImpersonatePrivilege          Impersonate a client after authentication
2344    taskhost.exe    30      SeCreateGlobalPrivilege         Create global objects
2344    taskhost.exe    31      SeTrustedCredManAccessPrivilege         Access Credential Manager as a trusted caller
2344    taskhost.exe    32      SeRelabelPrivilege              Modify the mandatory integrity level of an object
2344    taskhost.exe    33      SeIncreaseWorkingSetPrivilege   Present Allocate more memory for user applications
2344    taskhost.exe    34      SeTimeZonePrivilege     Present Adjust the time zone of the computer's internal clock
2344    taskhost.exe    35      SeCreateSymbolicLinkPrivilege           Required to create a symbolic link
2344    taskhost.exe    36      SeDelegateSessionUserImpersonatePrivilege               Obtain an impersonation token for another user in the same session.
2500    sppsvc.exe      2       SeCreateTokenPrivilege          Create a token object
2500    sppsvc.exe      3       SeAssignPrimaryTokenPrivilege           Replace a process-level token
2500    sppsvc.exe      4       SeLockMemoryPrivilege           Lock pages in memory
2500    sppsvc.exe      5       SeIncreaseQuotaPrivilege                Increase quotas
2500    sppsvc.exe      6       SeMachineAccountPrivilege               Add workstations to the domain
2500    sppsvc.exe      7       SeTcbPrivilege          Act as part of the operating system
2500    sppsvc.exe      8       SeSecurityPrivilege             Manage auditing and security log
2500    sppsvc.exe      9       SeTakeOwnershipPrivilege                Take ownership of files/objects
2500    sppsvc.exe      10      SeLoadDriverPrivilege           Load and unload device drivers
2500    sppsvc.exe      11      SeSystemProfilePrivilege                Profile system performance
2500    sppsvc.exe      12      SeSystemtimePrivilege           Change the system time
2500    sppsvc.exe      13      SeProfileSingleProcessPrivilege         Profile a single process
2500    sppsvc.exe      14      SeIncreaseBasePriorityPrivilege         Increase scheduling priority
2500    sppsvc.exe      15      SeCreatePagefilePrivilege               Create a pagefile
2500    sppsvc.exe      16      SeCreatePermanentPrivilege              Create permanent shared objects
2500    sppsvc.exe      17      SeBackupPrivilege               Backup files and directories
2500    sppsvc.exe      18      SeRestorePrivilege              Restore files and directories
2500    sppsvc.exe      19      SeShutdownPrivilege             Shut down the system
2500    sppsvc.exe      20      SeDebugPrivilege                Debug programs
2500    sppsvc.exe      21      SeAuditPrivilege        Present Generate security audits
2500    sppsvc.exe      22      SeSystemEnvironmentPrivilege            Edit firmware environment values
2500    sppsvc.exe      23      SeChangeNotifyPrivilege Present,Enabled,Default Receive notifications of changes to files or directories
2500    sppsvc.exe      24      SeRemoteShutdownPrivilege               Force shutdown from a remote system
2500    sppsvc.exe      25      SeUndockPrivilege               Remove computer from docking station
2500    sppsvc.exe      26      SeSyncAgentPrivilege            Synch directory service data
2500    sppsvc.exe      27      SeEnableDelegationPrivilege             Enable user accounts to be trusted for delegation
2500    sppsvc.exe      28      SeManageVolumePrivilege         Manage the files on a volume
2500    sppsvc.exe      29      SeImpersonatePrivilege  Present,Enabled,Default Impersonate a client after authentication
2500    sppsvc.exe      30      SeCreateGlobalPrivilege Present,Enabled,Default Create global objects
2500    sppsvc.exe      31      SeTrustedCredManAccessPrivilege         Access Credential Manager as a trusted caller
2500    sppsvc.exe      32      SeRelabelPrivilege              Modify the mandatory integrity level of an object
2500    sppsvc.exe      33      SeIncreaseWorkingSetPrivilege           Allocate more memory for user applications
2500    sppsvc.exe      34      SeTimeZonePrivilege             Adjust the time zone of the computer's internal clock
2500    sppsvc.exe      35      SeCreateSymbolicLinkPrivilege           Required to create a symbolic link
2500    sppsvc.exe      36      SeDelegateSessionUserImpersonatePrivilege               Obtain an impersonation token for another user in the same session.
2704    dwm.exe 2       SeCreateTokenPrivilege          Create a token object
2704    dwm.exe 3       SeAssignPrimaryTokenPrivilege           Replace a process-level token
2704    dwm.exe 4       SeLockMemoryPrivilege           Lock pages in memory
2704    dwm.exe 5       SeIncreaseQuotaPrivilege                Increase quotas
2704    dwm.exe 6       SeMachineAccountPrivilege               Add workstations to the domain
2704    dwm.exe 7       SeTcbPrivilege          Act as part of the operating system
2704    dwm.exe 8       SeSecurityPrivilege             Manage auditing and security log
2704    dwm.exe 9       SeTakeOwnershipPrivilege                Take ownership of files/objects
2704    dwm.exe 10      SeLoadDriverPrivilege           Load and unload device drivers
2704    dwm.exe 11      SeSystemProfilePrivilege                Profile system performance
2704    dwm.exe 12      SeSystemtimePrivilege           Change the system time
2704    dwm.exe 13      SeProfileSingleProcessPrivilege         Profile a single process
2704    dwm.exe 14      SeIncreaseBasePriorityPrivilege         Increase scheduling priority
2704    dwm.exe 15      SeCreatePagefilePrivilege               Create a pagefile
2704    dwm.exe 16      SeCreatePermanentPrivilege              Create permanent shared objects
2704    dwm.exe 17      SeBackupPrivilege               Backup files and directories
2704    dwm.exe 18      SeRestorePrivilege              Restore files and directories
2704    dwm.exe 19      SeShutdownPrivilege     Present Shut down the system
2704    dwm.exe 20      SeDebugPrivilege                Debug programs
2704    dwm.exe 21      SeAuditPrivilege                Generate security audits
2704    dwm.exe 22      SeSystemEnvironmentPrivilege            Edit firmware environment values
2704    dwm.exe 23      SeChangeNotifyPrivilege Present,Enabled,Default Receive notifications of changes to files or directories
2704    dwm.exe 24      SeRemoteShutdownPrivilege               Force shutdown from a remote system
2704    dwm.exe 25      SeUndockPrivilege       Present Remove computer from docking station
2704    dwm.exe 26      SeSyncAgentPrivilege            Synch directory service data
2704    dwm.exe 27      SeEnableDelegationPrivilege             Enable user accounts to be trusted for delegation
2704    dwm.exe 28      SeManageVolumePrivilege         Manage the files on a volume
2704    dwm.exe 29      SeImpersonatePrivilege          Impersonate a client after authentication
2704    dwm.exe 30      SeCreateGlobalPrivilege         Create global objects
2704    dwm.exe 31      SeTrustedCredManAccessPrivilege         Access Credential Manager as a trusted caller
2704    dwm.exe 32      SeRelabelPrivilege              Modify the mandatory integrity level of an object
2704    dwm.exe 33      SeIncreaseWorkingSetPrivilege   Present Allocate more memory for user applications
2704    dwm.exe 34      SeTimeZonePrivilege     Present Adjust the time zone of the computer's internal clock
2704    dwm.exe 35      SeCreateSymbolicLinkPrivilege           Required to create a symbolic link
2704    dwm.exe 36      SeDelegateSessionUserImpersonatePrivilege               Obtain an impersonation token for another user in the same session.
2728    explorer.exe    2       SeCreateTokenPrivilege          Create a token object
2728    explorer.exe    3       SeAssignPrimaryTokenPrivilege           Replace a process-level token
2728    explorer.exe    4       SeLockMemoryPrivilege           Lock pages in memory
2728    explorer.exe    5       SeIncreaseQuotaPrivilege                Increase quotas
2728    explorer.exe    6       SeMachineAccountPrivilege               Add workstations to the domain
2728    explorer.exe    7       SeTcbPrivilege          Act as part of the operating system
2728    explorer.exe    8       SeSecurityPrivilege             Manage auditing and security log
2728    explorer.exe    9       SeTakeOwnershipPrivilege                Take ownership of files/objects
2728    explorer.exe    10      SeLoadDriverPrivilege           Load and unload device drivers
2728    explorer.exe    11      SeSystemProfilePrivilege                Profile system performance
2728    explorer.exe    12      SeSystemtimePrivilege           Change the system time
2728    explorer.exe    13      SeProfileSingleProcessPrivilege         Profile a single process
2728    explorer.exe    14      SeIncreaseBasePriorityPrivilege         Increase scheduling priority
2728    explorer.exe    15      SeCreatePagefilePrivilege               Create a pagefile
2728    explorer.exe    16      SeCreatePermanentPrivilege              Create permanent shared objects
2728    explorer.exe    17      SeBackupPrivilege               Backup files and directories
2728    explorer.exe    18      SeRestorePrivilege              Restore files and directories
2728    explorer.exe    19      SeShutdownPrivilege     Present Shut down the system
2728    explorer.exe    20      SeDebugPrivilege                Debug programs
2728    explorer.exe    21      SeAuditPrivilege                Generate security audits
2728    explorer.exe    22      SeSystemEnvironmentPrivilege            Edit firmware environment values
2728    explorer.exe    23      SeChangeNotifyPrivilege Present,Enabled,Default Receive notifications of changes to files or directories
2728    explorer.exe    24      SeRemoteShutdownPrivilege               Force shutdown from a remote system
2728    explorer.exe    25      SeUndockPrivilege       Present Remove computer from docking station
2728    explorer.exe    26      SeSyncAgentPrivilege            Synch directory service data
2728    explorer.exe    27      SeEnableDelegationPrivilege             Enable user accounts to be trusted for delegation
2728    explorer.exe    28      SeManageVolumePrivilege         Manage the files on a volume
2728    explorer.exe    29      SeImpersonatePrivilege          Impersonate a client after authentication
2728    explorer.exe    30      SeCreateGlobalPrivilege         Create global objects
2728    explorer.exe    31      SeTrustedCredManAccessPrivilege         Access Credential Manager as a trusted caller
2728    explorer.exe    32      SeRelabelPrivilege              Modify the mandatory integrity level of an object
2728    explorer.exe    33      SeIncreaseWorkingSetPrivilege   Present Allocate more memory for user applications
2728    explorer.exe    34      SeTimeZonePrivilege     Present Adjust the time zone of the computer's internal clock
2728    explorer.exe    35      SeCreateSymbolicLinkPrivilege           Required to create a symbolic link
2728    explorer.exe    36      SeDelegateSessionUserImpersonatePrivilege               Obtain an impersonation token for another user in the same session.
2804    vmtoolsd.exe    2       SeCreateTokenPrivilege          Create a token object
2804    vmtoolsd.exe    3       SeAssignPrimaryTokenPrivilege           Replace a process-level token
2804    vmtoolsd.exe    4       SeLockMemoryPrivilege           Lock pages in memory
2804    vmtoolsd.exe    5       SeIncreaseQuotaPrivilege                Increase quotas
2804    vmtoolsd.exe    6       SeMachineAccountPrivilege               Add workstations to the domain
2804    vmtoolsd.exe    7       SeTcbPrivilege          Act as part of the operating system
2804    vmtoolsd.exe    8       SeSecurityPrivilege             Manage auditing and security log
2804    vmtoolsd.exe    9       SeTakeOwnershipPrivilege                Take ownership of files/objects
2804    vmtoolsd.exe    10      SeLoadDriverPrivilege           Load and unload device drivers
2804    vmtoolsd.exe    11      SeSystemProfilePrivilege                Profile system performance
2804    vmtoolsd.exe    12      SeSystemtimePrivilege           Change the system time
2804    vmtoolsd.exe    13      SeProfileSingleProcessPrivilege         Profile a single process
2804    vmtoolsd.exe    14      SeIncreaseBasePriorityPrivilege         Increase scheduling priority
2804    vmtoolsd.exe    15      SeCreatePagefilePrivilege               Create a pagefile
2804    vmtoolsd.exe    16      SeCreatePermanentPrivilege              Create permanent shared objects
2804    vmtoolsd.exe    17      SeBackupPrivilege               Backup files and directories
2804    vmtoolsd.exe    18      SeRestorePrivilege              Restore files and directories
2804    vmtoolsd.exe    19      SeShutdownPrivilege     Present Shut down the system
2804    vmtoolsd.exe    20      SeDebugPrivilege                Debug programs
2804    vmtoolsd.exe    21      SeAuditPrivilege                Generate security audits
2804    vmtoolsd.exe    22      SeSystemEnvironmentPrivilege            Edit firmware environment values
2804    vmtoolsd.exe    23      SeChangeNotifyPrivilege Present,Enabled,Default Receive notifications of changes to files or directories
2804    vmtoolsd.exe    24      SeRemoteShutdownPrivilege               Force shutdown from a remote system
2804    vmtoolsd.exe    25      SeUndockPrivilege       Present Remove computer from docking station
2804    vmtoolsd.exe    26      SeSyncAgentPrivilege            Synch directory service data
2804    vmtoolsd.exe    27      SeEnableDelegationPrivilege             Enable user accounts to be trusted for delegation
2804    vmtoolsd.exe    28      SeManageVolumePrivilege         Manage the files on a volume
2804    vmtoolsd.exe    29      SeImpersonatePrivilege          Impersonate a client after authentication
2804    vmtoolsd.exe    30      SeCreateGlobalPrivilege         Create global objects
2804    vmtoolsd.exe    31      SeTrustedCredManAccessPrivilege         Access Credential Manager as a trusted caller
2804    vmtoolsd.exe    32      SeRelabelPrivilege              Modify the mandatory integrity level of an object
2804    vmtoolsd.exe    33      SeIncreaseWorkingSetPrivilege   Present Allocate more memory for user applications
2804    vmtoolsd.exe    34      SeTimeZonePrivilege     Present Adjust the time zone of the computer's internal clock
2804    vmtoolsd.exe    35      SeCreateSymbolicLinkPrivilege           Required to create a symbolic link
2804    vmtoolsd.exe    36      SeDelegateSessionUserImpersonatePrivilege               Obtain an impersonation token for another user in the same session.
2836    BitTorrent.exe  2       SeCreateTokenPrivilege          Create a token object
2836    BitTorrent.exe  3       SeAssignPrimaryTokenPrivilege           Replace a process-level token
2836    BitTorrent.exe  4       SeLockMemoryPrivilege           Lock pages in memory
2836    BitTorrent.exe  5       SeIncreaseQuotaPrivilege                Increase quotas
2836    BitTorrent.exe  6       SeMachineAccountPrivilege               Add workstations to the domain
2836    BitTorrent.exe  7       SeTcbPrivilege          Act as part of the operating system
2836    BitTorrent.exe  8       SeSecurityPrivilege             Manage auditing and security log
2836    BitTorrent.exe  9       SeTakeOwnershipPrivilege                Take ownership of files/objects
2836    BitTorrent.exe  10      SeLoadDriverPrivilege           Load and unload device drivers
2836    BitTorrent.exe  11      SeSystemProfilePrivilege                Profile system performance
2836    BitTorrent.exe  12      SeSystemtimePrivilege           Change the system time
2836    BitTorrent.exe  13      SeProfileSingleProcessPrivilege         Profile a single process
2836    BitTorrent.exe  14      SeIncreaseBasePriorityPrivilege         Increase scheduling priority
2836    BitTorrent.exe  15      SeCreatePagefilePrivilege               Create a pagefile
2836    BitTorrent.exe  16      SeCreatePermanentPrivilege              Create permanent shared objects
2836    BitTorrent.exe  17      SeBackupPrivilege               Backup files and directories
2836    BitTorrent.exe  18      SeRestorePrivilege              Restore files and directories
2836    BitTorrent.exe  19      SeShutdownPrivilege     Present Shut down the system
2836    BitTorrent.exe  20      SeDebugPrivilege                Debug programs
2836    BitTorrent.exe  21      SeAuditPrivilege                Generate security audits
2836    BitTorrent.exe  22      SeSystemEnvironmentPrivilege            Edit firmware environment values
2836    BitTorrent.exe  23      SeChangeNotifyPrivilege Present,Enabled,Default Receive notifications of changes to files or directories
2836    BitTorrent.exe  24      SeRemoteShutdownPrivilege               Force shutdown from a remote system
2836    BitTorrent.exe  25      SeUndockPrivilege       Present Remove computer from docking station
2836    BitTorrent.exe  26      SeSyncAgentPrivilege            Synch directory service data
2836    BitTorrent.exe  27      SeEnableDelegationPrivilege             Enable user accounts to be trusted for delegation
2836    BitTorrent.exe  28      SeManageVolumePrivilege         Manage the files on a volume
2836    BitTorrent.exe  29      SeImpersonatePrivilege          Impersonate a client after authentication
2836    BitTorrent.exe  30      SeCreateGlobalPrivilege         Create global objects
2836    BitTorrent.exe  31      SeTrustedCredManAccessPrivilege         Access Credential Manager as a trusted caller
2836    BitTorrent.exe  32      SeRelabelPrivilege              Modify the mandatory integrity level of an object
2836    BitTorrent.exe  33      SeIncreaseWorkingSetPrivilege   Present Allocate more memory for user applications
2836    BitTorrent.exe  34      SeTimeZonePrivilege     Present Adjust the time zone of the computer's internal clock
2836    BitTorrent.exe  35      SeCreateSymbolicLinkPrivilege           Required to create a symbolic link
2836    BitTorrent.exe  36      SeDelegateSessionUserImpersonatePrivilege               Obtain an impersonation token for another user in the same session.
2844    WebCompanion.e  2       SeCreateTokenPrivilege          Create a token object
2844    WebCompanion.e  3       SeAssignPrimaryTokenPrivilege           Replace a process-level token
2844    WebCompanion.e  4       SeLockMemoryPrivilege           Lock pages in memory
2844    WebCompanion.e  5       SeIncreaseQuotaPrivilege                Increase quotas
2844    WebCompanion.e  6       SeMachineAccountPrivilege               Add workstations to the domain
2844    WebCompanion.e  7       SeTcbPrivilege          Act as part of the operating system
2844    WebCompanion.e  8       SeSecurityPrivilege             Manage auditing and security log
2844    WebCompanion.e  9       SeTakeOwnershipPrivilege                Take ownership of files/objects
2844    WebCompanion.e  10      SeLoadDriverPrivilege           Load and unload device drivers
2844    WebCompanion.e  11      SeSystemProfilePrivilege                Profile system performance
2844    WebCompanion.e  12      SeSystemtimePrivilege           Change the system time
2844    WebCompanion.e  13      SeProfileSingleProcessPrivilege         Profile a single process
2844    WebCompanion.e  14      SeIncreaseBasePriorityPrivilege         Increase scheduling priority
2844    WebCompanion.e  15      SeCreatePagefilePrivilege               Create a pagefile
2844    WebCompanion.e  16      SeCreatePermanentPrivilege              Create permanent shared objects
2844    WebCompanion.e  17      SeBackupPrivilege               Backup files and directories
2844    WebCompanion.e  18      SeRestorePrivilege              Restore files and directories
2844    WebCompanion.e  19      SeShutdownPrivilege     Present Shut down the system
2844    WebCompanion.e  20      SeDebugPrivilege                Debug programs
2844    WebCompanion.e  21      SeAuditPrivilege                Generate security audits
2844    WebCompanion.e  22      SeSystemEnvironmentPrivilege            Edit firmware environment values
2844    WebCompanion.e  23      SeChangeNotifyPrivilege Present,Enabled,Default Receive notifications of changes to files or directories
2844    WebCompanion.e  24      SeRemoteShutdownPrivilege               Force shutdown from a remote system
2844    WebCompanion.e  25      SeUndockPrivilege       Present Remove computer from docking station
2844    WebCompanion.e  26      SeSyncAgentPrivilege            Synch directory service data
2844    WebCompanion.e  27      SeEnableDelegationPrivilege             Enable user accounts to be trusted for delegation
2844    WebCompanion.e  28      SeManageVolumePrivilege         Manage the files on a volume
2844    WebCompanion.e  29      SeImpersonatePrivilege          Impersonate a client after authentication
2844    WebCompanion.e  30      SeCreateGlobalPrivilege         Create global objects
2844    WebCompanion.e  31      SeTrustedCredManAccessPrivilege         Access Credential Manager as a trusted caller
2844    WebCompanion.e  32      SeRelabelPrivilege              Modify the mandatory integrity level of an object
2844    WebCompanion.e  33      SeIncreaseWorkingSetPrivilege   Present Allocate more memory for user applications
2844    WebCompanion.e  34      SeTimeZonePrivilege     Present Adjust the time zone of the computer's internal clock
2844    WebCompanion.e  35      SeCreateSymbolicLinkPrivilege           Required to create a symbolic link
2844    WebCompanion.e  36      SeDelegateSessionUserImpersonatePrivilege               Obtain an impersonation token for another user in the same session.
3064    SearchIndexer.  2       SeCreateTokenPrivilege          Create a token object
3064    SearchIndexer.  3       SeAssignPrimaryTokenPrivilege   Present Replace a process-level token
3064    SearchIndexer.  4       SeLockMemoryPrivilege   Default Lock pages in memory
3064    SearchIndexer.  5       SeIncreaseQuotaPrivilege        Present Increase quotas
3064    SearchIndexer.  6       SeMachineAccountPrivilege               Add workstations to the domain
3064    SearchIndexer.  7       SeTcbPrivilege  Present,Enabled,Default Act as part of the operating system
3064    SearchIndexer.  8       SeSecurityPrivilege             Manage auditing and security log
3064    SearchIndexer.  9       SeTakeOwnershipPrivilege                Take ownership of files/objects
3064    SearchIndexer.  10      SeLoadDriverPrivilege           Load and unload device drivers
3064    SearchIndexer.  11      SeSystemProfilePrivilege        Default Profile system performance
3064    SearchIndexer.  12      SeSystemtimePrivilege           Change the system time
3064    SearchIndexer.  13      SeProfileSingleProcessPrivilege Default Profile a single process
3064    SearchIndexer.  14      SeIncreaseBasePriorityPrivilege Default Increase scheduling priority
3064    SearchIndexer.  15      SeCreatePagefilePrivilege       Default Create a pagefile
3064    SearchIndexer.  16      SeCreatePermanentPrivilege      Default Create permanent shared objects
3064    SearchIndexer.  17      SeBackupPrivilege               Backup files and directories
3064    SearchIndexer.  18      SeRestorePrivilege              Restore files and directories
3064    SearchIndexer.  19      SeShutdownPrivilege             Shut down the system
3064    SearchIndexer.  20      SeDebugPrivilege        Default Debug programs
3064    SearchIndexer.  21      SeAuditPrivilege        Default Generate security audits
3064    SearchIndexer.  22      SeSystemEnvironmentPrivilege            Edit firmware environment values
3064    SearchIndexer.  23      SeChangeNotifyPrivilege Present,Enabled,Default Receive notifications of changes to files or directories
3064    SearchIndexer.  24      SeRemoteShutdownPrivilege               Force shutdown from a remote system
3064    SearchIndexer.  25      SeUndockPrivilege               Remove computer from docking station
3064    SearchIndexer.  26      SeSyncAgentPrivilege            Synch directory service data
3064    SearchIndexer.  27      SeEnableDelegationPrivilege             Enable user accounts to be trusted for delegation
3064    SearchIndexer.  28      SeManageVolumePrivilege Present Manage the files on a volume
3064    SearchIndexer.  29      SeImpersonatePrivilege  Present,Enabled,Default Impersonate a client after authentication
3064    SearchIndexer.  30      SeCreateGlobalPrivilege Default Create global objects
3064    SearchIndexer.  31      SeTrustedCredManAccessPrivilege         Access Credential Manager as a trusted caller
3064    SearchIndexer.  32      SeRelabelPrivilege              Modify the mandatory integrity level of an object
3064    SearchIndexer.  33      SeIncreaseWorkingSetPrivilege   Default Allocate more memory for user applications
3064    SearchIndexer.  34      SeTimeZonePrivilege     Default Adjust the time zone of the computer's internal clock
3064    SearchIndexer.  35      SeCreateSymbolicLinkPrivilege   Default Required to create a symbolic link
3064    SearchIndexer.  36      SeDelegateSessionUserImpersonatePrivilege               Obtain an impersonation token for another user in the same session.
2308    bittorrentie.e  2       SeCreateTokenPrivilege          Create a token object
2308    bittorrentie.e  3       SeAssignPrimaryTokenPrivilege           Replace a process-level token
2308    bittorrentie.e  4       SeLockMemoryPrivilege           Lock pages in memory
2308    bittorrentie.e  5       SeIncreaseQuotaPrivilege                Increase quotas
2308    bittorrentie.e  6       SeMachineAccountPrivilege               Add workstations to the domain
2308    bittorrentie.e  7       SeTcbPrivilege          Act as part of the operating system
2308    bittorrentie.e  8       SeSecurityPrivilege             Manage auditing and security log
2308    bittorrentie.e  9       SeTakeOwnershipPrivilege                Take ownership of files/objects
2308    bittorrentie.e  10      SeLoadDriverPrivilege           Load and unload device drivers
2308    bittorrentie.e  11      SeSystemProfilePrivilege                Profile system performance
2308    bittorrentie.e  12      SeSystemtimePrivilege           Change the system time
2308    bittorrentie.e  13      SeProfileSingleProcessPrivilege         Profile a single process
2308    bittorrentie.e  14      SeIncreaseBasePriorityPrivilege         Increase scheduling priority
2308    bittorrentie.e  15      SeCreatePagefilePrivilege               Create a pagefile
2308    bittorrentie.e  16      SeCreatePermanentPrivilege              Create permanent shared objects
2308    bittorrentie.e  17      SeBackupPrivilege               Backup files and directories
2308    bittorrentie.e  18      SeRestorePrivilege              Restore files and directories
2308    bittorrentie.e  19      SeShutdownPrivilege     Present Shut down the system
2308    bittorrentie.e  20      SeDebugPrivilege                Debug programs
2308    bittorrentie.e  21      SeAuditPrivilege                Generate security audits
2308    bittorrentie.e  22      SeSystemEnvironmentPrivilege            Edit firmware environment values
2308    bittorrentie.e  23      SeChangeNotifyPrivilege Present,Enabled,Default Receive notifications of changes to files or directories
2308    bittorrentie.e  24      SeRemoteShutdownPrivilege               Force shutdown from a remote system
2308    bittorrentie.e  25      SeUndockPrivilege       Present Remove computer from docking station
2308    bittorrentie.e  26      SeSyncAgentPrivilege            Synch directory service data
2308    bittorrentie.e  27      SeEnableDelegationPrivilege             Enable user accounts to be trusted for delegation
2308    bittorrentie.e  28      SeManageVolumePrivilege         Manage the files on a volume
2308    bittorrentie.e  29      SeImpersonatePrivilege          Impersonate a client after authentication
2308    bittorrentie.e  30      SeCreateGlobalPrivilege         Create global objects
2308    bittorrentie.e  31      SeTrustedCredManAccessPrivilege         Access Credential Manager as a trusted caller
2308    bittorrentie.e  32      SeRelabelPrivilege              Modify the mandatory integrity level of an object
2308    bittorrentie.e  33      SeIncreaseWorkingSetPrivilege   Present Allocate more memory for user applications
2308    bittorrentie.e  34      SeTimeZonePrivilege     Present Adjust the time zone of the computer's internal clock
2308    bittorrentie.e  35      SeCreateSymbolicLinkPrivilege           Required to create a symbolic link
2308    bittorrentie.e  36      SeDelegateSessionUserImpersonatePrivilege               Obtain an impersonation token for another user in the same session.
2624    bittorrentie.e  2       SeCreateTokenPrivilege          Create a token object
2624    bittorrentie.e  3       SeAssignPrimaryTokenPrivilege           Replace a process-level token
2624    bittorrentie.e  4       SeLockMemoryPrivilege           Lock pages in memory
2624    bittorrentie.e  5       SeIncreaseQuotaPrivilege                Increase quotas
2624    bittorrentie.e  6       SeMachineAccountPrivilege               Add workstations to the domain
2624    bittorrentie.e  7       SeTcbPrivilege          Act as part of the operating system
2624    bittorrentie.e  8       SeSecurityPrivilege             Manage auditing and security log
2624    bittorrentie.e  9       SeTakeOwnershipPrivilege                Take ownership of files/objects
2624    bittorrentie.e  10      SeLoadDriverPrivilege           Load and unload device drivers
2624    bittorrentie.e  11      SeSystemProfilePrivilege                Profile system performance
2624    bittorrentie.e  12      SeSystemtimePrivilege           Change the system time
2624    bittorrentie.e  13      SeProfileSingleProcessPrivilege         Profile a single process
2624    bittorrentie.e  14      SeIncreaseBasePriorityPrivilege         Increase scheduling priority
2624    bittorrentie.e  15      SeCreatePagefilePrivilege               Create a pagefile
2624    bittorrentie.e  16      SeCreatePermanentPrivilege              Create permanent shared objects
2624    bittorrentie.e  17      SeBackupPrivilege               Backup files and directories
2624    bittorrentie.e  18      SeRestorePrivilege              Restore files and directories
2624    bittorrentie.e  19      SeShutdownPrivilege     Present Shut down the system
2624    bittorrentie.e  20      SeDebugPrivilege                Debug programs
2624    bittorrentie.e  21      SeAuditPrivilege                Generate security audits
2624    bittorrentie.e  22      SeSystemEnvironmentPrivilege            Edit firmware environment values
2624    bittorrentie.e  23      SeChangeNotifyPrivilege Present,Enabled,Default Receive notifications of changes to files or directories
2624    bittorrentie.e  24      SeRemoteShutdownPrivilege               Force shutdown from a remote system
2624    bittorrentie.e  25      SeUndockPrivilege       Present Remove computer from docking station
2624    bittorrentie.e  26      SeSyncAgentPrivilege            Synch directory service data
2624    bittorrentie.e  27      SeEnableDelegationPrivilege             Enable user accounts to be trusted for delegation
2624    bittorrentie.e  28      SeManageVolumePrivilege         Manage the files on a volume
2624    bittorrentie.e  29      SeImpersonatePrivilege          Impersonate a client after authentication
2624    bittorrentie.e  30      SeCreateGlobalPrivilege         Create global objects
2624    bittorrentie.e  31      SeTrustedCredManAccessPrivilege         Access Credential Manager as a trusted caller
2624    bittorrentie.e  32      SeRelabelPrivilege              Modify the mandatory integrity level of an object
2624    bittorrentie.e  33      SeIncreaseWorkingSetPrivilege   Present Allocate more memory for user applications
2624    bittorrentie.e  34      SeTimeZonePrivilege     Present Adjust the time zone of the computer's internal clock
2624    bittorrentie.e  35      SeCreateSymbolicLinkPrivilege           Required to create a symbolic link
2624    bittorrentie.e  36      SeDelegateSessionUserImpersonatePrivilege               Obtain an impersonation token for another user in the same session.
708     LunarMS.exe     2       SeCreateTokenPrivilege          Create a token object
708     LunarMS.exe     3       SeAssignPrimaryTokenPrivilege           Replace a process-level token
708     LunarMS.exe     4       SeLockMemoryPrivilege           Lock pages in memory
708     LunarMS.exe     5       SeIncreaseQuotaPrivilege        Present Increase quotas
708     LunarMS.exe     6       SeMachineAccountPrivilege               Add workstations to the domain
708     LunarMS.exe     7       SeTcbPrivilege          Act as part of the operating system
708     LunarMS.exe     8       SeSecurityPrivilege     Present Manage auditing and security log
708     LunarMS.exe     9       SeTakeOwnershipPrivilege        Present Take ownership of files/objects
708     LunarMS.exe     10      SeLoadDriverPrivilege   Present Load and unload device drivers
708     LunarMS.exe     11      SeSystemProfilePrivilege        Present Profile system performance
708     LunarMS.exe     12      SeSystemtimePrivilege   Present Change the system time
708     LunarMS.exe     13      SeProfileSingleProcessPrivilege Present Profile a single process
708     LunarMS.exe     14      SeIncreaseBasePriorityPrivilege Present Increase scheduling priority
708     LunarMS.exe     15      SeCreatePagefilePrivilege       Present Create a pagefile
708     LunarMS.exe     16      SeCreatePermanentPrivilege              Create permanent shared objects
708     LunarMS.exe     17      SeBackupPrivilege       Present Backup files and directories
708     LunarMS.exe     18      SeRestorePrivilege      Present Restore files and directories
708     LunarMS.exe     19      SeShutdownPrivilege     Present Shut down the system
708     LunarMS.exe     20      SeDebugPrivilege        Present,Enabled Debug programs
708     LunarMS.exe     21      SeAuditPrivilege                Generate security audits
708     LunarMS.exe     22      SeSystemEnvironmentPrivilege    Present Edit firmware environment values
708     LunarMS.exe     23      SeChangeNotifyPrivilege Present,Enabled,Default Receive notifications of changes to files or directories
708     LunarMS.exe     24      SeRemoteShutdownPrivilege       Present Force shutdown from a remote system
708     LunarMS.exe     25      SeUndockPrivilege       Present Remove computer from docking station
708     LunarMS.exe     26      SeSyncAgentPrivilege            Synch directory service data
708     LunarMS.exe     27      SeEnableDelegationPrivilege             Enable user accounts to be trusted for delegation
708     LunarMS.exe     28      SeManageVolumePrivilege Present Manage the files on a volume
708     LunarMS.exe     29      SeImpersonatePrivilege  Present,Enabled,Default Impersonate a client after authentication
708     LunarMS.exe     30      SeCreateGlobalPrivilege Present,Enabled,Default Create global objects
708     LunarMS.exe     31      SeTrustedCredManAccessPrivilege         Access Credential Manager as a trusted caller
708     LunarMS.exe     32      SeRelabelPrivilege              Modify the mandatory integrity level of an object
708     LunarMS.exe     33      SeIncreaseWorkingSetPrivilege   Present Allocate more memory for user applications
708     LunarMS.exe     34      SeTimeZonePrivilege     Present Adjust the time zone of the computer's internal clock
708     LunarMS.exe     35      SeCreateSymbolicLinkPrivilege   Present Required to create a symbolic link
708     LunarMS.exe     36      SeDelegateSessionUserImpersonatePrivilege               Obtain an impersonation token for another user in the same session.
724     PresentationFo  2       SeCreateTokenPrivilege          Create a token object
724     PresentationFo  3       SeAssignPrimaryTokenPrivilege   Present Replace a process-level token
724     PresentationFo  4       SeLockMemoryPrivilege           Lock pages in memory
724     PresentationFo  5       SeIncreaseQuotaPrivilege        Present Increase quotas
724     PresentationFo  6       SeMachineAccountPrivilege               Add workstations to the domain
724     PresentationFo  7       SeTcbPrivilege          Act as part of the operating system
724     PresentationFo  8       SeSecurityPrivilege             Manage auditing and security log
724     PresentationFo  9       SeTakeOwnershipPrivilege                Take ownership of files/objects
724     PresentationFo  10      SeLoadDriverPrivilege           Load and unload device drivers
724     PresentationFo  11      SeSystemProfilePrivilege                Profile system performance
724     PresentationFo  12      SeSystemtimePrivilege   Present Change the system time
724     PresentationFo  13      SeProfileSingleProcessPrivilege         Profile a single process
724     PresentationFo  14      SeIncreaseBasePriorityPrivilege         Increase scheduling priority
724     PresentationFo  15      SeCreatePagefilePrivilege               Create a pagefile
724     PresentationFo  16      SeCreatePermanentPrivilege              Create permanent shared objects
724     PresentationFo  17      SeBackupPrivilege               Backup files and directories
724     PresentationFo  18      SeRestorePrivilege              Restore files and directories
724     PresentationFo  19      SeShutdownPrivilege     Present Shut down the system
724     PresentationFo  20      SeDebugPrivilege                Debug programs
724     PresentationFo  21      SeAuditPrivilege        Present Generate security audits
724     PresentationFo  22      SeSystemEnvironmentPrivilege            Edit firmware environment values
724     PresentationFo  23      SeChangeNotifyPrivilege Present,Enabled,Default Receive notifications of changes to files or directories
724     PresentationFo  24      SeRemoteShutdownPrivilege               Force shutdown from a remote system
724     PresentationFo  25      SeUndockPrivilege       Present Remove computer from docking station
724     PresentationFo  26      SeSyncAgentPrivilege            Synch directory service data
724     PresentationFo  27      SeEnableDelegationPrivilege             Enable user accounts to be trusted for delegation
724     PresentationFo  28      SeManageVolumePrivilege         Manage the files on a volume
724     PresentationFo  29      SeImpersonatePrivilege  Present,Enabled,Default Impersonate a client after authentication
724     PresentationFo  30      SeCreateGlobalPrivilege Present,Enabled,Default Create global objects
724     PresentationFo  31      SeTrustedCredManAccessPrivilege         Access Credential Manager as a trusted caller
724     PresentationFo  32      SeRelabelPrivilege              Modify the mandatory integrity level of an object
724     PresentationFo  33      SeIncreaseWorkingSetPrivilege   Present Allocate more memory for user applications
724     PresentationFo  34      SeTimeZonePrivilege     Present Adjust the time zone of the computer's internal clock
724     PresentationFo  35      SeCreateSymbolicLinkPrivilege           Required to create a symbolic link
724     PresentationFo  36      SeDelegateSessionUserImpersonatePrivilege               Obtain an impersonation token for another user in the same session.
412     mscorsvw.exe    2       SeCreateTokenPrivilege          Create a token object
412     mscorsvw.exe    3       SeAssignPrimaryTokenPrivilege   Present Replace a process-level token
412     mscorsvw.exe    4       SeLockMemoryPrivilege   Default Lock pages in memory
412     mscorsvw.exe    5       SeIncreaseQuotaPrivilege        Present Increase quotas
412     mscorsvw.exe    6       SeMachineAccountPrivilege               Add workstations to the domain
412     mscorsvw.exe    7       SeTcbPrivilege  Present,Enabled,Default Act as part of the operating system
412     mscorsvw.exe    8       SeSecurityPrivilege             Manage auditing and security log
412     mscorsvw.exe    9       SeTakeOwnershipPrivilege                Take ownership of files/objects
412     mscorsvw.exe    10      SeLoadDriverPrivilege           Load and unload device drivers
412     mscorsvw.exe    11      SeSystemProfilePrivilege        Default Profile system performance
412     mscorsvw.exe    12      SeSystemtimePrivilege           Change the system time
412     mscorsvw.exe    13      SeProfileSingleProcessPrivilege Default Profile a single process
412     mscorsvw.exe    14      SeIncreaseBasePriorityPrivilege Present,Enabled,Default Increase scheduling priority
412     mscorsvw.exe    15      SeCreatePagefilePrivilege       Default Create a pagefile
412     mscorsvw.exe    16      SeCreatePermanentPrivilege      Default Create permanent shared objects
412     mscorsvw.exe    17      SeBackupPrivilege               Backup files and directories
412     mscorsvw.exe    18      SeRestorePrivilege              Restore files and directories
412     mscorsvw.exe    19      SeShutdownPrivilege     Present Shut down the system
412     mscorsvw.exe    20      SeDebugPrivilege        Default Debug programs
412     mscorsvw.exe    21      SeAuditPrivilege        Default Generate security audits
412     mscorsvw.exe    22      SeSystemEnvironmentPrivilege            Edit firmware environment values
412     mscorsvw.exe    23      SeChangeNotifyPrivilege Present,Enabled,Default Receive notifications of changes to files or directories
412     mscorsvw.exe    24      SeRemoteShutdownPrivilege               Force shutdown from a remote system
412     mscorsvw.exe    25      SeUndockPrivilege               Remove computer from docking station
412     mscorsvw.exe    26      SeSyncAgentPrivilege            Synch directory service data
412     mscorsvw.exe    27      SeEnableDelegationPrivilege             Enable user accounts to be trusted for delegation
412     mscorsvw.exe    28      SeManageVolumePrivilege         Manage the files on a volume
412     mscorsvw.exe    29      SeImpersonatePrivilege  Default Impersonate a client after authentication
412     mscorsvw.exe    30      SeCreateGlobalPrivilege Present,Enabled,Default Create global objects
412     mscorsvw.exe    31      SeTrustedCredManAccessPrivilege         Access Credential Manager as a trusted caller
412     mscorsvw.exe    32      SeRelabelPrivilege              Modify the mandatory integrity level of an object
412     mscorsvw.exe    33      SeIncreaseWorkingSetPrivilege   Default Allocate more memory for user applications
412     mscorsvw.exe    34      SeTimeZonePrivilege     Default Adjust the time zone of the computer's internal clock
412     mscorsvw.exe    35      SeCreateSymbolicLinkPrivilege   Default Required to create a symbolic link
412     mscorsvw.exe    36      SeDelegateSessionUserImpersonatePrivilege               Obtain an impersonation token for another user in the same session.
164     svchost.exe     2       SeCreateTokenPrivilege          Create a token object
164     svchost.exe     3       SeAssignPrimaryTokenPrivilege           Replace a process-level token
164     svchost.exe     4       SeLockMemoryPrivilege           Lock pages in memory
164     svchost.exe     5       SeIncreaseQuotaPrivilege                Increase quotas
164     svchost.exe     6       SeMachineAccountPrivilege               Add workstations to the domain
164     svchost.exe     7       SeTcbPrivilege          Act as part of the operating system
164     svchost.exe     8       SeSecurityPrivilege             Manage auditing and security log
164     svchost.exe     9       SeTakeOwnershipPrivilege                Take ownership of files/objects
164     svchost.exe     10      SeLoadDriverPrivilege           Load and unload device drivers
164     svchost.exe     11      SeSystemProfilePrivilege                Profile system performance
164     svchost.exe     12      SeSystemtimePrivilege           Change the system time
164     svchost.exe     13      SeProfileSingleProcessPrivilege         Profile a single process
164     svchost.exe     14      SeIncreaseBasePriorityPrivilege         Increase scheduling priority
164     svchost.exe     15      SeCreatePagefilePrivilege               Create a pagefile
164     svchost.exe     16      SeCreatePermanentPrivilege              Create permanent shared objects
164     svchost.exe     17      SeBackupPrivilege               Backup files and directories
164     svchost.exe     18      SeRestorePrivilege              Restore files and directories
164     svchost.exe     19      SeShutdownPrivilege             Shut down the system
164     svchost.exe     20      SeDebugPrivilege                Debug programs
164     svchost.exe     21      SeAuditPrivilege        Present Generate security audits
164     svchost.exe     22      SeSystemEnvironmentPrivilege            Edit firmware environment values
164     svchost.exe     23      SeChangeNotifyPrivilege Present,Enabled,Default Receive notifications of changes to files or directories
164     svchost.exe     24      SeRemoteShutdownPrivilege               Force shutdown from a remote system
164     svchost.exe     25      SeUndockPrivilege               Remove computer from docking station
164     svchost.exe     26      SeSyncAgentPrivilege            Synch directory service data
164     svchost.exe     27      SeEnableDelegationPrivilege             Enable user accounts to be trusted for delegation
164     svchost.exe     28      SeManageVolumePrivilege         Manage the files on a volume
164     svchost.exe     29      SeImpersonatePrivilege  Default Impersonate a client after authentication
164     svchost.exe     30      SeCreateGlobalPrivilege Present,Enabled,Default Create global objects
164     svchost.exe     31      SeTrustedCredManAccessPrivilege         Access Credential Manager as a trusted caller
164     svchost.exe     32      SeRelabelPrivilege              Modify the mandatory integrity level of an object
164     svchost.exe     33      SeIncreaseWorkingSetPrivilege           Allocate more memory for user applications
164     svchost.exe     34      SeTimeZonePrivilege             Adjust the time zone of the computer's internal clock
164     svchost.exe     35      SeCreateSymbolicLinkPrivilege           Required to create a symbolic link
164     svchost.exe     36      SeDelegateSessionUserImpersonatePrivilege               Obtain an impersonation token for another user in the same session.
3124    mscorsvw.exe    2       SeCreateTokenPrivilege          Create a token object
3124    mscorsvw.exe    3       SeAssignPrimaryTokenPrivilege   Present Replace a process-level token
3124    mscorsvw.exe    4       SeLockMemoryPrivilege   Default Lock pages in memory
3124    mscorsvw.exe    5       SeIncreaseQuotaPrivilege        Present Increase quotas
3124    mscorsvw.exe    6       SeMachineAccountPrivilege               Add workstations to the domain
3124    mscorsvw.exe    7       SeTcbPrivilege  Present,Enabled,Default Act as part of the operating system
3124    mscorsvw.exe    8       SeSecurityPrivilege             Manage auditing and security log
3124    mscorsvw.exe    9       SeTakeOwnershipPrivilege                Take ownership of files/objects
3124    mscorsvw.exe    10      SeLoadDriverPrivilege           Load and unload device drivers
3124    mscorsvw.exe    11      SeSystemProfilePrivilege        Default Profile system performance
3124    mscorsvw.exe    12      SeSystemtimePrivilege           Change the system time
3124    mscorsvw.exe    13      SeProfileSingleProcessPrivilege Default Profile a single process
3124    mscorsvw.exe    14      SeIncreaseBasePriorityPrivilege Present,Enabled,Default Increase scheduling priority
3124    mscorsvw.exe    15      SeCreatePagefilePrivilege       Default Create a pagefile
3124    mscorsvw.exe    16      SeCreatePermanentPrivilege      Default Create permanent shared objects
3124    mscorsvw.exe    17      SeBackupPrivilege               Backup files and directories
3124    mscorsvw.exe    18      SeRestorePrivilege              Restore files and directories
3124    mscorsvw.exe    19      SeShutdownPrivilege     Present Shut down the system
3124    mscorsvw.exe    20      SeDebugPrivilege        Default Debug programs
3124    mscorsvw.exe    21      SeAuditPrivilege        Default Generate security audits
3124    mscorsvw.exe    22      SeSystemEnvironmentPrivilege            Edit firmware environment values
3124    mscorsvw.exe    23      SeChangeNotifyPrivilege Present,Enabled,Default Receive notifications of changes to files or directories
3124    mscorsvw.exe    24      SeRemoteShutdownPrivilege               Force shutdown from a remote system
3124    mscorsvw.exe    25      SeUndockPrivilege               Remove computer from docking station
3124    mscorsvw.exe    26      SeSyncAgentPrivilege            Synch directory service data
3124    mscorsvw.exe    27      SeEnableDelegationPrivilege             Enable user accounts to be trusted for delegation
3124    mscorsvw.exe    28      SeManageVolumePrivilege         Manage the files on a volume
3124    mscorsvw.exe    29      SeImpersonatePrivilege  Default Impersonate a client after authentication
3124    mscorsvw.exe    30      SeCreateGlobalPrivilege Present,Enabled,Default Create global objects
3124    mscorsvw.exe    31      SeTrustedCredManAccessPrivilege         Access Credential Manager as a trusted caller
3124    mscorsvw.exe    32      SeRelabelPrivilege              Modify the mandatory integrity level of an object
3124    mscorsvw.exe    33      SeIncreaseWorkingSetPrivilege   Default Allocate more memory for user applications
3124    mscorsvw.exe    34      SeTimeZonePrivilege     Default Adjust the time zone of the computer's internal clock
3124    mscorsvw.exe    35      SeCreateSymbolicLinkPrivilege   Default Required to create a symbolic link
3124    mscorsvw.exe    36      SeDelegateSessionUserImpersonatePrivilege               Obtain an impersonation token for another user in the same session.
3196    svchost.exe     2       SeCreateTokenPrivilege          Create a token object
3196    svchost.exe     3       SeAssignPrimaryTokenPrivilege   Present,Enabled Replace a process-level token
3196    svchost.exe     4       SeLockMemoryPrivilege   Default Lock pages in memory
3196    svchost.exe     5       SeIncreaseQuotaPrivilege        Present,Enabled Increase quotas
3196    svchost.exe     6       SeMachineAccountPrivilege               Add workstations to the domain
3196    svchost.exe     7       SeTcbPrivilege  Default Act as part of the operating system
3196    svchost.exe     8       SeSecurityPrivilege     Present,Enabled Manage auditing and security log
3196    svchost.exe     9       SeTakeOwnershipPrivilege                Take ownership of files/objects
3196    svchost.exe     10      SeLoadDriverPrivilege           Load and unload device drivers
3196    svchost.exe     11      SeSystemProfilePrivilege        Default Profile system performance
3196    svchost.exe     12      SeSystemtimePrivilege           Change the system time
3196    svchost.exe     13      SeProfileSingleProcessPrivilege Default Profile a single process
3196    svchost.exe     14      SeIncreaseBasePriorityPrivilege Default Increase scheduling priority
3196    svchost.exe     15      SeCreatePagefilePrivilege       Default Create a pagefile
3196    svchost.exe     16      SeCreatePermanentPrivilege      Default Create permanent shared objects
3196    svchost.exe     17      SeBackupPrivilege       Present,Enabled Backup files and directories
3196    svchost.exe     18      SeRestorePrivilege      Present,Enabled Restore files and directories
3196    svchost.exe     19      SeShutdownPrivilege     Present,Enabled Shut down the system
3196    svchost.exe     20      SeDebugPrivilege        Present,Enabled,Default Debug programs
3196    svchost.exe     21      SeAuditPrivilege        Default Generate security audits
3196    svchost.exe     22      SeSystemEnvironmentPrivilege            Edit firmware environment values
3196    svchost.exe     23      SeChangeNotifyPrivilege Present,Enabled,Default Receive notifications of changes to files or directories
3196    svchost.exe     24      SeRemoteShutdownPrivilege               Force shutdown from a remote system
3196    svchost.exe     25      SeUndockPrivilege               Remove computer from docking station
3196    svchost.exe     26      SeSyncAgentPrivilege            Synch directory service data
3196    svchost.exe     27      SeEnableDelegationPrivilege             Enable user accounts to be trusted for delegation
3196    svchost.exe     28      SeManageVolumePrivilege         Manage the files on a volume
3196    svchost.exe     29      SeImpersonatePrivilege  Present,Enabled,Default Impersonate a client after authentication
3196    svchost.exe     30      SeCreateGlobalPrivilege Default Create global objects
3196    svchost.exe     31      SeTrustedCredManAccessPrivilege         Access Credential Manager as a trusted caller
3196    svchost.exe     32      SeRelabelPrivilege              Modify the mandatory integrity level of an object
3196    svchost.exe     33      SeIncreaseWorkingSetPrivilege   Default Allocate more memory for user applications
3196    svchost.exe     34      SeTimeZonePrivilege     Default Adjust the time zone of the computer's internal clock
3196    svchost.exe     35      SeCreateSymbolicLinkPrivilege   Default Required to create a symbolic link
3196    svchost.exe     36      SeDelegateSessionUserImpersonatePrivilege               Obtain an impersonation token for another user in the same session.
4076    chrome.exe      2       SeCreateTokenPrivilege          Create a token object
4076    chrome.exe      3       SeAssignPrimaryTokenPrivilege           Replace a process-level token
4076    chrome.exe      4       SeLockMemoryPrivilege           Lock pages in memory
4076    chrome.exe      5       SeIncreaseQuotaPrivilege                Increase quotas
4076    chrome.exe      6       SeMachineAccountPrivilege               Add workstations to the domain
4076    chrome.exe      7       SeTcbPrivilege          Act as part of the operating system
4076    chrome.exe      8       SeSecurityPrivilege             Manage auditing and security log
4076    chrome.exe      9       SeTakeOwnershipPrivilege                Take ownership of files/objects
4076    chrome.exe      10      SeLoadDriverPrivilege           Load and unload device drivers
4076    chrome.exe      11      SeSystemProfilePrivilege                Profile system performance
4076    chrome.exe      12      SeSystemtimePrivilege           Change the system time
4076    chrome.exe      13      SeProfileSingleProcessPrivilege         Profile a single process
4076    chrome.exe      14      SeIncreaseBasePriorityPrivilege         Increase scheduling priority
4076    chrome.exe      15      SeCreatePagefilePrivilege               Create a pagefile
4076    chrome.exe      16      SeCreatePermanentPrivilege              Create permanent shared objects
4076    chrome.exe      17      SeBackupPrivilege               Backup files and directories
4076    chrome.exe      18      SeRestorePrivilege              Restore files and directories
4076    chrome.exe      19      SeShutdownPrivilege     Present Shut down the system
4076    chrome.exe      20      SeDebugPrivilege                Debug programs
4076    chrome.exe      21      SeAuditPrivilege                Generate security audits
4076    chrome.exe      22      SeSystemEnvironmentPrivilege            Edit firmware environment values
4076    chrome.exe      23      SeChangeNotifyPrivilege Present,Enabled,Default Receive notifications of changes to files or directories
4076    chrome.exe      24      SeRemoteShutdownPrivilege               Force shutdown from a remote system
4076    chrome.exe      25      SeUndockPrivilege       Present Remove computer from docking station
4076    chrome.exe      26      SeSyncAgentPrivilege            Synch directory service data
4076    chrome.exe      27      SeEnableDelegationPrivilege             Enable user accounts to be trusted for delegation
4076    chrome.exe      28      SeManageVolumePrivilege         Manage the files on a volume
4076    chrome.exe      29      SeImpersonatePrivilege          Impersonate a client after authentication
4076    chrome.exe      30      SeCreateGlobalPrivilege         Create global objects
4076    chrome.exe      31      SeTrustedCredManAccessPrivilege         Access Credential Manager as a trusted caller
4076    chrome.exe      32      SeRelabelPrivilege              Modify the mandatory integrity level of an object
4076    chrome.exe      33      SeIncreaseWorkingSetPrivilege   Present Allocate more memory for user applications
4076    chrome.exe      34      SeTimeZonePrivilege     Present Adjust the time zone of the computer's internal clock
4076    chrome.exe      35      SeCreateSymbolicLinkPrivilege           Required to create a symbolic link
4076    chrome.exe      36      SeDelegateSessionUserImpersonatePrivilege               Obtain an impersonation token for another user in the same session.
4084    chrome.exe      2       SeCreateTokenPrivilege          Create a token object
4084    chrome.exe      3       SeAssignPrimaryTokenPrivilege           Replace a process-level token
4084    chrome.exe      4       SeLockMemoryPrivilege           Lock pages in memory
4084    chrome.exe      5       SeIncreaseQuotaPrivilege                Increase quotas
4084    chrome.exe      6       SeMachineAccountPrivilege               Add workstations to the domain
4084    chrome.exe      7       SeTcbPrivilege          Act as part of the operating system
4084    chrome.exe      8       SeSecurityPrivilege             Manage auditing and security log
4084    chrome.exe      9       SeTakeOwnershipPrivilege                Take ownership of files/objects
4084    chrome.exe      10      SeLoadDriverPrivilege           Load and unload device drivers
4084    chrome.exe      11      SeSystemProfilePrivilege                Profile system performance
4084    chrome.exe      12      SeSystemtimePrivilege           Change the system time
4084    chrome.exe      13      SeProfileSingleProcessPrivilege         Profile a single process
4084    chrome.exe      14      SeIncreaseBasePriorityPrivilege         Increase scheduling priority
4084    chrome.exe      15      SeCreatePagefilePrivilege               Create a pagefile
4084    chrome.exe      16      SeCreatePermanentPrivilege              Create permanent shared objects
4084    chrome.exe      17      SeBackupPrivilege               Backup files and directories
4084    chrome.exe      18      SeRestorePrivilege              Restore files and directories
4084    chrome.exe      19      SeShutdownPrivilege     Present Shut down the system
4084    chrome.exe      20      SeDebugPrivilege                Debug programs
4084    chrome.exe      21      SeAuditPrivilege                Generate security audits
4084    chrome.exe      22      SeSystemEnvironmentPrivilege            Edit firmware environment values
4084    chrome.exe      23      SeChangeNotifyPrivilege Present,Enabled,Default Receive notifications of changes to files or directories
4084    chrome.exe      24      SeRemoteShutdownPrivilege               Force shutdown from a remote system
4084    chrome.exe      25      SeUndockPrivilege       Present Remove computer from docking station
4084    chrome.exe      26      SeSyncAgentPrivilege            Synch directory service data
4084    chrome.exe      27      SeEnableDelegationPrivilege             Enable user accounts to be trusted for delegation
4084    chrome.exe      28      SeManageVolumePrivilege         Manage the files on a volume
4084    chrome.exe      29      SeImpersonatePrivilege          Impersonate a client after authentication
4084    chrome.exe      30      SeCreateGlobalPrivilege         Create global objects
4084    chrome.exe      31      SeTrustedCredManAccessPrivilege         Access Credential Manager as a trusted caller
4084    chrome.exe      32      SeRelabelPrivilege              Modify the mandatory integrity level of an object
4084    chrome.exe      33      SeIncreaseWorkingSetPrivilege   Present Allocate more memory for user applications
4084    chrome.exe      34      SeTimeZonePrivilege     Present Adjust the time zone of the computer's internal clock
4084    chrome.exe      35      SeCreateSymbolicLinkPrivilege           Required to create a symbolic link
4084    chrome.exe      36      SeDelegateSessionUserImpersonatePrivilege               Obtain an impersonation token for another user in the same session.
576     chrome.exe      2       SeCreateTokenPrivilege          Create a token object
576     chrome.exe      3       SeAssignPrimaryTokenPrivilege           Replace a process-level token
576     chrome.exe      4       SeLockMemoryPrivilege           Lock pages in memory
576     chrome.exe      5       SeIncreaseQuotaPrivilege                Increase quotas
576     chrome.exe      6       SeMachineAccountPrivilege               Add workstations to the domain
576     chrome.exe      7       SeTcbPrivilege          Act as part of the operating system
576     chrome.exe      8       SeSecurityPrivilege             Manage auditing and security log
576     chrome.exe      9       SeTakeOwnershipPrivilege                Take ownership of files/objects
576     chrome.exe      10      SeLoadDriverPrivilege           Load and unload device drivers
576     chrome.exe      11      SeSystemProfilePrivilege                Profile system performance
576     chrome.exe      12      SeSystemtimePrivilege           Change the system time
576     chrome.exe      13      SeProfileSingleProcessPrivilege         Profile a single process
576     chrome.exe      14      SeIncreaseBasePriorityPrivilege         Increase scheduling priority
576     chrome.exe      15      SeCreatePagefilePrivilege               Create a pagefile
576     chrome.exe      16      SeCreatePermanentPrivilege              Create permanent shared objects
576     chrome.exe      17      SeBackupPrivilege               Backup files and directories
576     chrome.exe      18      SeRestorePrivilege              Restore files and directories
576     chrome.exe      19      SeShutdownPrivilege     Present Shut down the system
576     chrome.exe      20      SeDebugPrivilege                Debug programs
576     chrome.exe      21      SeAuditPrivilege                Generate security audits
576     chrome.exe      22      SeSystemEnvironmentPrivilege            Edit firmware environment values
576     chrome.exe      23      SeChangeNotifyPrivilege Present,Enabled,Default Receive notifications of changes to files or directories
576     chrome.exe      24      SeRemoteShutdownPrivilege               Force shutdown from a remote system
576     chrome.exe      25      SeUndockPrivilege       Present Remove computer from docking station
576     chrome.exe      26      SeSyncAgentPrivilege            Synch directory service data
576     chrome.exe      27      SeEnableDelegationPrivilege             Enable user accounts to be trusted for delegation
576     chrome.exe      28      SeManageVolumePrivilege         Manage the files on a volume
576     chrome.exe      29      SeImpersonatePrivilege          Impersonate a client after authentication
576     chrome.exe      30      SeCreateGlobalPrivilege         Create global objects
576     chrome.exe      31      SeTrustedCredManAccessPrivilege         Access Credential Manager as a trusted caller
576     chrome.exe      32      SeRelabelPrivilege              Modify the mandatory integrity level of an object
576     chrome.exe      33      SeIncreaseWorkingSetPrivilege   Present Allocate more memory for user applications
576     chrome.exe      34      SeTimeZonePrivilege     Present Adjust the time zone of the computer's internal clock
576     chrome.exe      35      SeCreateSymbolicLinkPrivilege           Required to create a symbolic link
576     chrome.exe      36      SeDelegateSessionUserImpersonatePrivilege               Obtain an impersonation token for another user in the same session.
1808    chrome.exe      2       SeCreateTokenPrivilege          Create a token object
1808    chrome.exe      3       SeAssignPrimaryTokenPrivilege           Replace a process-level token
1808    chrome.exe      4       SeLockMemoryPrivilege           Lock pages in memory
1808    chrome.exe      5       SeIncreaseQuotaPrivilege                Increase quotas
1808    chrome.exe      6       SeMachineAccountPrivilege               Add workstations to the domain
1808    chrome.exe      7       SeTcbPrivilege          Act as part of the operating system
1808    chrome.exe      8       SeSecurityPrivilege             Manage auditing and security log
1808    chrome.exe      9       SeTakeOwnershipPrivilege                Take ownership of files/objects
1808    chrome.exe      10      SeLoadDriverPrivilege           Load and unload device drivers
1808    chrome.exe      11      SeSystemProfilePrivilege                Profile system performance
1808    chrome.exe      12      SeSystemtimePrivilege           Change the system time
1808    chrome.exe      13      SeProfileSingleProcessPrivilege         Profile a single process
1808    chrome.exe      14      SeIncreaseBasePriorityPrivilege         Increase scheduling priority
1808    chrome.exe      15      SeCreatePagefilePrivilege               Create a pagefile
1808    chrome.exe      16      SeCreatePermanentPrivilege              Create permanent shared objects
1808    chrome.exe      17      SeBackupPrivilege               Backup files and directories
1808    chrome.exe      18      SeRestorePrivilege              Restore files and directories
1808    chrome.exe      19      SeShutdownPrivilege             Shut down the system
1808    chrome.exe      20      SeDebugPrivilege                Debug programs
1808    chrome.exe      21      SeAuditPrivilege                Generate security audits
1808    chrome.exe      22      SeSystemEnvironmentPrivilege            Edit firmware environment values
1808    chrome.exe      23      SeChangeNotifyPrivilege Present,Enabled,Default Receive notifications of changes to files or directories
1808    chrome.exe      24      SeRemoteShutdownPrivilege               Force shutdown from a remote system
1808    chrome.exe      25      SeUndockPrivilege               Remove computer from docking station
1808    chrome.exe      26      SeSyncAgentPrivilege            Synch directory service data
1808    chrome.exe      27      SeEnableDelegationPrivilege             Enable user accounts to be trusted for delegation
1808    chrome.exe      28      SeManageVolumePrivilege         Manage the files on a volume
1808    chrome.exe      29      SeImpersonatePrivilege          Impersonate a client after authentication
1808    chrome.exe      30      SeCreateGlobalPrivilege         Create global objects
1808    chrome.exe      31      SeTrustedCredManAccessPrivilege         Access Credential Manager as a trusted caller
1808    chrome.exe      32      SeRelabelPrivilege              Modify the mandatory integrity level of an object
1808    chrome.exe      33      SeIncreaseWorkingSetPrivilege           Allocate more memory for user applications
1808    chrome.exe      34      SeTimeZonePrivilege             Adjust the time zone of the computer's internal clock
1808    chrome.exe      35      SeCreateSymbolicLinkPrivilege           Required to create a symbolic link
1808    chrome.exe      36      SeDelegateSessionUserImpersonatePrivilege               Obtain an impersonation token for another user in the same session.
3924    chrome.exe      2       SeCreateTokenPrivilege          Create a token object
3924    chrome.exe      3       SeAssignPrimaryTokenPrivilege           Replace a process-level token
3924    chrome.exe      4       SeLockMemoryPrivilege           Lock pages in memory
3924    chrome.exe      5       SeIncreaseQuotaPrivilege                Increase quotas
3924    chrome.exe      6       SeMachineAccountPrivilege               Add workstations to the domain
3924    chrome.exe      7       SeTcbPrivilege          Act as part of the operating system
3924    chrome.exe      8       SeSecurityPrivilege             Manage auditing and security log
3924    chrome.exe      9       SeTakeOwnershipPrivilege                Take ownership of files/objects
3924    chrome.exe      10      SeLoadDriverPrivilege           Load and unload device drivers
3924    chrome.exe      11      SeSystemProfilePrivilege                Profile system performance
3924    chrome.exe      12      SeSystemtimePrivilege           Change the system time
3924    chrome.exe      13      SeProfileSingleProcessPrivilege         Profile a single process
3924    chrome.exe      14      SeIncreaseBasePriorityPrivilege         Increase scheduling priority
3924    chrome.exe      15      SeCreatePagefilePrivilege               Create a pagefile
3924    chrome.exe      16      SeCreatePermanentPrivilege              Create permanent shared objects
3924    chrome.exe      17      SeBackupPrivilege               Backup files and directories
3924    chrome.exe      18      SeRestorePrivilege              Restore files and directories
3924    chrome.exe      19      SeShutdownPrivilege             Shut down the system
3924    chrome.exe      20      SeDebugPrivilege                Debug programs
3924    chrome.exe      21      SeAuditPrivilege                Generate security audits
3924    chrome.exe      22      SeSystemEnvironmentPrivilege            Edit firmware environment values
3924    chrome.exe      23      SeChangeNotifyPrivilege Default Receive notifications of changes to files or directories
3924    chrome.exe      24      SeRemoteShutdownPrivilege               Force shutdown from a remote system
3924    chrome.exe      25      SeUndockPrivilege               Remove computer from docking station
3924    chrome.exe      26      SeSyncAgentPrivilege            Synch directory service data
3924    chrome.exe      27      SeEnableDelegationPrivilege             Enable user accounts to be trusted for delegation
3924    chrome.exe      28      SeManageVolumePrivilege         Manage the files on a volume
3924    chrome.exe      29      SeImpersonatePrivilege          Impersonate a client after authentication
3924    chrome.exe      30      SeCreateGlobalPrivilege         Create global objects
3924    chrome.exe      31      SeTrustedCredManAccessPrivilege         Access Credential Manager as a trusted caller
3924    chrome.exe      32      SeRelabelPrivilege              Modify the mandatory integrity level of an object
3924    chrome.exe      33      SeIncreaseWorkingSetPrivilege           Allocate more memory for user applications
3924    chrome.exe      34      SeTimeZonePrivilege             Adjust the time zone of the computer's internal clock
3924    chrome.exe      35      SeCreateSymbolicLinkPrivilege           Required to create a symbolic link
3924    chrome.exe      36      SeDelegateSessionUserImpersonatePrivilege               Obtain an impersonation token for another user in the same session.
2748    chrome.exe      2       SeCreateTokenPrivilege          Create a token object
2748    chrome.exe      3       SeAssignPrimaryTokenPrivilege           Replace a process-level token
2748    chrome.exe      4       SeLockMemoryPrivilege           Lock pages in memory
2748    chrome.exe      5       SeIncreaseQuotaPrivilege                Increase quotas
2748    chrome.exe      6       SeMachineAccountPrivilege               Add workstations to the domain
2748    chrome.exe      7       SeTcbPrivilege          Act as part of the operating system
2748    chrome.exe      8       SeSecurityPrivilege             Manage auditing and security log
2748    chrome.exe      9       SeTakeOwnershipPrivilege                Take ownership of files/objects
2748    chrome.exe      10      SeLoadDriverPrivilege           Load and unload device drivers
2748    chrome.exe      11      SeSystemProfilePrivilege                Profile system performance
2748    chrome.exe      12      SeSystemtimePrivilege           Change the system time
2748    chrome.exe      13      SeProfileSingleProcessPrivilege         Profile a single process
2748    chrome.exe      14      SeIncreaseBasePriorityPrivilege         Increase scheduling priority
2748    chrome.exe      15      SeCreatePagefilePrivilege               Create a pagefile
2748    chrome.exe      16      SeCreatePermanentPrivilege              Create permanent shared objects
2748    chrome.exe      17      SeBackupPrivilege               Backup files and directories
2748    chrome.exe      18      SeRestorePrivilege              Restore files and directories
2748    chrome.exe      19      SeShutdownPrivilege             Shut down the system
2748    chrome.exe      20      SeDebugPrivilege                Debug programs
2748    chrome.exe      21      SeAuditPrivilege                Generate security audits
2748    chrome.exe      22      SeSystemEnvironmentPrivilege            Edit firmware environment values
2748    chrome.exe      23      SeChangeNotifyPrivilege Default Receive notifications of changes to files or directories
2748    chrome.exe      24      SeRemoteShutdownPrivilege               Force shutdown from a remote system
2748    chrome.exe      25      SeUndockPrivilege               Remove computer from docking station
2748    chrome.exe      26      SeSyncAgentPrivilege            Synch directory service data
2748    chrome.exe      27      SeEnableDelegationPrivilege             Enable user accounts to be trusted for delegation
2748    chrome.exe      28      SeManageVolumePrivilege         Manage the files on a volume
2748    chrome.exe      29      SeImpersonatePrivilege          Impersonate a client after authentication
2748    chrome.exe      30      SeCreateGlobalPrivilege         Create global objects
2748    chrome.exe      31      SeTrustedCredManAccessPrivilege         Access Credential Manager as a trusted caller
2748    chrome.exe      32      SeRelabelPrivilege              Modify the mandatory integrity level of an object
2748    chrome.exe      33      SeIncreaseWorkingSetPrivilege           Allocate more memory for user applications
2748    chrome.exe      34      SeTimeZonePrivilege             Adjust the time zone of the computer's internal clock
2748    chrome.exe      35      SeCreateSymbolicLinkPrivilege           Required to create a symbolic link
2748    chrome.exe      36      SeDelegateSessionUserImpersonatePrivilege               Obtain an impersonation token for another user in the same session.
3820    Rick And Morty  2       SeCreateTokenPrivilege          Create a token object
3820    Rick And Morty  3       SeAssignPrimaryTokenPrivilege           Replace a process-level token
3820    Rick And Morty  4       SeLockMemoryPrivilege           Lock pages in memory
3820    Rick And Morty  5       SeIncreaseQuotaPrivilege                Increase quotas
3820    Rick And Morty  6       SeMachineAccountPrivilege               Add workstations to the domain
3820    Rick And Morty  7       SeTcbPrivilege          Act as part of the operating system
3820    Rick And Morty  8       SeSecurityPrivilege             Manage auditing and security log
3820    Rick And Morty  9       SeTakeOwnershipPrivilege                Take ownership of files/objects
3820    Rick And Morty  10      SeLoadDriverPrivilege           Load and unload device drivers
3820    Rick And Morty  11      SeSystemProfilePrivilege                Profile system performance
3820    Rick And Morty  12      SeSystemtimePrivilege           Change the system time
3820    Rick And Morty  13      SeProfileSingleProcessPrivilege         Profile a single process
3820    Rick And Morty  14      SeIncreaseBasePriorityPrivilege         Increase scheduling priority
3820    Rick And Morty  15      SeCreatePagefilePrivilege               Create a pagefile
3820    Rick And Morty  16      SeCreatePermanentPrivilege              Create permanent shared objects
3820    Rick And Morty  17      SeBackupPrivilege               Backup files and directories
3820    Rick And Morty  18      SeRestorePrivilege              Restore files and directories
3820    Rick And Morty  19      SeShutdownPrivilege     Present Shut down the system
3820    Rick And Morty  20      SeDebugPrivilege                Debug programs
3820    Rick And Morty  21      SeAuditPrivilege                Generate security audits
3820    Rick And Morty  22      SeSystemEnvironmentPrivilege            Edit firmware environment values
3820    Rick And Morty  23      SeChangeNotifyPrivilege Present,Enabled,Default Receive notifications of changes to files or directories
3820    Rick And Morty  24      SeRemoteShutdownPrivilege               Force shutdown from a remote system
3820    Rick And Morty  25      SeUndockPrivilege       Present Remove computer from docking station
3820    Rick And Morty  26      SeSyncAgentPrivilege            Synch directory service data
3820    Rick And Morty  27      SeEnableDelegationPrivilege             Enable user accounts to be trusted for delegation
3820    Rick And Morty  28      SeManageVolumePrivilege         Manage the files on a volume
3820    Rick And Morty  29      SeImpersonatePrivilege          Impersonate a client after authentication
3820    Rick And Morty  30      SeCreateGlobalPrivilege         Create global objects
3820    Rick And Morty  31      SeTrustedCredManAccessPrivilege         Access Credential Manager as a trusted caller
3820    Rick And Morty  32      SeRelabelPrivilege              Modify the mandatory integrity level of an object
3820    Rick And Morty  33      SeIncreaseWorkingSetPrivilege   Present Allocate more memory for user applications
3820    Rick And Morty  34      SeTimeZonePrivilege     Present Adjust the time zone of the computer's internal clock
3820    Rick And Morty  35      SeCreateSymbolicLinkPrivilege           Required to create a symbolic link
3820    Rick And Morty  36      SeDelegateSessionUserImpersonatePrivilege               Obtain an impersonation token for another user in the same session.
3720    vmware-tray.ex  2       SeCreateTokenPrivilege          Create a token object
3720    vmware-tray.ex  3       SeAssignPrimaryTokenPrivilege           Replace a process-level token
3720    vmware-tray.ex  4       SeLockMemoryPrivilege           Lock pages in memory
3720    vmware-tray.ex  5       SeIncreaseQuotaPrivilege        Present Increase quotas
3720    vmware-tray.ex  6       SeMachineAccountPrivilege               Add workstations to the domain
3720    vmware-tray.ex  7       SeTcbPrivilege          Act as part of the operating system
3720    vmware-tray.ex  8       SeSecurityPrivilege     Present Manage auditing and security log
3720    vmware-tray.ex  9       SeTakeOwnershipPrivilege        Present Take ownership of files/objects
3720    vmware-tray.ex  10      SeLoadDriverPrivilege   Present Load and unload device drivers
3720    vmware-tray.ex  11      SeSystemProfilePrivilege        Present Profile system performance
3720    vmware-tray.ex  12      SeSystemtimePrivilege   Present Change the system time
3720    vmware-tray.ex  13      SeProfileSingleProcessPrivilege Present Profile a single process
3720    vmware-tray.ex  14      SeIncreaseBasePriorityPrivilege Present Increase scheduling priority
3720    vmware-tray.ex  15      SeCreatePagefilePrivilege       Present Create a pagefile
3720    vmware-tray.ex  16      SeCreatePermanentPrivilege              Create permanent shared objects
3720    vmware-tray.ex  17      SeBackupPrivilege       Present Backup files and directories
3720    vmware-tray.ex  18      SeRestorePrivilege      Present Restore files and directories
3720    vmware-tray.ex  19      SeShutdownPrivilege     Present Shut down the system
3720    vmware-tray.ex  20      SeDebugPrivilege        Present Debug programs
3720    vmware-tray.ex  21      SeAuditPrivilege                Generate security audits
3720    vmware-tray.ex  22      SeSystemEnvironmentPrivilege    Present Edit firmware environment values
3720    vmware-tray.ex  23      SeChangeNotifyPrivilege Present,Enabled,Default Receive notifications of changes to files or directories
3720    vmware-tray.ex  24      SeRemoteShutdownPrivilege       Present Force shutdown from a remote system
3720    vmware-tray.ex  25      SeUndockPrivilege       Present Remove computer from docking station
3720    vmware-tray.ex  26      SeSyncAgentPrivilege            Synch directory service data
3720    vmware-tray.ex  27      SeEnableDelegationPrivilege             Enable user accounts to be trusted for delegation
3720    vmware-tray.ex  28      SeManageVolumePrivilege Present Manage the files on a volume
3720    vmware-tray.ex  29      SeImpersonatePrivilege  Present,Enabled,Default Impersonate a client after authentication
3720    vmware-tray.ex  30      SeCreateGlobalPrivilege Present,Enabled,Default Create global objects
3720    vmware-tray.ex  31      SeTrustedCredManAccessPrivilege         Access Credential Manager as a trusted caller
3720    vmware-tray.ex  32      SeRelabelPrivilege              Modify the mandatory integrity level of an object
3720    vmware-tray.ex  33      SeIncreaseWorkingSetPrivilege   Present Allocate more memory for user applications
3720    vmware-tray.ex  34      SeTimeZonePrivilege     Present Adjust the time zone of the computer's internal clock
3720    vmware-tray.ex  35      SeCreateSymbolicLinkPrivilege   Present Required to create a symbolic link
3720    vmware-tray.ex  36      SeDelegateSessionUserImpersonatePrivilege               Obtain an impersonation token for another user in the same session.
3880    WebCompanionIn  2       SeCreateTokenPrivilege          Create a token object
3880    WebCompanionIn  3       SeAssignPrimaryTokenPrivilege   Present Replace a process-level token
3880    WebCompanionIn  4       SeLockMemoryPrivilege   Present,Enabled,Default Lock pages in memory
3880    WebCompanionIn  5       SeIncreaseQuotaPrivilege        Present Increase quotas
3880    WebCompanionIn  6       SeMachineAccountPrivilege               Add workstations to the domain
3880    WebCompanionIn  7       SeTcbPrivilege  Present,Enabled,Default Act as part of the operating system
3880    WebCompanionIn  8       SeSecurityPrivilege     Present Manage auditing and security log
3880    WebCompanionIn  9       SeTakeOwnershipPrivilege        Present Take ownership of files/objects
3880    WebCompanionIn  10      SeLoadDriverPrivilege   Present Load and unload device drivers
3880    WebCompanionIn  11      SeSystemProfilePrivilege        Present,Enabled,Default Profile system performance
3880    WebCompanionIn  12      SeSystemtimePrivilege   Present Change the system time
3880    WebCompanionIn  13      SeProfileSingleProcessPrivilege Present,Enabled,Default Profile a single process
3880    WebCompanionIn  14      SeIncreaseBasePriorityPrivilege Present,Enabled,Default Increase scheduling priority
3880    WebCompanionIn  15      SeCreatePagefilePrivilege       Present,Enabled,Default Create a pagefile
3880    WebCompanionIn  16      SeCreatePermanentPrivilege      Present,Enabled,Default Create permanent shared objects
3880    WebCompanionIn  17      SeBackupPrivilege       Present Backup files and directories
3880    WebCompanionIn  18      SeRestorePrivilege      Present Restore files and directories
3880    WebCompanionIn  19      SeShutdownPrivilege     Present Shut down the system
3880    WebCompanionIn  20      SeDebugPrivilege        Present,Enabled,Default Debug programs
3880    WebCompanionIn  21      SeAuditPrivilege        Present,Enabled,Default Generate security audits
3880    WebCompanionIn  22      SeSystemEnvironmentPrivilege    Present Edit firmware environment values
3880    WebCompanionIn  23      SeChangeNotifyPrivilege Present,Enabled,Default Receive notifications of changes to files or directories
3880    WebCompanionIn  24      SeRemoteShutdownPrivilege               Force shutdown from a remote system
3880    WebCompanionIn  25      SeUndockPrivilege       Present Remove computer from docking station
3880    WebCompanionIn  26      SeSyncAgentPrivilege            Synch directory service data
3880    WebCompanionIn  27      SeEnableDelegationPrivilege             Enable user accounts to be trusted for delegation
3880    WebCompanionIn  28      SeManageVolumePrivilege Present Manage the files on a volume
3880    WebCompanionIn  29      SeImpersonatePrivilege  Present,Enabled,Default Impersonate a client after authentication
3880    WebCompanionIn  30      SeCreateGlobalPrivilege Present,Enabled,Default Create global objects
3880    WebCompanionIn  31      SeTrustedCredManAccessPrivilege         Access Credential Manager as a trusted caller
3880    WebCompanionIn  32      SeRelabelPrivilege              Modify the mandatory integrity level of an object
3880    WebCompanionIn  33      SeIncreaseWorkingSetPrivilege   Present,Enabled,Default Allocate more memory for user applications
3880    WebCompanionIn  34      SeTimeZonePrivilege     Present,Enabled,Default Adjust the time zone of the computer's internal clock
3880    WebCompanionIn  35      SeCreateSymbolicLinkPrivilege   Present,Enabled,Default Required to create a symbolic link
3880    WebCompanionIn  36      SeDelegateSessionUserImpersonatePrivilege               Obtain an impersonation token for another user in the same session.
3648    chrome.exe      2       SeCreateTokenPrivilege          Create a token object
3648    chrome.exe      3       SeAssignPrimaryTokenPrivilege           Replace a process-level token
3648    chrome.exe      4       SeLockMemoryPrivilege           Lock pages in memory
3648    chrome.exe      5       SeIncreaseQuotaPrivilege                Increase quotas
3648    chrome.exe      6       SeMachineAccountPrivilege               Add workstations to the domain
3648    chrome.exe      7       SeTcbPrivilege          Act as part of the operating system
3648    chrome.exe      8       SeSecurityPrivilege             Manage auditing and security log
3648    chrome.exe      9       SeTakeOwnershipPrivilege                Take ownership of files/objects
3648    chrome.exe      10      SeLoadDriverPrivilege           Load and unload device drivers
3648    chrome.exe      11      SeSystemProfilePrivilege                Profile system performance
3648    chrome.exe      12      SeSystemtimePrivilege           Change the system time
3648    chrome.exe      13      SeProfileSingleProcessPrivilege         Profile a single process
3648    chrome.exe      14      SeIncreaseBasePriorityPrivilege         Increase scheduling priority
3648    chrome.exe      15      SeCreatePagefilePrivilege               Create a pagefile
3648    chrome.exe      16      SeCreatePermanentPrivilege              Create permanent shared objects
3648    chrome.exe      17      SeBackupPrivilege               Backup files and directories
3648    chrome.exe      18      SeRestorePrivilege              Restore files and directories
3648    chrome.exe      19      SeShutdownPrivilege             Shut down the system
3648    chrome.exe      20      SeDebugPrivilege                Debug programs
3648    chrome.exe      21      SeAuditPrivilege                Generate security audits
3648    chrome.exe      22      SeSystemEnvironmentPrivilege            Edit firmware environment values
3648    chrome.exe      23      SeChangeNotifyPrivilege Default Receive notifications of changes to files or directories
3648    chrome.exe      24      SeRemoteShutdownPrivilege               Force shutdown from a remote system
3648    chrome.exe      25      SeUndockPrivilege               Remove computer from docking station
3648    chrome.exe      26      SeSyncAgentPrivilege            Synch directory service data
3648    chrome.exe      27      SeEnableDelegationPrivilege             Enable user accounts to be trusted for delegation
3648    chrome.exe      28      SeManageVolumePrivilege         Manage the files on a volume
3648    chrome.exe      29      SeImpersonatePrivilege          Impersonate a client after authentication
3648    chrome.exe      30      SeCreateGlobalPrivilege         Create global objects
3648    chrome.exe      31      SeTrustedCredManAccessPrivilege         Access Credential Manager as a trusted caller
3648    chrome.exe      32      SeRelabelPrivilege              Modify the mandatory integrity level of an object
3648    chrome.exe      33      SeIncreaseWorkingSetPrivilege           Allocate more memory for user applications
3648    chrome.exe      34      SeTimeZonePrivilege             Adjust the time zone of the computer's internal clock
3648    chrome.exe      35      SeCreateSymbolicLinkPrivilege           Required to create a symbolic link
3648    chrome.exe      36      SeDelegateSessionUserImpersonatePrivilege               Obtain an impersonation token for another user in the same session.
1796    chrome.exe      2       SeCreateTokenPrivilege          Create a token object
1796    chrome.exe      3       SeAssignPrimaryTokenPrivilege           Replace a process-level token
1796    chrome.exe      4       SeLockMemoryPrivilege           Lock pages in memory
1796    chrome.exe      5       SeIncreaseQuotaPrivilege                Increase quotas
1796    chrome.exe      6       SeMachineAccountPrivilege               Add workstations to the domain
1796    chrome.exe      7       SeTcbPrivilege          Act as part of the operating system
1796    chrome.exe      8       SeSecurityPrivilege             Manage auditing and security log
1796    chrome.exe      9       SeTakeOwnershipPrivilege                Take ownership of files/objects
1796    chrome.exe      10      SeLoadDriverPrivilege           Load and unload device drivers
1796    chrome.exe      11      SeSystemProfilePrivilege                Profile system performance
1796    chrome.exe      12      SeSystemtimePrivilege           Change the system time
1796    chrome.exe      13      SeProfileSingleProcessPrivilege         Profile a single process
1796    chrome.exe      14      SeIncreaseBasePriorityPrivilege         Increase scheduling priority
1796    chrome.exe      15      SeCreatePagefilePrivilege               Create a pagefile
1796    chrome.exe      16      SeCreatePermanentPrivilege              Create permanent shared objects
1796    chrome.exe      17      SeBackupPrivilege               Backup files and directories
1796    chrome.exe      18      SeRestorePrivilege              Restore files and directories
1796    chrome.exe      19      SeShutdownPrivilege             Shut down the system
1796    chrome.exe      20      SeDebugPrivilege                Debug programs
1796    chrome.exe      21      SeAuditPrivilege                Generate security audits
1796    chrome.exe      22      SeSystemEnvironmentPrivilege            Edit firmware environment values
1796    chrome.exe      23      SeChangeNotifyPrivilege Default Receive notifications of changes to files or directories
1796    chrome.exe      24      SeRemoteShutdownPrivilege               Force shutdown from a remote system
1796    chrome.exe      25      SeUndockPrivilege               Remove computer from docking station
1796    chrome.exe      26      SeSyncAgentPrivilege            Synch directory service data
1796    chrome.exe      27      SeEnableDelegationPrivilege             Enable user accounts to be trusted for delegation
1796    chrome.exe      28      SeManageVolumePrivilege         Manage the files on a volume
1796    chrome.exe      29      SeImpersonatePrivilege          Impersonate a client after authentication
1796    chrome.exe      30      SeCreateGlobalPrivilege         Create global objects
1796    chrome.exe      31      SeTrustedCredManAccessPrivilege         Access Credential Manager as a trusted caller
1796    chrome.exe      32      SeRelabelPrivilege              Modify the mandatory integrity level of an object
1796    chrome.exe      33      SeIncreaseWorkingSetPrivilege           Allocate more memory for user applications
1796    chrome.exe      34      SeTimeZonePrivilege             Adjust the time zone of the computer's internal clock
1796    chrome.exe      35      SeCreateSymbolicLinkPrivilege           Required to create a symbolic link
1796    chrome.exe      36      SeDelegateSessionUserImpersonatePrivilege               Obtain an impersonation token for another user in the same session.
3208    sc.exe  2       SeCreateTokenPrivilege          Create a token object
3208    sc.exe  3       SeAssignPrimaryTokenPrivilege   Present Replace a process-level token
3208    sc.exe  4       SeLockMemoryPrivilege   Present,Enabled,Default Lock pages in memory
3208    sc.exe  5       SeIncreaseQuotaPrivilege        Present Increase quotas
3208    sc.exe  6       SeMachineAccountPrivilege               Add workstations to the domain
3208    sc.exe  7       SeTcbPrivilege  Present,Enabled,Default Act as part of the operating system
3208    sc.exe  8       SeSecurityPrivilege     Present Manage auditing and security log
3208    sc.exe  9       SeTakeOwnershipPrivilege        Present Take ownership of files/objects
3208    sc.exe  10      SeLoadDriverPrivilege   Present Load and unload device drivers
3208    sc.exe  11      SeSystemProfilePrivilege        Present,Enabled,Default Profile system performance
3208    sc.exe  12      SeSystemtimePrivilege   Present Change the system time
3208    sc.exe  13      SeProfileSingleProcessPrivilege Present,Enabled,Default Profile a single process
3208    sc.exe  14      SeIncreaseBasePriorityPrivilege Present,Enabled,Default Increase scheduling priority
3208    sc.exe  15      SeCreatePagefilePrivilege       Present,Enabled,Default Create a pagefile
3208    sc.exe  16      SeCreatePermanentPrivilege      Present,Enabled,Default Create permanent shared objects
3208    sc.exe  17      SeBackupPrivilege       Present Backup files and directories
3208    sc.exe  18      SeRestorePrivilege      Present Restore files and directories
3208    sc.exe  19      SeShutdownPrivilege     Present Shut down the system
3208    sc.exe  20      SeDebugPrivilege        Present,Enabled,Default Debug programs
3208    sc.exe  21      SeAuditPrivilege        Present,Enabled,Default Generate security audits
3208    sc.exe  22      SeSystemEnvironmentPrivilege    Present Edit firmware environment values
3208    sc.exe  23      SeChangeNotifyPrivilege Present,Enabled,Default Receive notifications of changes to files or directories
3208    sc.exe  24      SeRemoteShutdownPrivilege               Force shutdown from a remote system
3208    sc.exe  25      SeUndockPrivilege       Present Remove computer from docking station
3208    sc.exe  26      SeSyncAgentPrivilege            Synch directory service data
3208    sc.exe  27      SeEnableDelegationPrivilege             Enable user accounts to be trusted for delegation
3208    sc.exe  28      SeManageVolumePrivilege Present Manage the files on a volume
3208    sc.exe  29      SeImpersonatePrivilege  Present,Enabled,Default Impersonate a client after authentication
3208    sc.exe  30      SeCreateGlobalPrivilege Present,Enabled,Default Create global objects
3208    sc.exe  31      SeTrustedCredManAccessPrivilege         Access Credential Manager as a trusted caller
3208    sc.exe  32      SeRelabelPrivilege              Modify the mandatory integrity level of an object
3208    sc.exe  33      SeIncreaseWorkingSetPrivilege   Present,Enabled,Default Allocate more memory for user applications
3208    sc.exe  34      SeTimeZonePrivilege     Present,Enabled,Default Adjust the time zone of the computer's internal clock
3208    sc.exe  35      SeCreateSymbolicLinkPrivilege   Present,Enabled,Default Required to create a symbolic link
3208    sc.exe  36      SeDelegateSessionUserImpersonatePrivilege               Obtain an impersonation token for another user in the same session.
452     sc.exe  2       SeCreateTokenPrivilege          Create a token object
452     sc.exe  3       SeAssignPrimaryTokenPrivilege   Present Replace a process-level token
452     sc.exe  4       SeLockMemoryPrivilege   Present,Enabled,Default Lock pages in memory
452     sc.exe  5       SeIncreaseQuotaPrivilege        Present Increase quotas
452     sc.exe  6       SeMachineAccountPrivilege               Add workstations to the domain
452     sc.exe  7       SeTcbPrivilege  Present,Enabled,Default Act as part of the operating system
452     sc.exe  8       SeSecurityPrivilege     Present Manage auditing and security log
452     sc.exe  9       SeTakeOwnershipPrivilege        Present Take ownership of files/objects
452     sc.exe  10      SeLoadDriverPrivilege   Present Load and unload device drivers
452     sc.exe  11      SeSystemProfilePrivilege        Present,Enabled,Default Profile system performance
452     sc.exe  12      SeSystemtimePrivilege   Present Change the system time
452     sc.exe  13      SeProfileSingleProcessPrivilege Present,Enabled,Default Profile a single process
452     sc.exe  14      SeIncreaseBasePriorityPrivilege Present,Enabled,Default Increase scheduling priority
452     sc.exe  15      SeCreatePagefilePrivilege       Present,Enabled,Default Create a pagefile
452     sc.exe  16      SeCreatePermanentPrivilege      Present,Enabled,Default Create permanent shared objects
452     sc.exe  17      SeBackupPrivilege       Present Backup files and directories
452     sc.exe  18      SeRestorePrivilege      Present Restore files and directories
452     sc.exe  19      SeShutdownPrivilege     Present Shut down the system
452     sc.exe  20      SeDebugPrivilege        Present,Enabled,Default Debug programs
452     sc.exe  21      SeAuditPrivilege        Present,Enabled,Default Generate security audits
452     sc.exe  22      SeSystemEnvironmentPrivilege    Present Edit firmware environment values
452     sc.exe  23      SeChangeNotifyPrivilege Present,Enabled,Default Receive notifications of changes to files or directories
452     sc.exe  24      SeRemoteShutdownPrivilege               Force shutdown from a remote system
452     sc.exe  25      SeUndockPrivilege       Present Remove computer from docking station
452     sc.exe  26      SeSyncAgentPrivilege            Synch directory service data
452     sc.exe  27      SeEnableDelegationPrivilege             Enable user accounts to be trusted for delegation
452     sc.exe  28      SeManageVolumePrivilege Present Manage the files on a volume
452     sc.exe  29      SeImpersonatePrivilege  Present,Enabled,Default Impersonate a client after authentication
452     sc.exe  30      SeCreateGlobalPrivilege Present,Enabled,Default Create global objects
452     sc.exe  31      SeTrustedCredManAccessPrivilege         Access Credential Manager as a trusted caller
452     sc.exe  32      SeRelabelPrivilege              Modify the mandatory integrity level of an object
452     sc.exe  33      SeIncreaseWorkingSetPrivilege   Present,Enabled,Default Allocate more memory for user applications
452     sc.exe  34      SeTimeZonePrivilege     Present,Enabled,Default Adjust the time zone of the computer's internal clock
452     sc.exe  35      SeCreateSymbolicLinkPrivilege   Present,Enabled,Default Required to create a symbolic link
452     sc.exe  36      SeDelegateSessionUserImpersonatePrivilege               Obtain an impersonation token for another user in the same session.
3504    sc.exe  2       SeCreateTokenPrivilege          Create a token object
3504    sc.exe  3       SeAssignPrimaryTokenPrivilege   Present Replace a process-level token
3504    sc.exe  4       SeLockMemoryPrivilege   Present,Enabled,Default Lock pages in memory
3504    sc.exe  5       SeIncreaseQuotaPrivilege        Present Increase quotas
3504    sc.exe  6       SeMachineAccountPrivilege               Add workstations to the domain
3504    sc.exe  7       SeTcbPrivilege  Present,Enabled,Default Act as part of the operating system
3504    sc.exe  8       SeSecurityPrivilege     Present Manage auditing and security log
3504    sc.exe  9       SeTakeOwnershipPrivilege        Present Take ownership of files/objects
3504    sc.exe  10      SeLoadDriverPrivilege   Present Load and unload device drivers
3504    sc.exe  11      SeSystemProfilePrivilege        Present,Enabled,Default Profile system performance
3504    sc.exe  12      SeSystemtimePrivilege   Present Change the system time
3504    sc.exe  13      SeProfileSingleProcessPrivilege Present,Enabled,Default Profile a single process
3504    sc.exe  14      SeIncreaseBasePriorityPrivilege Present,Enabled,Default Increase scheduling priority
3504    sc.exe  15      SeCreatePagefilePrivilege       Present,Enabled,Default Create a pagefile
3504    sc.exe  16      SeCreatePermanentPrivilege      Present,Enabled,Default Create permanent shared objects
3504    sc.exe  17      SeBackupPrivilege       Present Backup files and directories
3504    sc.exe  18      SeRestorePrivilege      Present Restore files and directories
3504    sc.exe  19      SeShutdownPrivilege     Present Shut down the system
3504    sc.exe  20      SeDebugPrivilege        Present,Enabled,Default Debug programs
3504    sc.exe  21      SeAuditPrivilege        Present,Enabled,Default Generate security audits
3504    sc.exe  22      SeSystemEnvironmentPrivilege    Present Edit firmware environment values
3504    sc.exe  23      SeChangeNotifyPrivilege Present,Enabled,Default Receive notifications of changes to files or directories
3504    sc.exe  24      SeRemoteShutdownPrivilege               Force shutdown from a remote system
3504    sc.exe  25      SeUndockPrivilege       Present Remove computer from docking station
3504    sc.exe  26      SeSyncAgentPrivilege            Synch directory service data
3504    sc.exe  27      SeEnableDelegationPrivilege             Enable user accounts to be trusted for delegation
3504    sc.exe  28      SeManageVolumePrivilege Present Manage the files on a volume
3504    sc.exe  29      SeImpersonatePrivilege  Present,Enabled,Default Impersonate a client after authentication
3504    sc.exe  30      SeCreateGlobalPrivilege Present,Enabled,Default Create global objects
3504    sc.exe  31      SeTrustedCredManAccessPrivilege         Access Credential Manager as a trusted caller
3504    sc.exe  32      SeRelabelPrivilege              Modify the mandatory integrity level of an object
3504    sc.exe  33      SeIncreaseWorkingSetPrivilege   Present,Enabled,Default Allocate more memory for user applications
3504    sc.exe  34      SeTimeZonePrivilege     Present,Enabled,Default Adjust the time zone of the computer's internal clock
3504    sc.exe  35      SeCreateSymbolicLinkPrivilege   Present,Enabled,Default Required to create a symbolic link
3504    sc.exe  36      SeDelegateSessionUserImpersonatePrivilege               Obtain an impersonation token for another user in the same session.
2028    sc.exe  2       SeCreateTokenPrivilege          Create a token object
2028    sc.exe  3       SeAssignPrimaryTokenPrivilege   Present Replace a process-level token
2028    sc.exe  4       SeLockMemoryPrivilege   Present,Enabled,Default Lock pages in memory
2028    sc.exe  5       SeIncreaseQuotaPrivilege        Present Increase quotas
2028    sc.exe  6       SeMachineAccountPrivilege               Add workstations to the domain
2028    sc.exe  7       SeTcbPrivilege  Present,Enabled,Default Act as part of the operating system
2028    sc.exe  8       SeSecurityPrivilege     Present Manage auditing and security log
2028    sc.exe  9       SeTakeOwnershipPrivilege        Present Take ownership of files/objects
2028    sc.exe  10      SeLoadDriverPrivilege   Present Load and unload device drivers
2028    sc.exe  11      SeSystemProfilePrivilege        Present,Enabled,Default Profile system performance
2028    sc.exe  12      SeSystemtimePrivilege   Present Change the system time
2028    sc.exe  13      SeProfileSingleProcessPrivilege Present,Enabled,Default Profile a single process
2028    sc.exe  14      SeIncreaseBasePriorityPrivilege Present,Enabled,Default Increase scheduling priority
2028    sc.exe  15      SeCreatePagefilePrivilege       Present,Enabled,Default Create a pagefile
2028    sc.exe  16      SeCreatePermanentPrivilege      Present,Enabled,Default Create permanent shared objects
2028    sc.exe  17      SeBackupPrivilege       Present Backup files and directories
2028    sc.exe  18      SeRestorePrivilege      Present Restore files and directories
2028    sc.exe  19      SeShutdownPrivilege     Present Shut down the system
2028    sc.exe  20      SeDebugPrivilege        Present,Enabled,Default Debug programs
2028    sc.exe  21      SeAuditPrivilege        Present,Enabled,Default Generate security audits
2028    sc.exe  22      SeSystemEnvironmentPrivilege    Present Edit firmware environment values
2028    sc.exe  23      SeChangeNotifyPrivilege Present,Enabled,Default Receive notifications of changes to files or directories
2028    sc.exe  24      SeRemoteShutdownPrivilege               Force shutdown from a remote system
2028    sc.exe  25      SeUndockPrivilege       Present Remove computer from docking station
2028    sc.exe  26      SeSyncAgentPrivilege            Synch directory service data
2028    sc.exe  27      SeEnableDelegationPrivilege             Enable user accounts to be trusted for delegation
2028    sc.exe  28      SeManageVolumePrivilege Present Manage the files on a volume
2028    sc.exe  29      SeImpersonatePrivilege  Present,Enabled,Default Impersonate a client after authentication
2028    sc.exe  30      SeCreateGlobalPrivilege Present,Enabled,Default Create global objects
2028    sc.exe  31      SeTrustedCredManAccessPrivilege         Access Credential Manager as a trusted caller
2028    sc.exe  32      SeRelabelPrivilege              Modify the mandatory integrity level of an object
2028    sc.exe  33      SeIncreaseWorkingSetPrivilege   Present,Enabled,Default Allocate more memory for user applications
2028    sc.exe  34      SeTimeZonePrivilege     Present,Enabled,Default Adjust the time zone of the computer's internal clock
2028    sc.exe  35      SeCreateSymbolicLinkPrivilege   Present,Enabled,Default Required to create a symbolic link
2028    sc.exe  36      SeDelegateSessionUserImpersonatePrivilege               Obtain an impersonation token for another user in the same session.
3496    Lavasoft.WCAss  2       SeCreateTokenPrivilege          Create a token object
3496    Lavasoft.WCAss  3       SeAssignPrimaryTokenPrivilege   Present Replace a process-level token
3496    Lavasoft.WCAss  4       SeLockMemoryPrivilege   Present,Enabled,Default Lock pages in memory
3496    Lavasoft.WCAss  5       SeIncreaseQuotaPrivilege        Present Increase quotas
3496    Lavasoft.WCAss  6       SeMachineAccountPrivilege               Add workstations to the domain
3496    Lavasoft.WCAss  7       SeTcbPrivilege  Present,Enabled,Default Act as part of the operating system
3496    Lavasoft.WCAss  8       SeSecurityPrivilege     Present Manage auditing and security log
3496    Lavasoft.WCAss  9       SeTakeOwnershipPrivilege        Present Take ownership of files/objects
3496    Lavasoft.WCAss  10      SeLoadDriverPrivilege   Present Load and unload device drivers
3496    Lavasoft.WCAss  11      SeSystemProfilePrivilege        Present,Enabled,Default Profile system performance
3496    Lavasoft.WCAss  12      SeSystemtimePrivilege   Present Change the system time
3496    Lavasoft.WCAss  13      SeProfileSingleProcessPrivilege Present,Enabled,Default Profile a single process
3496    Lavasoft.WCAss  14      SeIncreaseBasePriorityPrivilege Present,Enabled,Default Increase scheduling priority
3496    Lavasoft.WCAss  15      SeCreatePagefilePrivilege       Present,Enabled,Default Create a pagefile
3496    Lavasoft.WCAss  16      SeCreatePermanentPrivilege      Present,Enabled,Default Create permanent shared objects
3496    Lavasoft.WCAss  17      SeBackupPrivilege       Present Backup files and directories
3496    Lavasoft.WCAss  18      SeRestorePrivilege      Present Restore files and directories
3496    Lavasoft.WCAss  19      SeShutdownPrivilege     Present Shut down the system
3496    Lavasoft.WCAss  20      SeDebugPrivilege        Present,Enabled,Default Debug programs
3496    Lavasoft.WCAss  21      SeAuditPrivilege        Present,Enabled,Default Generate security audits
3496    Lavasoft.WCAss  22      SeSystemEnvironmentPrivilege    Present Edit firmware environment values
3496    Lavasoft.WCAss  23      SeChangeNotifyPrivilege Present,Enabled,Default Receive notifications of changes to files or directories
3496    Lavasoft.WCAss  24      SeRemoteShutdownPrivilege               Force shutdown from a remote system
3496    Lavasoft.WCAss  25      SeUndockPrivilege       Present Remove computer from docking station
3496    Lavasoft.WCAss  26      SeSyncAgentPrivilege            Synch directory service data
3496    Lavasoft.WCAss  27      SeEnableDelegationPrivilege             Enable user accounts to be trusted for delegation
3496    Lavasoft.WCAss  28      SeManageVolumePrivilege Present Manage the files on a volume
3496    Lavasoft.WCAss  29      SeImpersonatePrivilege  Present,Enabled,Default Impersonate a client after authentication
3496    Lavasoft.WCAss  30      SeCreateGlobalPrivilege Present,Enabled,Default Create global objects
3496    Lavasoft.WCAss  31      SeTrustedCredManAccessPrivilege         Access Credential Manager as a trusted caller
3496    Lavasoft.WCAss  32      SeRelabelPrivilege              Modify the mandatory integrity level of an object
3496    Lavasoft.WCAss  33      SeIncreaseWorkingSetPrivilege   Present,Enabled,Default Allocate more memory for user applications
3496    Lavasoft.WCAss  34      SeTimeZonePrivilege     Present,Enabled,Default Adjust the time zone of the computer's internal clock
3496    Lavasoft.WCAss  35      SeCreateSymbolicLinkPrivilege   Present,Enabled,Default Required to create a symbolic link
3496    Lavasoft.WCAss  36      SeDelegateSessionUserImpersonatePrivilege               Obtain an impersonation token for another user in the same session.
3856    WebCompanion.e  2       SeCreateTokenPrivilege          Create a token object
3856    WebCompanion.e  3       SeAssignPrimaryTokenPrivilege   Present Replace a process-level token
3856    WebCompanion.e  4       SeLockMemoryPrivilege   Present,Enabled,Default Lock pages in memory
3856    WebCompanion.e  5       SeIncreaseQuotaPrivilege        Present Increase quotas
3856    WebCompanion.e  6       SeMachineAccountPrivilege               Add workstations to the domain
3856    WebCompanion.e  7       SeTcbPrivilege  Present,Enabled,Default Act as part of the operating system
3856    WebCompanion.e  8       SeSecurityPrivilege     Present Manage auditing and security log
3856    WebCompanion.e  9       SeTakeOwnershipPrivilege        Present Take ownership of files/objects
3856    WebCompanion.e  10      SeLoadDriverPrivilege   Present Load and unload device drivers
3856    WebCompanion.e  11      SeSystemProfilePrivilege        Present,Enabled,Default Profile system performance
3856    WebCompanion.e  12      SeSystemtimePrivilege   Present Change the system time
3856    WebCompanion.e  13      SeProfileSingleProcessPrivilege Present,Enabled,Default Profile a single process
3856    WebCompanion.e  14      SeIncreaseBasePriorityPrivilege Present,Enabled,Default Increase scheduling priority
3856    WebCompanion.e  15      SeCreatePagefilePrivilege       Present,Enabled,Default Create a pagefile
3856    WebCompanion.e  16      SeCreatePermanentPrivilege      Present,Enabled,Default Create permanent shared objects
3856    WebCompanion.e  17      SeBackupPrivilege       Present Backup files and directories
3856    WebCompanion.e  18      SeRestorePrivilege      Present Restore files and directories
3856    WebCompanion.e  19      SeShutdownPrivilege     Present Shut down the system
3856    WebCompanion.e  20      SeDebugPrivilege        Present,Enabled,Default Debug programs
3856    WebCompanion.e  21      SeAuditPrivilege        Present,Enabled,Default Generate security audits
3856    WebCompanion.e  22      SeSystemEnvironmentPrivilege    Present Edit firmware environment values
3856    WebCompanion.e  23      SeChangeNotifyPrivilege Present,Enabled,Default Receive notifications of changes to files or directories
3856    WebCompanion.e  24      SeRemoteShutdownPrivilege               Force shutdown from a remote system
3856    WebCompanion.e  25      SeUndockPrivilege       Present Remove computer from docking station
3856    WebCompanion.e  26      SeSyncAgentPrivilege            Synch directory service data
3856    WebCompanion.e  27      SeEnableDelegationPrivilege             Enable user accounts to be trusted for delegation
3856    WebCompanion.e  28      SeManageVolumePrivilege Present Manage the files on a volume
3856    WebCompanion.e  29      SeImpersonatePrivilege  Present,Enabled,Default Impersonate a client after authentication
3856    WebCompanion.e  30      SeCreateGlobalPrivilege Present,Enabled,Default Create global objects
3856    WebCompanion.e  31      SeTrustedCredManAccessPrivilege         Access Credential Manager as a trusted caller
3856    WebCompanion.e  32      SeRelabelPrivilege              Modify the mandatory integrity level of an object
3856    WebCompanion.e  33      SeIncreaseWorkingSetPrivilege   Present,Enabled,Default Allocate more memory for user applications
3856    WebCompanion.e  34      SeTimeZonePrivilege     Present,Enabled,Default Adjust the time zone of the computer's internal clock
3856    WebCompanion.e  35      SeCreateSymbolicLinkPrivilege   Present,Enabled,Default Required to create a symbolic link
3856    WebCompanion.e  36      SeDelegateSessionUserImpersonatePrivilege               Obtain an impersonation token for another user in the same session.
3304    notepad.exe     2       SeCreateTokenPrivilege          Create a token object
3304    notepad.exe     3       SeAssignPrimaryTokenPrivilege           Replace a process-level token
3304    notepad.exe     4       SeLockMemoryPrivilege           Lock pages in memory
3304    notepad.exe     5       SeIncreaseQuotaPrivilege                Increase quotas
3304    notepad.exe     6       SeMachineAccountPrivilege               Add workstations to the domain
3304    notepad.exe     7       SeTcbPrivilege          Act as part of the operating system
3304    notepad.exe     8       SeSecurityPrivilege             Manage auditing and security log
3304    notepad.exe     9       SeTakeOwnershipPrivilege                Take ownership of files/objects
3304    notepad.exe     10      SeLoadDriverPrivilege           Load and unload device drivers
3304    notepad.exe     11      SeSystemProfilePrivilege                Profile system performance
3304    notepad.exe     12      SeSystemtimePrivilege           Change the system time
3304    notepad.exe     13      SeProfileSingleProcessPrivilege         Profile a single process
3304    notepad.exe     14      SeIncreaseBasePriorityPrivilege         Increase scheduling priority
3304    notepad.exe     15      SeCreatePagefilePrivilege               Create a pagefile
3304    notepad.exe     16      SeCreatePermanentPrivilege              Create permanent shared objects
3304    notepad.exe     17      SeBackupPrivilege               Backup files and directories
3304    notepad.exe     18      SeRestorePrivilege              Restore files and directories
3304    notepad.exe     19      SeShutdownPrivilege     Present Shut down the system
3304    notepad.exe     20      SeDebugPrivilege                Debug programs
3304    notepad.exe     21      SeAuditPrivilege                Generate security audits
3304    notepad.exe     22      SeSystemEnvironmentPrivilege            Edit firmware environment values
3304    notepad.exe     23      SeChangeNotifyPrivilege Present,Enabled,Default Receive notifications of changes to files or directories
3304    notepad.exe     24      SeRemoteShutdownPrivilege               Force shutdown from a remote system
3304    notepad.exe     25      SeUndockPrivilege       Present Remove computer from docking station
3304    notepad.exe     26      SeSyncAgentPrivilege            Synch directory service data
3304    notepad.exe     27      SeEnableDelegationPrivilege             Enable user accounts to be trusted for delegation
3304    notepad.exe     28      SeManageVolumePrivilege         Manage the files on a volume
3304    notepad.exe     29      SeImpersonatePrivilege          Impersonate a client after authentication
3304    notepad.exe     30      SeCreateGlobalPrivilege         Create global objects
3304    notepad.exe     31      SeTrustedCredManAccessPrivilege         Access Credential Manager as a trusted caller
3304    notepad.exe     32      SeRelabelPrivilege              Modify the mandatory integrity level of an object
3304    notepad.exe     33      SeIncreaseWorkingSetPrivilege   Present Allocate more memory for user applications
3304    notepad.exe     34      SeTimeZonePrivilege     Present Adjust the time zone of the computer's internal clock
3304    notepad.exe     35      SeCreateSymbolicLinkPrivilege           Required to create a symbolic link
3304    notepad.exe     36      SeDelegateSessionUserImpersonatePrivilege               Obtain an impersonation token for another user in the same session.
3916    cmd.exe 2       SeCreateTokenPrivilege          Create a token object
3916    cmd.exe 3       SeAssignPrimaryTokenPrivilege   Present Replace a process-level token
3916    cmd.exe 4       SeLockMemoryPrivilege   Present,Enabled,Default Lock pages in memory
3916    cmd.exe 5       SeIncreaseQuotaPrivilege        Present Increase quotas
3916    cmd.exe 6       SeMachineAccountPrivilege               Add workstations to the domain
3916    cmd.exe 7       SeTcbPrivilege  Present,Enabled,Default Act as part of the operating system
3916    cmd.exe 8       SeSecurityPrivilege     Present Manage auditing and security log
3916    cmd.exe 9       SeTakeOwnershipPrivilege        Present Take ownership of files/objects
3916    cmd.exe 10      SeLoadDriverPrivilege   Present Load and unload device drivers
3916    cmd.exe 11      SeSystemProfilePrivilege        Present,Enabled,Default Profile system performance
3916    cmd.exe 12      SeSystemtimePrivilege   Present Change the system time
3916    cmd.exe 13      SeProfileSingleProcessPrivilege Present,Enabled,Default Profile a single process
3916    cmd.exe 14      SeIncreaseBasePriorityPrivilege Present,Enabled,Default Increase scheduling priority
3916    cmd.exe 15      SeCreatePagefilePrivilege       Present,Enabled,Default Create a pagefile
3916    cmd.exe 16      SeCreatePermanentPrivilege      Present,Enabled,Default Create permanent shared objects
3916    cmd.exe 17      SeBackupPrivilege       Present Backup files and directories
3916    cmd.exe 18      SeRestorePrivilege      Present Restore files and directories
3916    cmd.exe 19      SeShutdownPrivilege     Present Shut down the system
3916    cmd.exe 20      SeDebugPrivilege        Present,Enabled,Default Debug programs
3916    cmd.exe 21      SeAuditPrivilege        Present,Enabled,Default Generate security audits
3916    cmd.exe 22      SeSystemEnvironmentPrivilege    Present Edit firmware environment values
3916    cmd.exe 23      SeChangeNotifyPrivilege Present,Enabled,Default Receive notifications of changes to files or directories
3916    cmd.exe 24      SeRemoteShutdownPrivilege               Force shutdown from a remote system
3916    cmd.exe 25      SeUndockPrivilege       Present Remove computer from docking station
3916    cmd.exe 26      SeSyncAgentPrivilege            Synch directory service data
3916    cmd.exe 27      SeEnableDelegationPrivilege             Enable user accounts to be trusted for delegation
3916    cmd.exe 28      SeManageVolumePrivilege Present Manage the files on a volume
3916    cmd.exe 29      SeImpersonatePrivilege  Present,Enabled,Default Impersonate a client after authentication
3916    cmd.exe 30      SeCreateGlobalPrivilege Present,Enabled,Default Create global objects
3916    cmd.exe 31      SeTrustedCredManAccessPrivilege         Access Credential Manager as a trusted caller
3916    cmd.exe 32      SeRelabelPrivilege              Modify the mandatory integrity level of an object
3916    cmd.exe 33      SeIncreaseWorkingSetPrivilege   Present,Enabled,Default Allocate more memory for user applications
3916    cmd.exe 34      SeTimeZonePrivilege     Present,Enabled,Default Adjust the time zone of the computer's internal clock
3916    cmd.exe 35      SeCreateSymbolicLinkPrivilege   Present,Enabled,Default Required to create a symbolic link
3916    cmd.exe 36      SeDelegateSessionUserImpersonatePrivilege               Obtain an impersonation token for another user in the same session.
2420    conhost.exe     2       SeCreateTokenPrivilege          Create a token object
2420    conhost.exe     3       SeAssignPrimaryTokenPrivilege   Present Replace a process-level token
2420    conhost.exe     4       SeLockMemoryPrivilege   Present,Enabled,Default Lock pages in memory
2420    conhost.exe     5       SeIncreaseQuotaPrivilege        Present Increase quotas
2420    conhost.exe     6       SeMachineAccountPrivilege               Add workstations to the domain
2420    conhost.exe     7       SeTcbPrivilege  Present,Enabled,Default Act as part of the operating system
2420    conhost.exe     8       SeSecurityPrivilege     Present Manage auditing and security log
2420    conhost.exe     9       SeTakeOwnershipPrivilege        Present Take ownership of files/objects
2420    conhost.exe     10      SeLoadDriverPrivilege   Present Load and unload device drivers
2420    conhost.exe     11      SeSystemProfilePrivilege        Present,Enabled,Default Profile system performance
2420    conhost.exe     12      SeSystemtimePrivilege   Present Change the system time
2420    conhost.exe     13      SeProfileSingleProcessPrivilege Present,Enabled,Default Profile a single process
2420    conhost.exe     14      SeIncreaseBasePriorityPrivilege Present,Enabled,Default Increase scheduling priority
2420    conhost.exe     15      SeCreatePagefilePrivilege       Present,Enabled,Default Create a pagefile
2420    conhost.exe     16      SeCreatePermanentPrivilege      Present,Enabled,Default Create permanent shared objects
2420    conhost.exe     17      SeBackupPrivilege       Present Backup files and directories
2420    conhost.exe     18      SeRestorePrivilege      Present Restore files and directories
2420    conhost.exe     19      SeShutdownPrivilege     Present Shut down the system
2420    conhost.exe     20      SeDebugPrivilege        Present,Enabled,Default Debug programs
2420    conhost.exe     21      SeAuditPrivilege        Present,Enabled,Default Generate security audits
2420    conhost.exe     22      SeSystemEnvironmentPrivilege    Present Edit firmware environment values
2420    conhost.exe     23      SeChangeNotifyPrivilege Present,Enabled,Default Receive notifications of changes to files or directories
2420    conhost.exe     24      SeRemoteShutdownPrivilege               Force shutdown from a remote system
2420    conhost.exe     25      SeUndockPrivilege       Present Remove computer from docking station
2420    conhost.exe     26      SeSyncAgentPrivilege            Synch directory service data
2420    conhost.exe     27      SeEnableDelegationPrivilege             Enable user accounts to be trusted for delegation
2420    conhost.exe     28      SeManageVolumePrivilege Present Manage the files on a volume
2420    conhost.exe     29      SeImpersonatePrivilege  Present,Enabled,Default Impersonate a client after authentication
2420    conhost.exe     30      SeCreateGlobalPrivilege Present,Enabled,Default Create global objects
2420    conhost.exe     31      SeTrustedCredManAccessPrivilege         Access Credential Manager as a trusted caller
2420    conhost.exe     32      SeRelabelPrivilege              Modify the mandatory integrity level of an object
2420    conhost.exe     33      SeIncreaseWorkingSetPrivilege   Present,Enabled,Default Allocate more memory for user applications
2420    conhost.exe     34      SeTimeZonePrivilege     Present,Enabled,Default Adjust the time zone of the computer's internal clock
2420    conhost.exe     35      SeCreateSymbolicLinkPrivilege   Present,Enabled,Default Required to create a symbolic link
2420    conhost.exe     36      SeDelegateSessionUserImpersonatePrivilege               Obtain an impersonation token for another user in the same session.
```

# windows.privileges.Privs 分析

## 1. Plugin 功能說明

`windows.privileges.Privs` 用來列出各 Process Token 中的 Windows 權限狀態。

Windows 權限可以用來判斷 Process 是否具備較高的系統操作能力，例如：

```text
SeDebugPrivilege
SeBackupPrivilege
SeRestorePrivilege
SeLoadDriverPrivilege
SeTakeOwnershipPrivilege
SeImpersonatePrivilege
SeShutdownPrivilege
```

在惡意程式分析中，如果可疑 Process 具有大量啟用的高權限，可能代表它嘗試進行權限提升、除錯其他 Process、載入 Driver、備份/還原檔案，或進行系統層級操作。

---

## 2. 執行指令

```bash
.\vol.exe -f .\OtterCTF.vmem windows.privileges.Privs
```

---

## 3. 欄位說明

| 欄位            | 說明         |
| ------------- | ---------- |
| `PID`         | Process ID |
| `Process`     | Process 名稱 |
| `Value`       | 權限編號       |
| `Privilege`   | 權限名稱       |
| `Attributes`  | 權限狀態       |
| `Description` | 權限說明       |

`Attributes` 常見狀態如下：

| 狀態        | 說明                   |
| --------- | -------------------- |
| `Present` | Process Token 中存在此權限 |
| `Enabled` | 此權限目前已啟用             |
| `Default` | 此權限為預設狀態             |
| 空白        | 該權限未持有或未啟用           |

---

## 4. 系統 Process 權限觀察

結果中可以看到 `System`、`smss.exe`、`csrss.exe`、`lsass.exe`、`services.exe` 等系統 Process 具有較多高權限，例如：

```text
SeTcbPrivilege
SeDebugPrivilege
SeLoadDriverPrivilege
SeBackupPrivilege
SeRestorePrivilege
SeCreateTokenPrivilege
SeImpersonatePrivilege
```

這些 Process 屬於 Windows 系統核心或服務相關 Process，因此具有較高權限是正常現象。

---

## 5. PID 3820：Rick And Morty 權限分析

PID 3820 `Rick And Morty` 是本案主要可疑 Process。

其權限結果中，大部分高權限並未啟用，較明確出現的主要是：

```text
SeShutdownPrivilege    Present
SeChangeNotifyPrivilege    Present,Enabled,Default
SeUndockPrivilege    Present
SeIncreaseWorkingSetPrivilege    Present
```

其中 `SeChangeNotifyPrivilege` 是 Windows 一般 Process 常見權限，用於接收檔案或目錄變更通知，並不代表惡意。

未看到 PID 3820 明顯啟用以下高風險權限：

```text
SeDebugPrivilege    Enabled
SeLoadDriverPrivilege    Enabled
SeBackupPrivilege    Enabled
SeRestorePrivilege    Enabled
SeTakeOwnershipPrivilege    Enabled
```

因此，從 Privileges 角度來看，PID 3820 沒有明顯使用系統高權限或權限提升跡象。

---

## 6. PID 3720：vmware-tray.ex 權限分析

PID 3720 `vmware-tray.ex` 是 PID 3820 啟動出的可疑子 Process。

其權限結果中可看到部分權限為 `Present`，例如：

```text
SeIncreaseQuotaPrivilege
SeSecurityPrivilege
SeTakeOwnershipPrivilege
SeLoadDriverPrivilege
SeSystemProfilePrivilege
SeSystemtimePrivilege
SeProfileSingleProcessPrivilege
SeIncreaseBasePriorityPrivilege
SeCreatePagefilePrivilege
SeBackupPrivilege
SeRestorePrivilege
SeShutdownPrivilege
SeSystemEnvironmentPrivilege
SeRemoteShutdownPrivilege
SeUndockPrivilege
SeManageVolumePrivilege
SeDebugPrivilege
SeCreateSymbolicLinkPrivilege
```

但從結果來看，這些多數只是 `Present`，並沒有大量顯示為 `Enabled`。

比較明確的啟用權限主要是：

```text
SeChangeNotifyPrivilege    Present,Enabled,Default
SeImpersonatePrivilege     Present,Enabled,Default
SeCreateGlobalPrivilege    Present,Enabled,Default
```

這些權限在許多一般 Windows Process 中也可能出現，不能單獨判定為惡意。

---

## 7. 鑑識判斷

本次 `Privs` 結果沒有發現 PID 3820 或 PID 3720 出現明顯異常的高權限啟用狀態。

尤其沒有看到可疑 Process 明確啟用以下高風險權限：

```text
SeDebugPrivilege
SeLoadDriverPrivilege
SeBackupPrivilege
SeRestorePrivilege
SeTakeOwnershipPrivilege
```

因此，目前沒有證據顯示本案主要是透過權限提升、Driver 載入、LSASS 操作或系統權限濫用來執行攻擊。

---

## 8. 與本案關聯

本案主要證據仍集中於 User-mode 執行鏈：

```text
BitTorrent 下載活動
Rick And Morty season 1 download.exe
Temp\RarSFX0\vmware-tray.exe
Handles 顯示 PID 3820 持有 PID 3720 Process handle
Malfind / VadInfo 顯示 vmware-tray.exe 有可疑記憶體區段
READ_IT.txt 顯示檔案遭加密
```

`Privs` 的結果主要作為輔助檢查，用來確認可疑 Process 是否具備異常高權限。

本次結果顯示 PID 3820 與 PID 3720 並沒有明顯權限提升或高權限濫用跡象。

---

## 9. 結論

`windows.privileges.Privs` 成功列出系統中各 Process 的 Token 權限。

本次分析中，系統 Process 具有較多高權限屬於正常現象。

PID 3820 `Rick And Morty` 與 PID 3720 `vmware-tray.ex` 雖然具備部分一般權限，但沒有看到明顯異常的高權限啟用狀態。

因此，此 Plugin 結果顯示本案目前不像是以權限提升、Driver 載入或系統權限濫用為主的攻擊。

本案重點仍應放在：

```text
Rick And Morty season 1 download.exe
→ Temp\RarSFX0
→ vmware-tray.exe
→ 可疑記憶體區段
→ READ_IT.txt 加密提示
```
