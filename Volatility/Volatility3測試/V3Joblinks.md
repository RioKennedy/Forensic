# 測試內容
- vol.exe -f .\OtterCTF.vmem windows.joblinks.Joblinks

```
D:\Forensic\G140A006\VolatilityWorkbench>.\vol.exe -f .\OtterCTF.vmem windows.joblinks.JobLinks
Volatility 3 Framework 2.5.0
Progress:  100.00               PDB scanning finished
Offset(V)       Name    PID     PPID    Sess    JobSess Wow64   Total   Active  Term    JobLink Process

0xfa8019124b30  WmiPrvSE.exe    1800    604     0       0       False   2       2       0       N/A     (Original Process)
* 0xfa8019124b30        WmiPrvSE.exe    1800    604     0       0       False   0       0       0       Yes     C:\Windows\system32\wbem\wmiprvse.exe
* 0xfa801b112060        WmiPrvSE.exe    2136    604     0       0       False   0       0       0       Yes     C:\Windows\system32\wbem\wmiprvse.exe
0xfa801b112060  WmiPrvSE.exe    2136    604     0       0       False   2       2       0       N/A     (Original Process)
* 0xfa8019124b30        WmiPrvSE.exe    1800    604     0       0       False   0       0       0       Yes     C:\Windows\system32\wbem\wmiprvse.exe
* 0xfa801b112060        WmiPrvSE.exe    2136    604     0       0       False   0       0       0       Yes     C:\Windows\system32\wbem\wmiprvse.exe
0xfa801b5cb740  LunarMS.exe     708     2728    1       1       True    1       1       0       N/A     (Original Process)
* 0xfa801b5cb740        LunarMS.exe     708     2728    1       0       True    0       0       0       Yes     C:\Nexon\MapleStory\LunarMS.exe
0xfa801a4f7b30  chrome.exe      1808    4076    1       1       False   1       1       0       N/A     (Original Process)
* 0xfa801a4f7b30        chrome.exe      1808    4076    1       0       False   0       0       0       Yes     C:\Program Files (x86)\Google\Chrome\Application\chrome.exe
0xfa801aa00a90  chrome.exe      3924    4076    1       1       False   1       1       0       N/A     (Original Process)
* 0xfa801aa00a90        chrome.exe      3924    4076    1       0       False   0       0       0       Yes     C:\Program Files (x86)\Google\Chrome\Application\chrome.exe
0xfa801a7f98f0  chrome.exe      2748    4076    1       1       False   1       1       0       N/A     (Original Process)
* 0xfa801a7f98f0        chrome.exe      2748    4076    1       0       False   0       0       0       Yes     C:\Program Files (x86)\Google\Chrome\Application\chrome.exe
0xfa801b486b30  Rick And Morty  3820    2728    1       1       True    3       2       0       N/A     (Original Process)
* 0xfa801b486b30        Rick And Morty  3820    2728    1       0       True    0       0       0       Yes     C:\Torrents\Rick And Morty season 1 download.exe
* 0xfa801a4c5b30        vmware-tray.ex  3720    3820    1       0       True    0       0       0       Yes     C:\Users\Rick\AppData\Local\Temp\RarSFX0\vmware-tray.exe
0xfa801a4c5b30  vmware-tray.ex  3720    3820    1       1       True    3       2       0       N/A     (Original Process)
* 0xfa801b486b30        Rick And Morty  3820    2728    1       0       True    0       0       0       Yes     C:\Torrents\Rick And Morty season 1 download.exe
* 0xfa801a4c5b30        vmware-tray.ex  3720    3820    1       0       True    0       0       0       Yes     C:\Users\Rick\AppData\Local\Temp\RarSFX0\vmware-tray.exe
0xfa801a635240  chrome.exe      3648    4076    1       1       False   1       1       0       N/A     (Original Process)
* 0xfa801a635240        chrome.exe      3648    4076    1       0       False   0       0       0       Yes     C:\Program Files (x86)\Google\Chrome\Application\chrome.exe
0xfa801a5ef1f0  chrome.exe      1796    4076    1       1       False   1       1       0       N/A     (Original Process)
* 0xfa801a5ef1f0        chrome.exe      1796    4076    1       0       False   0       0       0       Yes     C:\Program Files (x86)\Google\Chrome\Application\chrome.exe
```
