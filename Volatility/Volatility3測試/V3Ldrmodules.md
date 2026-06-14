# 測試內容

- vol.exe -f .\OtterCTF.vmem windows.ldrmodules.LdrModules --pid  3820
```
D:\Forensic\G140A006\VolatilityWorkbench>.\vol.exe -f .\OtterCTF.vmem windows.ldrmodules.LdrModules --pid 3820
Volatility 3 Framework 2.5.0
Progress:  100.00               PDB scanning finished
Pid     Process Base    InLoad  InInit  InMem   MappedPath

3820    Rick And Morty  0x400000        True    False   True    \Torrents\Rick And Morty season 1 download.exe
3820    Rick And Morty  0x240000        False   False   False   \Windows\SysWOW64\en-US\user32.dll.mui
3820    Rick And Morty  0x530000        False   False   False   \Windows\SysWOW64\en-US\propsys.dll.mui
3820    Rick And Morty  0x75210000      True    True    True    \Windows\System32\wow64.dll
3820    Rick And Morty  0x6c2d0000      False   False   False   \Windows\SysWOW64\mpr.dll
3820    Rick And Morty  0x2f80000       False   False   False   \Windows\SysWOW64\en-US\urlmon.dll.mui
3820    Rick And Morty  0x2fa0000       False   False   False   \Windows\SysWOW64\en-US\setupapi.dll.mui
3820    Rick And Morty  0x68770000      False   False   False   \Windows\SysWOW64\riched20.dll
3820    Rick And Morty  0x68870000      False   False   False   \Program Files (x86)\Common Files\microsoft shared\ink\tiptsf.dll
3820    Rick And Morty  0x68950000      False   False   False   \Windows\SysWOW64\shdocvw.dll
3820    Rick And Morty  0x73da0000      False   False   False   \Windows\SysWOW64\riched32.dll
3820    Rick And Morty  0x72ce0000      False   False   False   \Windows\SysWOW64\apphelp.dll
3820    Rick And Morty  0x6c350000      False   False   False   \Windows\AppPatch\AcLayers.dll
3820    Rick And Morty  0x6c2f0000      False   False   False   \Windows\SysWOW64\winspool.drv
3820    Rick And Morty  0x72080000      False   False   False   \Windows\SysWOW64\propsys.dll
3820    Rick And Morty  0x73c90000      False   False   False   \Windows\SysWOW64\ntmarta.dll
3820    Rick And Morty  0x73c70000      False   False   False   \Windows\SysWOW64\dwmapi.dll
3820    Rick And Morty  0x73ce0000      False   False   False   \Windows\SysWOW64\userenv.dll
3820    Rick And Morty  0x75000000      False   False   False   \Windows\winsxs\x86_microsoft.windows.common-controls_6595b64144ccf1df_6.0.7601.17514_none_41e6975e2bd6f2b2\comctl32.dll
3820    Rick And Morty  0x741a0000      False   False   False   \Windows\SysWOW64\profapi.dll
3820    Rick And Morty  0x74120000      False   False   False   \Windows\SysWOW64\uxtheme.dll
3820    Rick And Morty  0x74820000      False   False   False   \Windows\SysWOW64\version.dll
3820    Rick And Morty  0x751a0000      True    True    True    \Windows\System32\wow64cpu.dll
3820    Rick And Morty  0x751b0000      True    True    True    \Windows\System32\wow64win.dll
3820    Rick And Morty  0x76160000      False   False   False   \Windows\SysWOW64\msvcrt.dll
3820    Rick And Morty  0x75ad0000      False   False   False   \Windows\SysWOW64\usp10.dll
3820    Rick And Morty  0x756c0000      False   False   False   \Windows\SysWOW64\oleaut32.dll
3820    Rick And Morty  0x754b0000      False   False   False   \Windows\SysWOW64\rpcrt4.dll
3820    Rick And Morty  0x75430000      False   False   False   \Windows\SysWOW64\sspicli.dll
3820    Rick And Morty  0x75420000      False   False   False   \Windows\SysWOW64\cryptbase.dll
3820    Rick And Morty  0x75490000      False   False   False   \Windows\SysWOW64\devobj.dll
3820    Rick And Morty  0x755e0000      False   False   False   \Windows\SysWOW64\advapi32.dll
3820    Rick And Morty  0x75680000      False   False   False   \Windows\SysWOW64\cfgmgr32.dll
3820    Rick And Morty  0x757d0000      False   False   False   \Windows\SysWOW64\lpk.dll
3820    Rick And Morty  0x75750000      False   False   False   \Windows\SysWOW64\Wldap32.dll
3820    Rick And Morty  0x757e0000      False   False   False   \Windows\SysWOW64\wininet.dll
3820    Rick And Morty  0x759b0000      False   False   False   \Windows\SysWOW64\crypt32.dll
3820    Rick And Morty  0x75d30000      False   False   False   \Windows\SysWOW64\KernelBase.dll
3820    Rick And Morty  0x75b70000      False   False   False   \Windows\SysWOW64\comdlg32.dll
3820    Rick And Morty  0x75bf0000      False   False   False   \Windows\SysWOW64\urlmon.dll
3820    Rick And Morty  0x75de0000      False   False   False   \Windows\SysWOW64\sechost.dll
3820    Rick And Morty  0x75d80000      False   False   False   \Windows\SysWOW64\imm32.dll
3820    Rick And Morty  0x76000000      False   False   False   \Windows\SysWOW64\ole32.dll
3820    Rick And Morty  0x75e00000      False   False   False   \Windows\SysWOW64\iertutil.dll
3820    Rick And Morty  0x772f0000      False   False   False   \Windows\SysWOW64\kernel32.dll
3820    Rick And Morty  0x76f00000      False   False   False   \Windows\SysWOW64\user32.dll
3820    Rick And Morty  0x76e70000      False   False   False   \Windows\SysWOW64\gdi32.dll
3820    Rick And Morty  0x76220000      False   False   False   \Windows\SysWOW64\shell32.dll
3820    Rick And Morty  0x77200000      False   False   False   \Windows\SysWOW64\shlwapi.dll
3820    Rick And Morty  0x77060000      False   False   False   \Windows\SysWOW64\setupapi.dll
3820    Rick And Morty  0x77260000      False   False   False   \Windows\SysWOW64\clbcatq.dll
3820    Rick And Morty  0x776f0000      True    True    True    \Windows\System32\ntdll.dll
3820    Rick And Morty  0x77400000      False   False   False   \Windows\SysWOW64\msctf.dll
3820    Rick And Morty  0x778d0000      False   False   False   \Windows\SysWOW64\ntdll.dll
3820    Rick And Morty  0x778a0000      False   False   False   \Windows\SysWOW64\msasn1.dll
```

