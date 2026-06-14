# Volatility3

## Volatylity 3 Help
- [Help](Volatility3測試/V3Help.md)
- [NetScan](Volatility3測試/V3NetScan.md)

# Windows Volatility 3 Plugin 分類整理

> 來源：Volatility 3 Framework 2.5.0 `vol.exe -h` 輸出  
> 範圍：只整理 `windows.*` 類別 Plugin

---

## 一、系統基本資訊類

| Plugin | 功能說明 | 用途 |
|---|---|---|
| [`windows.info.Info`](Volatility3測試/V3Info.md) | 顯示記憶體映像檔的 Windows 系統與核心資訊 | 確認 OS 版本、Kernel、Symbol 是否正確 |
| [`windows.crashinfo.Crashinfo`](Volatility3測試/V3CrashInfo.md) | 顯示 Windows crash dump 資訊 | 分析當機傾印檔 |
| [`windows.statistics.Statistics`](Volatility3測試/V3Statistics.md) | 顯示記憶體空間統計資訊 | 初步了解記憶體結構 |
| [`windows.memmap.Memmap`](Volatility3測試/V3Memmap.md) | 顯示記憶體映射 | 查看虛擬記憶體對應情況 |
| [`windows.virtmap.VirtMap`](Volatility3測試/V3Virtmap.md) | 顯示虛擬記憶體映射區段 | 輔助分析記憶體位址 |

---

## 二、Process 行程分析類

| Plugin | 功能說明 | 用途 |
|---|---|---|
| [`windows.pslist.PsList`](Volatility3測試/V3Pslist.md) | 列出目前記憶體中的行程 | 基本行程清單 |
| [`windows.psscan.PsScan`](Volatility3測試/V3Psscan.md) | 掃描隱藏或已結束的行程 | 找可疑或隱藏行程 |
| [`windows.pstree.PsTree`](Volatility3測試/V3Pstree.md) | 用樹狀結構顯示父子行程關係 | 看行程是否正常由誰啟動 |
| [`windows.cmdline.CmdLine`](Volatility3測試/V3Cmdline.md) | 顯示行程執行命令列 | 找可疑參數、惡意程式執行路徑 |
| [`windows.envars.Envars`](Volatility3測試/V3Envars.md) | 顯示行程環境變數 | 查看使用者、路徑、執行環境 |
| [`windows.sessions.Sessions`](Volatility3測試/V3Sessions.md) | 顯示 Session 資訊 | 判斷行程屬於哪個登入階段 |
| [`windows.joblinks.JobLinks`](Volatility3測試/V3Joblinks.md) | 顯示行程 Job link 資訊 | 分析行程群組關係 |

### 常用指令

```bash
vol.exe -f memory.vmem windows.pslist.PsList
vol.exe -f memory.vmem windows.pstree.PsTree
vol.exe -f memory.vmem windows.psscan.PsScan
vol.exe -f memory.vmem windows.cmdline.CmdLine
```

---

## 三、DLL / 模組 / 程式載入分析類

| Plugin | 功能說明 | 用途 |
|---|---|---|
| [`windows.dlllist.DllList`](Volatility3測試/V3Pslist.md) | 列出行程載入的 DLL | 查看行程載入哪些模組 |
| [`windows.ldrmodules.LdrModules`](Volatility3測試/V3Pslist.md) | 比對載入模組資訊 | 找 DLL Injection、Unlinked DLL |
| [`windows.verinfo.VerInfo`](Volatility3測試/V3Pslist.md) | 顯示 PE 檔版本資訊 | 判斷檔案公司、版本、可疑 PE |
| [`windows.modules.Modules`](Volatility3測試/V3Pslist.md) | 列出 Kernel module | 查看核心模組 |
| [`windows.modscan.ModScan`](Volatility3測試/V3Pslist.md) | 掃描記憶體中的模組 | 找隱藏 Kernel module |

### 常用指令

```bash
vol.exe -f memory.vmem windows.dlllist.DllList --pid <PID>
vol.exe -f memory.vmem windows.ldrmodules.LdrModules --pid <PID>
vol.exe -f memory.vmem windows.verinfo.VerInfo
```

