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

## 1. 分析目標

本次只針對以下兩個可疑 Process 進行 `LdrModules` 分析：

|  PID | Process           | 路徑                                                       |
| ---: | ----------------- | -------------------------------------------------------- |
| 3820 | `Rick And Morty`  | `\Torrents\Rick And Morty season 1 download.exe`         |
| 3720 | `vmware-tray.exe` | `\Users\Rick\AppData\Local\Temp\RarSFX0\vmware-tray.exe` |

這兩個 Process 是目前最重要的可疑執行鏈。

---

## 2. PID 3820 - Rick And Morty 分析

### 2.1 主要發現

```text
PID: 3820
Process: Rick And Morty
MappedPath: \Torrents\Rick And Morty season 1 download.exe
```

`Rick And Morty` 的主程式位於 `\Torrents` 目錄，檔名看起來像影片下載檔案，但實際上是 `.exe` 可執行檔。

這是本次分析中最明顯的可疑點。

### 2.2 模組載入狀況

此 Process 載入的模組大多是 Windows 32-bit 系統模組，例如：

```text
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

其中 `wow64.dll`、`wow64cpu.dll`、`wow64win.dll` 表示此程式是 32-bit 程式，正在 64-bit Windows 環境中執行。

另外，`wininet.dll`、`urlmon.dll`、`crypt32.dll` 代表程式可能具備網路連線、URL 存取或憑證處理能力。不過這些 DLL 本身不代表惡意，仍需搭配其他 Plugin 判斷。

### 2.3 InLoad / InInit / InMem 判斷

主程式顯示：

```text
InLoad: True
InInit: False
InMem: True
```

代表此主模組存在於主要 Loader List 與記憶體中。`InInit` 為 `False` 不一定代表惡意，因為不同模組在初始化清單中的狀態可能不同。

本次重點不是 `InInit=False`，而是主程式路徑與檔名高度可疑。

### 2.4 鑑識判斷

`Rick And Morty season 1 download.exe` 具有以下可疑特徵：

| 項目   | 分析                          |
| ---- | --------------------------- |
| 檔名   | 偽裝成影片下載                     |
| 副檔名  | 實際為 `.exe`                  |
| 位置   | 位於 `\Torrents` 下載目錄         |
| 執行型態 | 32-bit 程式執行於 64-bit Windows |
| 可疑程度 | 高                           |

判斷：

```text
PID 3820 Rick And Morty 是本次主要可疑程式。
```

---

## 3. PID 3720 - vmware-tray.exe 分析

### 3.1 主要發現

```text
PID: 3720
Process: vmware-tray.exe
MappedPath: \Users\Rick\AppData\Local\Temp\RarSFX0\vmware-tray.exe
```

此 Process 名稱看起來像 VMware Tools 相關程式，但實際路徑位於使用者 Temp 目錄下的 `RarSFX0`。

正常 VMware Tools 程式通常應位於類似：

```text
C:\Program Files\VMware\VMware Tools\
```

但本次發現的路徑是：

```text
C:\Users\Rick\AppData\Local\Temp\RarSFX0\
```

因此此 `vmware-tray.exe` 不像正常 VMware 元件。

### 3.2 模組載入狀況

`vmware-tray.exe` 載入多個 .NET Framework 相關模組，例如：

```text
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

### 3.3 InLoad / InInit / InMem 判斷

主程式顯示：

```text
InLoad: True
InInit: False
InMem: True
```

代表主程式存在於 Loader List 與記憶體中。這個狀態本身不是最可疑的地方。

真正可疑的是：

```text
\Users\Rick\AppData\Local\Temp\RarSFX0\vmware-tray.exe
```

`RarSFX0` 通常與自解壓縮檔釋放的暫存目錄有關，因此此程式可能是被其他執行檔釋放後啟動。

### 3.4 鑑識判斷

`vmware-tray.exe` 具有以下可疑特徵：

| 項目   | 分析                  |
| ---- | ------------------- |
| 檔名   | 偽裝成 VMware Tools 元件 |
| 路徑   | 位於使用者 Temp 目錄       |
| 目錄   | `RarSFX0`，疑似自解壓暫存路徑 |
| 程式型態 | .NET 程式             |
| 可疑程度 | 高                   |

判斷：

```text
PID 3720 vmware-tray.exe 很可能是由 Rick And Morty 釋放或啟動的可疑子程式。
```

---

## 4. 兩者關聯分析

從 `LdrModules` 的結果來看，這兩個 Process 的路徑關係非常重要：

```text
\Torrents\Rick And Morty season 1 download.exe
↓
\Users\Rick\AppData\Local\Temp\RarSFX0\vmware-tray.exe
```

`Rick And Morty` 位於 Torrent 下載目錄，檔名偽裝成影片下載，但實際是 EXE。

`vmware-tray.exe` 則位於使用者 Temp 的 `RarSFX0` 目錄，名稱偽裝成 VMware 元件，但不在正常 VMware 安裝路徑。

因此可以推論：

```text
Rick And Morty season 1 download.exe 執行後，很可能釋放或啟動了 Temp\RarSFX0\vmware-tray.exe。
```

---

## 5. 可疑程度比較

|  PID | Process           | 可疑程度 | 原因                                 |
| ---: | ----------------- | ---- | ---------------------------------- |
| 3820 | `Rick And Morty`  | 高    | 偽裝成影片下載的 EXE，位於 Torrent 目錄         |
| 3720 | `vmware-tray.exe` | 高    | 從 Temp `RarSFX0` 執行，名稱偽裝 VMware 元件 |

兩者都是高可疑，但角色不同：

| Process           | 角色判斷         |
| ----------------- | ------------ |
| `Rick And Morty`  | 主要可疑執行檔      |
| `vmware-tray.exe` | 被釋放或啟動的可疑子程式 |

---

## 6. 結論

本次 `windows.ldrmodules.LdrModules` 分析確認了兩個重要可疑 Process。

第一個是：

```text
PID 3820 - Rick And Morty
\Torrents\Rick And Morty season 1 download.exe
```

此檔案名稱偽裝成影片下載，但實際上是可執行檔，且位於 Torrent 下載目錄，因此具有高度可疑性。

第二個是：

```text
PID 3720 - vmware-tray.exe
\Users\Rick\AppData\Local\Temp\RarSFX0\vmware-tray.exe
```

此程式名稱偽裝成 VMware Tools 元件，但實際執行位置位於使用者 Temp 目錄下的 `RarSFX0`，不屬於正常 VMware 安裝路徑，因此同樣高度可疑。

綜合判斷，這兩個 Process 很可能屬於同一條可疑執行鏈：

```text
Rick And Morty season 1 download.exe
↓
Temp\RarSFX0\vmware-tray.exe
```

`Rick And Morty` 可視為主要可疑程式，`vmware-tray.exe` 則可能是其釋放或啟動的子程式。

---

## 7. 後續建議

建議接著針對這兩個 PID 執行 `malfind`：

```bash
.\vol.exe -f .\OtterCTF.vmem windows.malfind.Malfind --pid 3820
.\vol.exe -f .\OtterCTF.vmem windows.malfind.Malfind --pid 3720
```

如果需要補充記憶體區段資訊，可再執行：

```bash
.\vol.exe -f .\OtterCTF.vmem windows.vadinfo.VadInfo --pid 3820
.\vol.exe -f .\OtterCTF.vmem windows.vadinfo.VadInfo --pid 3720
```