- vol.exe -f .\OtterCTF.vmem windows.ldrmodules.LdrModules --pid  3720
```
D:\Forensic\G140A006\VolatilityWorkbench>.\vol.exe -f .\OtterCTF.vmem windows.ldrmodules.LdrModules --pid 3720
Volatility 3 Framework 2.5.0
Progress:  100.00               PDB scanning finished
Pid     Process Base    InLoad  InInit  InMem   MappedPath

3720    vmware-tray.ex  0xec0000        True    False   True    \Users\Rick\AppData\Local\Temp\RarSFX0\vmware-tray.exe
3720    vmware-tray.ex  0xd90000        False   False   False   \Windows\Microsoft.NET\Framework\v4.0.30319\mscorrc.dll
3720    vmware-tray.ex  0x74a00000      False   False   False   \Windows\Microsoft.NET\Framework\v4.0.30319\mscoreei.dll
3720    vmware-tray.ex  0x66660000      False   False   False   \Windows\assembly\NativeImages_v4.0.30319_32\System.Drawing\dd57bc19f5807c6dbe8f88d4a23277f6\System.Drawing.ni.dll
3720    vmware-tray.ex  0x65330000      False   False   False   \Windows\assembly\NativeImages_v4.0.30319_32\System.Core\713647b987b140a17e3c4ffe4c721f85\System.Core.ni.dll
3720    vmware-tray.ex  0x659f0000      False   False   False   \Windows\assembly\NativeImages_v4.0.30319_32\System.Windows.Forms\17e020ae92d7fab33bcc1c98b25019d0\System.Windows.Forms.ni.dll
3720    vmware-tray.ex  0x69720000      False   False   False   \Windows\SysWOW64\msvcr100_clr0400.dll
3720    vmware-tray.ex  0x68070000      False   False   False   \Windows\Microsoft.NET\Framework\v4.0.30319\clr.dll
3720    vmware-tray.ex  0x670a0000      False   False   False   \Windows\assembly\NativeImages_v4.0.30319_32\mscorlib\246f1a5abb686b9dcdf22d3505b08cea\mscorlib.ni.dll
3720    vmware-tray.ex  0x66800000      False   False   False   \Windows\assembly\NativeImages_v4.0.30319_32\System\964da027ebca3b263a05cadb8eaa20a3\System.ni.dll
3720    vmware-tray.ex  0x68010000      False   False   False   \Windows\Microsoft.NET\Framework\v4.0.30319\clrjit.dll
3720    vmware-tray.ex  0x68860000      False   False   False   \Windows\Microsoft.NET\Framework\v4.0.30319\nlssorting.dll
3720    vmware-tray.ex  0x73fe0000      False   False   False   \Windows\winsxs\x86_microsoft.windows.common-controls_6595b64144ccf1df_5.82.7601.17514_none_ec83dffa859149af\comctl32.dll
3720    vmware-tray.ex  0x73c70000      False   False   False   \Windows\SysWOW64\dwmapi.dll
3720    vmware-tray.ex  0x71990000      False   False   False   \Windows\SysWOW64\WindowsCodecs.dll
3720    vmware-tray.ex  0x73f60000      False   False   False   \Windows\SysWOW64\bcrypt.dll
3720    vmware-tray.ex  0x741a0000      False   False   False   \Windows\SysWOW64\profapi.dll
3720    vmware-tray.ex  0x74100000      False   False   False   \Windows\SysWOW64\cryptsp.dll
3720    vmware-tray.ex  0x740c0000      False   False   False   \Windows\SysWOW64\rsaenh.dll
3720    vmware-tray.ex  0x74120000      False   False   False   \Windows\SysWOW64\uxtheme.dll
3720    vmware-tray.ex  0x74870000      False   False   False   \Windows\winsxs\x86_microsoft.windows.gdiplus_6595b64144ccf1df_1.1.7601.17514_none_72d18a4386696c80\GdiPlus.dll
3720    vmware-tray.ex  0x754b0000      False   False   False   \Windows\SysWOW64\rpcrt4.dll
3720    vmware-tray.ex  0x75210000      True    True    True    \Windows\System32\wow64.dll
3720    vmware-tray.ex  0x751a0000      True    True    True    \Windows\System32\wow64cpu.dll
3720    vmware-tray.ex  0x74f60000      False   False   False   \Windows\SysWOW64\mscoree.dll
3720    vmware-tray.ex  0x75000000      False   False   False   \Windows\winsxs\x86_microsoft.windows.common-controls_6595b64144ccf1df_6.0.7601.17514_none_41e6975e2bd6f2b2\comctl32.dll
3720    vmware-tray.ex  0x751b0000      True    True    True    \Windows\System32\wow64win.dll
3720    vmware-tray.ex  0x75430000      False   False   False   \Windows\SysWOW64\sspicli.dll
3720    vmware-tray.ex  0x75420000      False   False   False   \Windows\SysWOW64\cryptbase.dll
3720    vmware-tray.ex  0x76160000      False   False   False   \Windows\SysWOW64\msvcrt.dll
3720    vmware-tray.ex  0x75d30000      False   False   False   \Windows\SysWOW64\KernelBase.dll
3720    vmware-tray.ex  0x757d0000      False   False   False   \Windows\SysWOW64\lpk.dll
3720    vmware-tray.ex  0x755e0000      False   False   False   \Windows\SysWOW64\advapi32.dll
3720    vmware-tray.ex  0x75ad0000      False   False   False   \Windows\SysWOW64\usp10.dll
3720    vmware-tray.ex  0x75de0000      False   False   False   \Windows\SysWOW64\sechost.dll
3720    vmware-tray.ex  0x75d80000      False   False   False   \Windows\SysWOW64\imm32.dll
3720    vmware-tray.ex  0x76000000      False   False   False   \Windows\SysWOW64\ole32.dll
3720    vmware-tray.ex  0x77200000      False   False   False   \Windows\SysWOW64\shlwapi.dll
3720    vmware-tray.ex  0x76e70000      False   False   False   \Windows\SysWOW64\gdi32.dll
3720    vmware-tray.ex  0x76220000      False   False   False   \Windows\SysWOW64\shell32.dll
3720    vmware-tray.ex  0x76f00000      False   False   False   \Windows\SysWOW64\user32.dll
3720    vmware-tray.ex  0x772f0000      False   False   False   \Windows\SysWOW64\kernel32.dll
3720    vmware-tray.ex  0x77400000      False   False   False   \Windows\SysWOW64\msctf.dll
3720    vmware-tray.ex  0x776f0000      True    True    True    \Windows\System32\ntdll.dll
3720    vmware-tray.ex  0x778d0000      False   False   False   \Windows\SysWOW64\ntdll.dll
```

