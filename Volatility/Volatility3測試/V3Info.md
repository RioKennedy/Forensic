## 測試內容
 - .\vol.exe -f .\OtterCTF.vmem windows.info.Info

```
D:\Forensic\G140A006\VolatilityWorkbench>.\vol.exe -f .\OtterCTF.vmem windows.info.Info
Volatility 3 Framework 2.5.0
Progress:  100.00               PDB scanning finished
Variable        Value

Kernel Base     0xf80002a52000
DTB     0x187000
Symbols file:///D:/Forensic/G140A006/VolatilityWorkbench/symbols/windows/ntkrnlmp.pdb/3844DBB920174967BE7AA4A2C20430FA-2.json.xz
Is64Bit True
IsPAE   False
layer_name      0 WindowsIntel32e
memory_layer    1 FileLayer
KdDebuggerDataBlock     0xf80002c430a0
NTBuildLab      7601.17514.amd64fre.win7sp1_rtm.
CSDVersion      1
KdVersionBlock  0xf80002c43068
Major/Minor     15.7601
MachineType     34404
KeNumberProcessors      2
SystemTime      2018-08-04 19:34:22
NtSystemRoot    C:\Windows
NtProductType   NtProductWinNt
NtMajorVersion  6
NtMinorVersion  1
PE MajorOperatingSystemVersion  6
PE MinorOperatingSystemVersion  1
PE Machine      34404
PE TimeDateStamp        Sat Nov 20 09:30:02 2010
```

# windows.info.Info 分析說明

## 1. 執行指令

```bash
.\vol.exe -f .\OtterCTF.vmem windows.info.Info
```

## 2. Plugin 功能說明

`windows.info.Info` 是 Volatility 3 中用來查看 Windows 記憶體映像檔基本資訊的 Plugin。

它主要可以協助分析人員確認：

* 記憶體映像檔是否能被 Volatility 正確辨識
* 作業系統版本
* Kernel Base 位址
* Symbol 檔案是否成功載入
* 系統架構是 32-bit 或 64-bit
* 記憶體映像檔擷取時的系統時間
* Windows 系統根目錄
* CPU 數量
* Windows Build 版本

在記憶體鑑識流程中，`windows.info.Info` 通常是第一個執行的 Plugin，因為它可以先確認整個記憶體檔案的基本環境是否正常。

---

## 3. 分析結果整理

| 欄位                 | 結果                                                        |
| ------------------ | --------------------------------------------------------- |
| Kernel Base        | `0xf80002a52000`                                          |
| DTB                | `0x187000`                                                |
| Symbols            | `ntkrnlmp.pdb/3844DBB920174967BE7AA4A2C20430FA-2.json.xz` |
| Is64Bit            | `True`                                                    |
| IsPAE              | `False`                                                   |
| layer_name         | `0 WindowsIntel32e`                                       |
| memory_layer       | `1 FileLayer`                                             |
| NTBuildLab         | `7601.17514.amd64fre.win7sp1_rtm.`                        |
| CSDVersion         | `1`                                                       |
| Major/Minor        | `15.7601`                                                 |
| KeNumberProcessors | `2`                                                       |
| SystemTime         | `2018-08-04 19:34:22`                                     |
| NtSystemRoot       | `C:\Windows`                                              |
| NtProductType      | `NtProductWinNt`                                          |
| NtMajorVersion     | `6`                                                       |
| NtMinorVersion     | `1`                                                       |
| PE TimeDateStamp   | `Sat Nov 20 09:30:02 2010`                                |

---

## 4. 細節欄位說明

### 4.1 Kernel Base

```text
Kernel Base     0xf80002a52000
```

`Kernel Base` 是 Windows Kernel 在記憶體中的基底位址。

在本次分析中，Kernel Base 為：

```text
0xf80002a52000
```

這代表 Windows 核心載入在記憶體中的起始位置。Volatility 需要透過這個位址來解析 Kernel 結構，例如 Process、Thread、Driver、Handle 等資料。

若 Kernel Base 無法正確辨識，可能會導致後續 Plugin 無法正常執行。

---

### 4.2 DTB

```text
DTB     0x187000
```

`DTB` 的全名是 Directory Table Base，也可以理解為記憶體分頁轉換時使用的重要位址。

在本次分析中，DTB 為：

```text
0x187000
```

