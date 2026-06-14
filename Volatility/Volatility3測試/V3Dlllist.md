# 測試內容
- vol.exe -f .\OtterCTF.vmem windows.dlllist.DllList --pid 3820
```
D:\Forensic\G140A006\VolatilityWorkbench>.\vol.exe -f .\OtterCTF.vmem windows.dlllist.DllList --pid 3820
Volatility 3 Framework 2.5.0
Progress:  100.00               PDB scanning finished
PID     Process Base    Size    Name    Path    LoadTime        File output

3820    Rick And Morty  0x400000        0x56000 Rick And Morty season 1 download.exe    C:\Torrents\Rick And Morty season 1 download.exe        N/A     Disabled
3820    Rick And Morty  0x776f0000      0x1a9000        ntdll.dll       C:\Windows\SYSTEM32\ntdll.dll   N/A     Disabled
3820    Rick And Morty  0x75210000      0x3f000 wow64.dll       C:\Windows\SYSTEM32\wow64.dll   2018-08-04 19:32:55.000000      Disabled
3820    Rick And Morty  0x751b0000      0x5c000 wow64win.dll    C:\Windows\SYSTEM32\wow64win.dll        2018-08-04 19:32:55.000000      Disabled
3820    Rick And Morty  0x751a0000      0x8000  wow64cpu.dll    C:\Windows\SYSTEM32\wow64cpu.dll        2018-08-04 19:32:55.000000      Disabled
```

- vol.exe -f .\OtterCTF.vmem windows.dlllist.DllList --pid 3720
```
D:\Forensic\G140A006\VolatilityWorkbench>.\vol.exe -f .\OtterCTF.vmem windows.dlllist.DllList --pid 3720
Volatility 3 Framework 2.5.0
Progress:  100.00               PDB scanning finished
PID     Process Base    Size    Name    Path    LoadTime        File output

3720    vmware-tray.ex  0xec0000        0x6e000 vmware-tray.exe C:\Users\Rick\AppData\Local\Temp\RarSFX0\vmware-tray.exeN/A     Disabled
3720    vmware-tray.ex  0x776f0000      0x1a9000        ntdll.dll       C:\Windows\SYSTEM32\ntdll.dll   N/A     Disabled
3720    vmware-tray.ex  0x75210000      0x3f000 wow64.dll       C:\Windows\SYSTEM32\wow64.dll   2018-08-04 19:33:03.000000      Disabled
3720    vmware-tray.ex  0x751b0000      0x5c000 wow64win.dll    C:\Windows\SYSTEM32\wow64win.dll        2018-08-04 19:33:03.000000      Disabled
3720    vmware-tray.ex  0x751a0000      0x8000  wow64cpu.dll    C:\Windows\SYSTEM32\wow64cpu.dll        2018-08-04 19:33:03.000000      Disabled
```

- vol.exe -f .\OtterCTF.vmem windows.dlllist.DllList --pid 708
```
D:\Forensic\G140A006\VolatilityWorkbench>.\vol.exe -f .\OtterCTF.vmem windows.dlllist.DllList --pid 708
Volatility 3 Framework 2.5.0
Progress:  100.00               PDB scanning finished
PID     Process Base    Size    Name    Path    LoadTime        File output

708     LunarMS.exe     0x400000        0xa95000        LunarMS.exe     C:\Nexon\MapleStory\LunarMS.exe  N/A     Disabled
708     LunarMS.exe     0x776f0000      0x1a9000        ntdll.dll       C:\Windows\SYSTEM32\ntdll.dll    N/A     Disabled
708     LunarMS.exe     0x75210000      0x3f000 wow64.dll       C:\Windows\SYSTEM32\wow64.dll   2018-08-04 19:27:39.000000       Disabled
708     LunarMS.exe     0x751b0000      0x5c000 wow64win.dll    C:\Windows\SYSTEM32\wow64win.dll2018-08-04 19:27:39.000000       Disabled
708     LunarMS.exe     0x751a0000      0x8000  wow64cpu.dll    C:\Windows\SYSTEM32\wow64cpu.dll2018-08-04 19:27:39.000000       Disabled
```