# windows.ldrmodules.LdrModules 分析

## 1. Plugin 功能說明

`windows.ldrmodules.LdrModules` 是 Volatility 3 用來檢查 Process 載入模組狀態的 Plugin。

它會比對 Process 中的模組是否存在於 Windows 的 Loader List 中，主要用來觀察：

* Process 載入了哪些 EXE / DLL 模組
* 模組路徑是否正常
* 是否有從可疑路徑載入模組
* 是否有模組不在正常 Loader List 中
* 是否可能存在隱藏模組或可疑載入行為

本次使用此 Plugin 的目的，是確認 `Rick And Morty` 與 `vmware-tray.exe` 的模組路徑是否合理，以及兩者是否存在可疑載入特徵。

---

## 2. 欄位說明

| 欄位           | 說明                              |
| ------------ | ------------------------------- |
| `Pid`        | Process ID，行程編號                 |
| `Process`    | Process 名稱                      |
| `Base`       | 模組載入到記憶體中的基底位址                  |
| `InLoad`     | 是否存在於 Load Order List           |
| `InInit`     | 是否存在於 Initialization Order List |
| `InMem`      | 是否存在於 Memory Order List         |
| `MappedPath` | 模組對應的檔案路徑                       |

其中 `InLoad`、`InInit`、`InMem` 是用來判斷模組是否存在於不同的 Loader List 中。