DTB 主要用於虛擬位址與實體位址之間的轉換。Volatility 透過 DTB 來正確讀取不同 Process 或 Kernel 的記憶體內容。

---

### 4.3 Symbols

```text
Symbols file:///D:/Forensic/G140A006/VolatilityWorkbench/symbols/windows/ntkrnlmp.pdb/3844DBB920174967BE7AA4A2C20430FA-2.json.xz
```

`Symbols` 代表 Volatility 使用的 Windows Symbol 檔案。

本次分析使用的 Symbol 檔案為：

```text
ntkrnlmp.pdb/3844DBB920174967BE7AA4A2C20430FA-2.json.xz
```

Symbol 檔案的作用是幫助 Volatility 理解 Windows Kernel 內部資料結構，例如行程清單、模組、網路連線與 Registry 結構。

從結果來看，Volatility 已成功找到對應的 Symbol 檔案，因此後續 Windows Plugin 應該可以正常分析。

---

### 4.4 Is64Bit

```text
Is64Bit True
```

`Is64Bit` 用來判斷目標系統是否為 64 位元作業系統。

結果顯示：

```text
True
```

代表這個記憶體映像檔來自 64-bit Windows 系統。

這點很重要，因為 32-bit 與 64-bit Windows 的 Kernel 結構、記憶體位址與資料解析方式不同。

---

### 4.5 IsPAE

```text
IsPAE   False
```

`IsPAE` 表示系統是否啟用 PAE，也就是 Physical Address Extension。

本次結果為：

```text
False
```

代表此系統沒有啟用 PAE。

PAE 通常與 32-bit 系統支援較大記憶體空間有關。由於本次系統是 64-bit Windows，因此 `IsPAE` 為 False 是合理的。

---

### 4.6 layer_name

```text
layer_name      0 WindowsIntel32e
```

`layer_name` 表示 Volatility 建立的記憶體轉換層名稱。

本次結果為：

```text
WindowsIntel32e
```

`Intel32e` 代表這是 x64 架構使用的記憶體分頁模式，也符合前面 `Is64Bit=True` 的結果。

---

### 4.7 memory_layer

```text
memory_layer    1 FileLayer
```

`memory_layer` 表示 Volatility 讀取記憶體資料的來源層。

本次結果為：

```text
FileLayer
```

代表 Volatility 是直接從記憶體映像檔 `OtterCTF.vmem` 中讀取資料。

---

### 4.8 KdDebuggerDataBlock

```text
KdDebuggerDataBlock     0xf80002c430a0
```

`KdDebuggerDataBlock` 是 Windows Kernel Debugger Data Block 的位址。

它包含許多 Kernel 調試相關的重要資訊，例如已載入模組、系統資訊與 Kernel 結構位置。

Volatility 可以透過這個結構取得更多 Windows Kernel 內部資料。

---

### 4.9 NTBuildLab

```text
NTBuildLab      7601.17514.amd64fre.win7sp1_rtm.
```

`NTBuildLab` 顯示 Windows 的 Build 版本資訊。

本次結果為：

```text
7601.17514.amd64fre.win7sp1_rtm.
```

可以拆解如下：

| 內容            | 說明                              |
| ------------- | ------------------------------- |
| `7601`        | Windows 7 SP1 的 Build Number    |
| `amd64`       | 64-bit 架構                       |
| `fre`         | Free Build，也就是正式發行版             |
| `win7sp1_rtm` | Windows 7 Service Pack 1 RTM 版本 |

因此可以判斷，這份記憶體映像檔來自：

```text
Windows 7 SP1 64-bit
```

---

### 4.10 CSDVersion

```text
CSDVersion      1
```

`CSDVersion` 表示 Windows Service Pack 版本。

結果為：

```text
1
```

代表此系統安裝的是 Service Pack 1，也就是 Windows 7 SP1。

---

### 4.11 Major/Minor

```text
Major/Minor     15.7601
```

`Major/Minor` 是 Volatility 顯示的版本資訊。

其中 `7601` 對應 Windows 7 SP1 的系統版本。

這也再次驗證此記憶體映像檔是 Windows 7 Service Pack 1。

---

### 4.12 MachineType

```text
MachineType     34404
```

`MachineType` 是 PE 檔案或系統架構的機器類型代碼。

`34404` 對應的是 64-bit AMD64 架構。