---

## 四、網路連線分析類

| Plugin | 功能說明 | 用途 |
|---|---|---|
| [`windows.netscan.NetScan`](Volatility3測試/V3NetScan.md) | 掃描 Windows 網路連線物件 | 找 TCP/UDP 連線、可疑連外 |
| [`windows.netstat.NetStat`](Volatility3測試/V3NetStat.md) | 透過網路追蹤結構列出連線 | 類似 netstat 的效果 |

### 常用指令

```bash
vol.exe -f memory.vmem windows.netscan.NetScan
vol.exe -f memory.vmem windows.netstat.NetStat
```

### 可觀察重點

- 可疑遠端 IP
- 可疑連外連線
- 哪個 PID 建立連線
- Port 是否異常

---

## 五、檔案與檔案系統分析類

| Plugin | 功能說明 | 用途 |
|---|---|---|
| `windows.filescan.FileScan` | 掃描記憶體中的 File Object | 找開啟過或殘留的檔案 |
| `windows.dumpfiles.DumpFiles` | Dump 記憶體中的快取檔案 | 把可疑檔案匯出 |
| `windows.mftscan.MFTScan` | 掃描 MFT FILE objects | NTFS / MFT 鑑識分析 |
| `windows.mbrscan.MBRScan` | 掃描並解析 MBR | 找 Bootkit、MBR 感染 |
| `windows.symlinkscan.SymlinkScan` | 掃描 Symbolic Link | 分析連結物件 |

### 與 NTFS 鑑識相關

```bash
vol.exe -f memory.vmem windows.mftscan.MFTScan
vol.exe -f memory.vmem windows.filescan.FileScan
vol.exe -f memory.vmem windows.dumpfiles.DumpFiles
```

---

## 六、Registry 登錄檔分析類

| Plugin | 功能說明 | 用途 |
|---|---|---|
| `windows.registry.hivelist.HiveList` | 列出 Registry hive | 找 SYSTEM、SOFTWARE、SAM、NTUSER.DAT |
| `windows.registry.hivescan.HiveScan` | 掃描 Registry hive | 找隱藏或殘留的 hive |
| `windows.registry.printkey.PrintKey` | 顯示指定 Registry key | 查看登錄鍵內容 |
| `windows.registry.userassist.UserAssist` | 顯示 UserAssist 執行紀錄 | 分析使用者執行過哪些程式 |
| `windows.registry.certificates.Certificates` | 顯示憑證儲存區 | 查看系統憑證 |

### 報告寫法範例

Registry 類 Plugin 主要用於分析 Windows 登錄檔，例如系統設定、使用者活動紀錄、程式執行紀錄與憑證資訊。其中 `UserAssist` 可以協助判斷使用者是否曾經執行特定程式。

---

## 七、惡意程式 / Injection / Rootkit 偵測類

| Plugin | 功能說明 | 用途 |
|---|---|---|
| `windows.malfind.Malfind` | 找可能被注入惡意程式碼的記憶體區段 | 偵測 Process Injection |
| `windows.vadinfo.VadInfo` | 顯示行程 VAD 記憶體區段 | 查看行程記憶體分配 |
| `windows.vadwalk.VadWalk` | 走訪 VAD Tree | 深入分析行程記憶體 |
| `windows.vadyarascan.VadYaraScan` | 用 YARA 掃描 VAD 區段 | 用規則找惡意特徵 |
| `windows.skeleton_key_check.Skeleton_Key_Check` | 檢查 Skeleton Key malware | 偵測特定惡意攻擊 |
| `windows.callbacks.Callbacks` | 列出 Kernel callbacks | 找 Rootkit callback hook |
| `windows.ssdt.SSDT` | 顯示 System Service Dispatch Table | 找 SSDT Hook |
| `windows.driverirp.DriverIrp` | 顯示 Driver IRP | 找 Driver hook |
| `windows.drivermodule.DriverModule` | 偵測隱藏 Driver | Rootkit 分析 |
| `windows.driverscan.DriverScan` | 掃描 Driver | 找隱藏或殘留 Driver |

### 常用指令