如果某個模組顯示：

```text id="6o9wox"
False False False
```

不一定代表惡意，還要看它的檔案路徑與 Process 行為。
例如 Windows 系統 DLL、語言資源檔、.NET 模組，有時也可能顯示 `False`。

本次真正需要注意的是路徑是否異常。

---

## 3. 分析目標

本次只分析以下兩個可疑 Process：

|  PID | Process           | 路徑                                                       |
| ---: | ----------------- | -------------------------------------------------------- |
| 3820 | `Rick And Morty`  | `\Torrents\Rick And Morty season 1 download.exe`         |
| 3720 | `vmware-tray.exe` | `\Users\Rick\AppData\Local\Temp\RarSFX0\vmware-tray.exe` |

這兩個 Process 是目前最重要的可疑執行鏈。

---

## 4. PID 3820 - Rick And Morty 分析

### 4.1 主要發現

```text id="kndkqk"
PID: 3820
Process: Rick And Morty
MappedPath: \Torrents\Rick And Morty season 1 download.exe
```

`Rick And Morty` 的主程式位於 `\Torrents` 目錄，檔名看起來像影片下載檔案，但實際上是 `.exe` 可執行檔。

這是本次分析中最明顯的可疑點。

---

### 4.2 模組載入狀況

此 Process 載入的模組大多是 Windows 32-bit 系統模組，例如：

