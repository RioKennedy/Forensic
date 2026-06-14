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
# windows.joblinks.JobLinks 分析

## 1. 執行指令

```bash
.\vol.exe -f .\OtterCTF.vmem windows.joblinks.JobLinks
```

---

## 2. Plugin 功能簡述

`windows.joblinks.JobLinks` 用來查看 Process 是否被放在同一個 Windows Job Object 中。

重點是確認哪些 Process 被同一組 Job 管理，常用來觀察：

* 同一程式產生的子行程群組
* 可疑程式與子行程是否被關聯在一起
* Process 是否被 Job Object 控制

---

## 3. 結果重點整理

| 原始 Process        |  PID | 關聯 Process        |  PID | 判斷               |
| ----------------- | ---: | ----------------- | ---: | ---------------- |
| `WmiPrvSE.exe`    | 1800 | `WmiPrvSE.exe`    | 2136 | WMI 相關，較偏正常      |
| `LunarMS.exe`     |  708 | `LunarMS.exe`     |  708 | 單一 Job，需搭配前面結果確認 |
| `chrome.exe`      | 1808 | `chrome.exe`      | 1808 | Chrome 子行程 Job   |
| `chrome.exe`      | 3924 | `chrome.exe`      | 3924 | Chrome 子行程 Job   |
| `chrome.exe`      | 2748 | `chrome.exe`      | 2748 | Chrome 子行程 Job   |
| `Rick And Morty`  | 3820 | `vmware-tray.exe` | 3720 | 重要可疑關聯           |
| `vmware-tray.exe` | 3720 | `Rick And Morty`  | 3820 | 重要可疑關聯           |
| `chrome.exe`      | 3648 | `chrome.exe`      | 3648 | Chrome 子行程 Job   |
| `chrome.exe`      | 1796 | `chrome.exe`      | 1796 | Chrome 子行程 Job   |

---

## 4. 關鍵發現

本次最重要的 Job 關係是：

```text
Rick And Morty → vmware-tray.exe
```

結果中顯示：

```text
Rick And Morty
PID: 3820
Path: C:\Torrents\Rick And Morty season 1 download.exe

vmware-tray.exe
PID: 3720
Path: C:\Users\Rick\AppData\Local\Temp\RarSFX0\vmware-tray.exe
```

兩者出現在同一組 Job Object 中，代表它們不只是父子關係，也被同一個 Job 管理。

這進一步補強前面的判斷：

```text
Rick And Morty season 1 download.exe 執行後，釋放或啟動了 Temp\RarSFX0\vmware-tray.exe。
```

---

## 5. 其他結果判斷

| Process                              | 判斷                                   |
| ------------------------------------ | ------------------------------------ |
| `WmiPrvSE.exe`                       | 兩個 WMI 行程在同一 Job 中，較偏正常系統行為          |
| `chrome.exe`                         | 多個 Chrome 子行程使用 Job Object，屬於正常瀏覽器架構 |
| `LunarMS.exe`                        | 單一 Job，沒有看到其他關聯 Process              |
| `Rick And Morty` / `vmware-tray.exe` | 可疑關聯，需優先分析                           |

---

## 6. 鑑識判斷

`JobLinks` 結果再次確認 `Rick And Morty` 與 `vmware-tray.exe` 的關聯。

前面已知：

```text
pstree: Rick And Morty → vmware-tray.exe
cmdline: vmware-tray.exe 位於 Temp\RarSFX0
sessions: 兩者都屬於 Rick 使用者 Session
envars: 兩者都使用 Rick 的使用者環境
joblinks: 兩者在同一個 Job Object 中
```

因此可以判斷：

```text
PID 3820 Rick And Morty 與 PID 3720 vmware-tray.exe 是同一條可疑執行鏈。
```