- vol.exe -f .\OtterCTF.vmem windows.dlllist.DllList --pid 3880
```
D:\Forensic\G140A006\VolatilityWorkbench>.\vol.exe -f .\OtterCTF.vmem windows.dlllist.DllList --pid 3880
Volatility 3 Framework 2.5.0
Progress:  100.00               PDB scanning finished
PID     Process Base    Size    Name    Path    LoadTime        File output

3880    WebCompanionIn  0x300000        0x52000 WebCompanionInstaller.exe       C:\Program Files (x86)\Lavasoft\Web Companion\Application\WebCompanionInstaller.exe      N/A     Disabled
3880    WebCompanionIn  0x776f0000      0x1a9000        ntdll.dll       C:\Windows\SYSTEM32\ntdll.dll    N/A     Disabled
3880    WebCompanionIn  0x75210000      0x3f000 wow64.dll       C:\Windows\SYSTEM32\wow64.dll   2018-08-04 19:33:07.000000       Disabled
3880    WebCompanionIn  0x751b0000      0x5c000 wow64win.dll    C:\Windows\SYSTEM32\wow64win.dll2018-08-04 19:33:07.000000       Disabled
3880    WebCompanionIn  0x751a0000      0x8000  wow64cpu.dll    C:\Windows\SYSTEM32\wow64cpu.dll2018-08-04 19:33:07.000000       Disabled
```

- vol.exe -f .\OtterCTF.vmem windows.dlllist.DllList --pid 3856
```
D:\Forensic\G140A006\VolatilityWorkbench>.\vol.exe -f .\OtterCTF.vmem windows.dlllist.DllList --pid 3856
Volatility 3 Framework 2.5.0
Progress:  100.00               PDB scanning finished
PID     Process Base    Size    Name    Path    LoadTime        File output

3856    WebCompanion.e  0xf90000        0x70a000        WebCompanion.exe        C:\Program Files (x86)\Lavasoft\Web Companion\Application\WebCompanion.exe       N/A     Disabled
3856    WebCompanion.e  0x776f0000      0x1a9000        ntdll.dll       C:\Windows\SYSTEM32\ntdll.dll    N/A     Disabled
3856    WebCompanion.e  0x75210000      0x3f000 wow64.dll       C:\Windows\SYSTEM32\wow64.dll   2018-08-04 19:34:05.000000       Disabled
3856    WebCompanion.e  0x751b0000      0x5c000 wow64win.dll    C:\Windows\SYSTEM32\wow64win.dll2018-08-04 19:34:05.000000       Disabled
3856    WebCompanion.e  0x751a0000      0x8000  wow64cpu.dll    C:\Windows\SYSTEM32\wow64cpu.dll2018-08-04 19:34:05.000000       Disabled
```


# windows.dlllist.DllList 分析

## 1. 執行指令

```bash
.\vol.exe -f .\OtterCTF.vmem windows.dlllist.DllList --pid 3820
.\vol.exe -f .\OtterCTF.vmem windows.dlllist.DllList --pid 3720
.\vol.exe -f .\OtterCTF.vmem windows.dlllist.DllList --pid 708
.\vol.exe -f .\OtterCTF.vmem windows.dlllist.DllList --pid 3880
.\vol.exe -f .\OtterCTF.vmem windows.dlllist.DllList --pid 3856
```

---

## 2. Plugin 功能簡述

`windows.dlllist.DllList` 用來查看指定 Process 載入的 EXE 與 DLL 模組。

本次主要用來確認可疑 Process 的：

* 主程式路徑
* 是否為 32-bit 程式
* 是否載入可疑 DLL
* 是否與前面 `cmdline`、`pstree` 結果一致

---

## 3. 結果重點整理