```bash
vol.exe -f memory.vmem windows.malfind.Malfind --pid <PID>
vol.exe -f memory.vmem windows.vadinfo.VadInfo --pid <PID>
vol.exe -f memory.vmem windows.ldrmodules.LdrModules --pid <PID>
vol.exe -f memory.vmem windows.callbacks.Callbacks
vol.exe -f memory.vmem windows.ssdt.SSDT
```

---

## 八、Handle / Mutex / 權限 / SID 分析類

| Plugin | 功能說明 | 用途 |
|---|---|---|
| `windows.handles.Handles` | 顯示行程開啟的 Handle | 看行程開啟了哪些檔案、Registry、Mutex |
| `windows.mutantscan.MutantScan` | 掃描 Mutex / Mutant | 找惡意程式常用 Mutex |
| `windows.privileges.Privs` | 顯示行程 Token 權限 | 看是否有 Debug、SeImpersonate 等高風險權限 |
| `windows.getsids.GetSIDs` | 顯示行程擁有者 SID | 判斷行程使用者身分 |
| `windows.getservicesids.GetServiceSIDs` | 顯示服務 SID | 服務身分分析 |

---

## 九、帳號密碼 / Credential 分析類

| Plugin | 功能說明 | 用途 |
|---|---|---|
| `windows.hashdump.Hashdump` | Dump 使用者 Hash | 分析本機帳號密碼雜湊 |
| `windows.cachedump.Cachedump` | Dump cached logon secrets | 取得快取登入資訊 |
| `windows.lsadump.Lsadump` | Dump LSA secrets | 分析 LSA 機密資料 |

### 報告寫法範例

Credential 類 Plugin 可用於分析 Windows 記憶體中的認證資訊，例如使用者雜湊、快取登入資料與 LSA Secrets，常用於事件調查中確認帳號是否遭竊用。

---

## 十、Service / Device / Driver 分析類

| Plugin | 功能說明 | 用途 |
|---|---|---|
| `windows.svcscan.SvcScan` | 掃描 Windows services | 找可疑服務 |
| `windows.devicetree.DeviceTree` | 顯示 Driver 與 Device Tree | 分析裝置與驅動關係 |
| `windows.driverirp.DriverIrp` | 顯示 Driver IRP | 偵測 Driver Hook |
| `windows.driverscan.DriverScan` | 掃描 Driver | 找隱藏 Driver |
| `windows.drivermodule.DriverModule` | 偵測隱藏 Driver | Rootkit 分析 |
| `windows.modules.Modules` | 列出 Kernel modules | 查看核心模組 |

---

## 十一、Pool / Memory Object 掃描類

| Plugin | 功能說明 | 用途 |
|---|---|---|
| `windows.bigpools.BigPools` | 列出 Big Page Pools | Kernel memory pool 分析 |
| `windows.poolscanner.PoolScanner` | 通用 Pool 掃描器 | 掃描 Windows pool object |
| `windows.filescan.FileScan` | 掃描 File Object | 找檔案物件 |
| `windows.mutantscan.MutantScan` | 掃描 Mutant / Mutex | 找同步物件 |
| `windows.mbrscan.MBRScan` | 掃描 MBR | Boot record 分析 |

---

# Windows Memory Forensics 基本分析流程

```text
系統資訊
    ↓
行程分析
    ↓
命令列分析
    ↓
網路連線分析
    ↓
DLL / 模組分析
    ↓
惡意注入偵測
    ↓
檔案跡證分析
    ↓
Registry 使用者活動分析
    ↓
整理證據與報告
```

---

# 簡短總結

Windows 類 Volatility Plugin 可以依照鑑識目的分成：

1. 系統資訊分析
2. 行程分析
3. 網路連線分析
4. DLL 與模組分析
5. 檔案與 NTFS 分析
6. Registry 分析
7. 惡意程式與 Injection 偵測
8. Rootkit / Driver 偵測
9. 帳號與權限分析
10. Service / Handle / Object 分析

其中最適合初學與報告實作的流程是：

```text
info → pslist / pstree / psscan → cmdline → netscan → dlllist → malfind → filescan → registry
```