```text id="jk6o8z"
\Windows\SysWOW64\kernel32.dll
\Windows\SysWOW64\user32.dll
\Windows\SysWOW64\shell32.dll
\Windows\SysWOW64\wininet.dll
\Windows\SysWOW64\urlmon.dll
\Windows\SysWOW64\crypt32.dll
\Windows\System32\wow64.dll
\Windows\System32\wow64cpu.dll
\Windows\System32\wow64win.dll
\Windows\System32\ntdll.dll
```

其中 `wow64.dll`、`wow64cpu.dll`、`wow64win.dll` 代表此程式是 32-bit 程式，正在 64-bit Windows 環境中執行。

另外，`wininet.dll`、`urlmon.dll`、`crypt32.dll` 代表程式可能具備網路連線、URL 存取或憑證處理能力。不過這些 DLL 本身不能直接判斷惡意，需要搭配其他 Plugin 分析。

---

### 4.3 Loader List 狀態

主程式顯示：

```text id="20s83b"
InLoad: True
InInit: False
InMem: True
```

這代表主程式存在於主要 Loader List 與記憶體中。

`InInit` 為 `False` 不一定代表惡意，因為不是所有模組都一定會出現在 Initialization Order List 中。

本 Process 的重點不是 `InInit=False`，而是主程式路徑與檔名高度可疑。

---

### 4.4 鑑識判斷

`Rick And Morty season 1 download.exe` 具有以下可疑特徵：

| 項目   | 分析                  |
| ---- | ------------------- |
| 檔名   | 偽裝成影片下載             |
| 副檔名  | 實際為 `.exe`          |
| 位置   | 位於 `\Torrents` 下載目錄 |
| 程式型態 | 32-bit 程式           |
| 可疑程度 | 高                   |

判斷：

```text id="ev2gvv"
PID 3820 Rick And Morty 是本次主要可疑程式。
```

---

## 5. PID 3720 - vmware-tray.exe 分析

### 5.1 主要發現

```text id="l5v4sb"
PID: 3720
Process: vmware-tray.exe
MappedPath: \Users\Rick\AppData\Local\Temp\RarSFX0\vmware-tray.exe
```

此 Process 名稱看起來像 VMware Tools 相關程式，但實際路徑位於使用者 Temp 目錄下的 `RarSFX0`。

正常 VMware Tools 程式通常應位於類似：

```text id="nwoa7d"
C:\Program Files\VMware\VMware Tools\
```

但本次發現的路徑是：

```text id="utxtco"
C:\Users\Rick\AppData\Local\Temp\RarSFX0\
```

因此此 `vmware-tray.exe` 不像正常 VMware 元件。

---

### 5.2 模組載入狀況

`vmware-tray.exe` 載入多個 .NET Framework 相關模組，例如：

```text id="1yq5j8"
\Windows\Microsoft.NET\Framework\v4.0.30319\clr.dll
\Windows\Microsoft.NET\Framework\v4.0.30319\clrjit.dll
\Windows\Microsoft.NET\Framework\v4.0.30319\mscoreei.dll
\Windows\Microsoft.NET\Framework\v4.0.30319\mscorrc.dll
\Windows\assembly\NativeImages_v4.0.30319_32\System.Windows.Forms\
\Windows\assembly\NativeImages_v4.0.30319_32\System.Drawing\
\Windows\assembly\NativeImages_v4.0.30319_32\System.Core\
\Windows\assembly\NativeImages_v4.0.30319_32\mscorlib\
```

這表示 `vmware-tray.exe` 很可能是 .NET 程式。

其中 `System.Windows.Forms`、`System.Drawing` 代表它可能具有圖形介面或視窗元件。

---

### 5.3 Loader List 狀態

主程式顯示：

```text id="gkgnms"
InLoad: True
InInit: False
InMem: True
```

這代表主程式存在於 Loader List 與記憶體中。

這個狀態本身不是最可疑的地方。真正可疑的是它的執行路徑：

```text id="evl5yt"
\Users\Rick\AppData\Local\Temp\RarSFX0\vmware-tray.exe
```