因此可以判斷此記憶體檔案來自 x64 Windows 系統。

---

### 4.13 KeNumberProcessors

```text
KeNumberProcessors      2
```

`KeNumberProcessors` 表示系統中的處理器核心數量。

本次結果為：

```text
2
```

代表該系統在擷取記憶體時，有 2 個處理器核心可供 Windows 使用。

---

### 4.14 SystemTime

```text
SystemTime      2018-08-04 19:34:22
```

`SystemTime` 是記憶體映像檔中的系統時間。

本次結果為：

```text
2018-08-04 19:34:22
```

這代表記憶體擷取當下，系統時間約為 2018 年 8 月 4 日 19:34:22。

在鑑識分析中，這個時間非常重要，因為後續分析行程、網路連線、檔案與事件時，都可以用這個時間作為時間軸基準。

---

### 4.15 NtSystemRoot

```text
NtSystemRoot    C:\Windows
```

`NtSystemRoot` 表示 Windows 系統根目錄。

本次結果為：

```text
C:\Windows
```

代表作業系統安裝在 `C:\Windows` 目錄下。

這是一般 Windows 系統的預設安裝路徑。

---

### 4.16 NtProductType

```text
NtProductType   NtProductWinNt
```

`NtProductType` 表示 Windows 產品類型。

結果為：

```text
NtProductWinNt
```

代表這是一個一般 Windows 工作站版本，而不是 Windows Server。

因此可以推測此記憶體映像檔來自一般使用者電腦，而非伺服器系統。

---

### 4.17 NtMajorVersion 與 NtMinorVersion

```text
NtMajorVersion  6
NtMinorVersion  1
```

Windows 版本號 `6.1` 對應的是 Windows 7 或 Windows Server 2008 R2。

搭配前面的 `NtProductType = NtProductWinNt` 可以判斷，這不是 Server 版本，而是一般 Windows 7 工作站版本。

因此，此系統可以判斷為：

```text
Windows 7 SP1 64-bit
```

---

### 4.18 PE MajorOperatingSystemVersion 與 PE MinorOperatingSystemVersion

```text
PE MajorOperatingSystemVersion  6
PE MinorOperatingSystemVersion  1
```

這兩個欄位是從 PE Header 中取得的作業系統版本資訊。

結果為：

```text
6.1
```

同樣對應 Windows 7 / Windows Server 2008 R2。

搭配其他欄位後，可以確認此系統為 Windows 7 SP1。

---

### 4.19 PE Machine

```text
PE Machine      34404
```

`PE Machine` 表示 PE 檔案的目標處理器架構。

數值：

```text
34404
```

對應 AMD64，也就是 64-bit 架構。

這與 `Is64Bit=True` 及 `MachineType=34404` 的結果一致。

---

### 4.20 PE TimeDateStamp

```text
PE TimeDateStamp        Sat Nov 20 09:30:02 2010
```

`PE TimeDateStamp` 表示 Windows Kernel PE 檔案的時間戳記。

本次結果為：

```text
Sat Nov 20 09:30:02 2010
```

這是 Kernel 檔案建立或編譯的時間資訊，不是記憶體擷取時間。

需要注意的是：

* `SystemTime` 是記憶體擷取當下的系統時間
* `PE TimeDateStamp` 是 Kernel PE 檔案本身的時間戳記

因此兩者不能混淆。

---

## 5. 綜合判斷

根據 `windows.info.Info` 的分析結果，可以得出以下結論：

| 項目           | 判斷結果                  |
| ------------ | --------------------- |
| 作業系統         | Windows 7             |
| Service Pack | SP1                   |
| 系統架構         | 64-bit                |
| Kernel Build | 7601                  |
| 系統類型         | 一般 Windows 工作站        |
| CPU 數量       | 2                     |
| 系統根目錄        | `C:\Windows`          |
| 記憶體擷取時間      | `2018-08-04 19:34:22` |
| Symbol 載入狀態  | 成功                    |

---

## 6. 分析結論

透過 `windows.info.Info` 可以確認，`OtterCTF.vmem` 是一份來自 Windows 7 SP1 64-bit 系統的記憶體映像檔。

Volatility 成功辨識 Kernel Base、DTB、Windows Build 版本與 Symbol 檔案，代表此記憶體映像檔可以被正常解析。