|  PID | Process                     | 主要模組路徑                                                                                | 判斷                 |
| ---: | --------------------------- | ------------------------------------------------------------------------------------- | ------------------ |
| 3820 | `Rick And Morty`            | `C:\Torrents\Rick And Morty season 1 download.exe`                                    | 高度可疑               |
| 3720 | `vmware-tray.exe`           | `C:\Users\Rick\AppData\Local\Temp\RarSFX0\vmware-tray.exe`                            | 可疑子行程              |
|  708 | `LunarMS.exe`               | `C:\Nexon\MapleStory\LunarMS.exe`                                                     | 遊戲相關程式             |
| 3880 | `WebCompanionInstaller.exe` | `C:\Program Files (x86)\Lavasoft\Web Companion\Application\WebCompanionInstaller.exe` | WebCompanion 安裝/更新 |
| 3856 | `WebCompanion.exe`          | `C:\Program Files (x86)\Lavasoft\Web Companion\Application\WebCompanion.exe`          | WebCompanion 程式    |

---

## 4. 關鍵發現

### 4.1 Rick And Morty

```text
PID: 3820
Process: Rick And Morty
Path: C:\Torrents\Rick And Morty season 1 download.exe
```

重點：

* 主程式名稱偽裝成影片下載
* 實際上是 `.exe`
* 路徑位於 `C:\Torrents`
* 與 BitTorrent 下載活動相符

判斷：

```text
Rick And Morty season 1 download.exe 是本次最重要的可疑執行檔。
```

---

### 4.2 vmware-tray.exe

```text
PID: 3720
Process: vmware-tray.exe
Path: C:\Users\Rick\AppData\Local\Temp\RarSFX0\vmware-tray.exe
```

重點：

* 從 `Temp\RarSFX0` 執行
* 不在正常 VMware 安裝路徑
* 是 `Rick And Morty` 的子行程
* 與 `Rick And Morty` 位於同一條可疑執行鏈

判斷：

```text
vmware-tray.exe 很可能是可疑程式釋放出的子程式。
```

---

### 4.3 LunarMS.exe

```text
PID: 708
Process: LunarMS.exe
Path: C:\Nexon\MapleStory\LunarMS.exe
```

重點：

* 位於 MapleStory 相關目錄
* 沒有看到明顯可疑 DLL
* 仍建議搭配 `malfind` 確認是否有注入

判斷：

```text
LunarMS.exe 目前較像遊戲相關程式，優先度低於 Rick And Morty 與 vmware-tray.exe。
```

---

### 4.4 WebCompanion 相關程式

```text
PID 3880: WebCompanionInstaller.exe
PID 3856: WebCompanion.exe
```

路徑皆位於：

```text
C:\Program Files (x86)\Lavasoft\Web Companion\Application\
```

重點：

* 路徑與 WebCompanion 相符
* 前面曾觀察到 `WebCompanionIn → sc.exe`
* 可能涉及安裝、更新或服務操作

判斷：

```text
WebCompanion 相關行為需搭配 svcscan 確認服務操作內容。
```

---

## 5. DLL 載入狀況

這幾個 Process 都載入了：

```text
ntdll.dll
wow64.dll
wow64win.dll
wow64cpu.dll
```

這代表它們是 32-bit 程式在 64-bit Windows 上執行。

其中 `wow64.dll`、`wow64win.dll`、`wow64cpu.dll` 屬於正常 Windows WoW64 相關 DLL，本身不代表惡意。

---

## 6. 鑑識判斷

本次 `dlllist` 沒有看到明顯陌生或異常 DLL。

但它確認了兩個重要事實：

```text
Rick And Morty 的真實路徑：
C:\Torrents\Rick And Morty season 1 download.exe
```

```text
vmware-tray.exe 的真實路徑：
C:\Users\Rick\AppData\Local\Temp\RarSFX0\vmware-tray.exe
```

這兩個路徑與前面的 `cmdline`、`pstree`、`sessions`、`joblinks` 結果一致。

因此，`dlllist` 的重點不是發現惡意 DLL，而是確認可疑執行檔與其子行程的載入路徑。