`RarSFX0` 通常與自解壓縮檔釋放的暫存目錄有關，因此此程式可能是被其他執行檔釋放後啟動。

---

### 5.4 鑑識判斷

`vmware-tray.exe` 具有以下可疑特徵：

| 項目   | 分析                  |
| ---- | ------------------- |
| 檔名   | 偽裝成 VMware Tools 元件 |
| 路徑   | 位於使用者 Temp 目錄       |
| 目錄   | `RarSFX0`，疑似自解壓暫存路徑 |
| 程式型態 | .NET 程式             |
| 可疑程度 | 高                   |

判斷：

```text id="6v65ci"
PID 3720 vmware-tray.exe 很可能是由 Rick And Morty 釋放或啟動的可疑子程式。
```

---

## 6. 兩者關聯分析

從 `LdrModules` 的結果來看，這兩個 Process 的路徑關係非常重要：

```text id="6zy5ua"
\Torrents\Rick And Morty season 1 download.exe
↓
\Users\Rick\AppData\Local\Temp\RarSFX0\vmware-tray.exe
```

`Rick And Morty` 位於 Torrent 下載目錄，檔名偽裝成影片下載，但實際是 EXE。

`vmware-tray.exe` 則位於使用者 Temp 的 `RarSFX0` 目錄，名稱偽裝成 VMware 元件，但不在正常 VMware 安裝路徑。

因此可以推論：

```text id="0i92nw"
Rick And Morty season 1 download.exe 執行後，很可能釋放或啟動了 Temp\RarSFX0\vmware-tray.exe。
```

---

## 7. 可疑程度比較

|  PID | Process           | 可疑程度 | 原因                                 |
| ---: | ----------------- | ---- | ---------------------------------- |
| 3820 | `Rick And Morty`  | 高    | 偽裝成影片下載的 EXE，位於 Torrent 目錄         |
| 3720 | `vmware-tray.exe` | 高    | 從 Temp `RarSFX0` 執行，名稱偽裝 VMware 元件 |

兩者角色不同：

| Process           | 角色判斷         |
| ----------------- | ------------ |
| `Rick And Morty`  | 主要可疑執行檔      |
| `vmware-tray.exe` | 被釋放或啟動的可疑子程式 |

---

## 8. 結論

本次 `windows.ldrmodules.LdrModules` 分析確認了兩個重要可疑 Process。

第一個是：

```text id="kntcws"
PID 3820 - Rick And Morty
\Torrents\Rick And Morty season 1 download.exe
```

此檔案名稱偽裝成影片下載，但實際上是可執行檔，且位於 Torrent 下載目錄，因此具有高度可疑性。

第二個是：

```text id="rh1g3t"
PID 3720 - vmware-tray.exe
\Users\Rick\AppData\Local\Temp\RarSFX0\vmware-tray.exe
```

此程式名稱偽裝成 VMware Tools 元件，但實際執行位置位於使用者 Temp 目錄下的 `RarSFX0`，不屬於正常 VMware 安裝路徑，因此同樣高度可疑。

綜合判斷，這兩個 Process 很可能屬於同一條可疑執行鏈：

```text id="k8zfwm"
Rick And Morty season 1 download.exe
↓
Temp\RarSFX0\vmware-tray.exe
```

`Rick And Morty` 可視為主要可疑程式，`vmware-tray.exe` 則可能是其釋放或啟動的子程式。

---

## 9. 後續建議

建議接著針對這兩個 PID 執行 `malfind`：

```bash id="jnyd54"
.\vol.exe -f .\OtterCTF.vmem windows.malfind.Malfind --pid 3820
.\vol.exe -f .\OtterCTF.vmem windows.malfind.Malfind --pid 3720
```

如果需要補充記憶體區段資訊，可再執行：

```bash id="wz5itp"
.\vol.exe -f .\OtterCTF.vmem windows.vadinfo.VadInfo --pid 3820
.\vol.exe -f .\OtterCTF.vmem windows.vadinfo.VadInfo --pid 3720
```
