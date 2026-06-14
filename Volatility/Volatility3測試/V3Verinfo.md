# 測試內容

- vol.exe -f .\OtterCTF.vmem windows.verinfo.VerInfo
```
D:\Forensic\G140A006\VolatilityWorkbench>.\vol.exe -f .\OtterCTF.vmem windows.verinfo.VerInfo
Volatility 3 Framework 2.5.0
Progress:  100.00               PDB scanning finished
PID     Process Base    Name    Major   Minor   Product Build

N/A     N/A     0xf80002a52000  ntoskrnl.exe    6       1       7601    17514
N/A     N/A     0xf80002a09000  hal.dll -       -       -       -
N/A     N/A     0xf80000bb6000  kdcom.dll       -       -       -       -
N/A     N/A     0xf88000c1f000  mcupdate.dll    -       -       -       -
N/A     N/A     0xf88000c6e000  PSHED.dll       -       -       -       -
N/A     N/A     0xf88000c82000  CLFS.SYS        -       -       -       -
N/A     N/A     0xf88000ce0000  CI.dll  -       -       -       -
N/A     N/A     0xf88000efa000  Wdf01000.sys    -       -       -       -
N/A     N/A     0xf88000f9e000  WDFLDR.SYS      -       -       -       -
N/A     N/A     0xf88000e00000  ACPI.sys        -       -       -       -
N/A     N/A     0xf88000e57000  WMILIB.SYS      -       -       -       -
N/A     N/A     0xf88000e60000  msisadrv.sys    -       -       -       -
N/A     N/A     0xf88000e6a000  pci.sys -       -       -       -
N/A     N/A     0xf88000e9d000  vdrvroot.sys    -       -       -       -
N/A     N/A     0xf88000eaa000  partmgr.sys     -       -       -       -
N/A     N/A     0xf88000ebf000  compbatt.sys    -       -       -       -
N/A     N/A     0xf88000ec8000  BATTC.SYS       -       -       -       -
N/A     N/A     0xf88000ed4000  volmgr.sys      -       -       -       -
N/A     N/A     0xf88000da0000  volmgrx.sys     -       -       -       -
N/A     N/A     0xf88000ee9000  intelide.sys    -       -       -       -
N/A     N/A     0xf88000fad000  PCIIDEX.SYS     -       -       -       -
N/A     N/A     0xf88000fbd000  vmci.sys        -       -       -       -
N/A     N/A     0xf88000fd6000  mountmgr.sys    -       -       -       -
N/A     N/A     0xf88000c00000  vsock.sys       -       -       -       -
N/A     N/A     0xf88000ff0000  atapi.sys       -       -       -       -
N/A     N/A     0xf880010ae000  ataport.SYS     -       -       -       -
N/A     N/A     0xf880010d8000  lsi_sas.sys     -       -       -       -
N/A     N/A     0xf880010f5000  storport.sys    -       -       -       -
N/A     N/A     0xf88001158000  msahci.sys      -       -       -       -
N/A     N/A     0xf88001163000  amdxata.sys     -       -       -       -
N/A     N/A     0xf8800116e000  fltmgr.sys      -       -       -       -
N/A     N/A     0xf880011ba000  fileinfo.sys    -       -       -       -
N/A     N/A     0xf8800125d000  Ntfs.sys        -       -       -       -
N/A     N/A     0xf88001000000  msrpc.sys       -       -       -       -
N/A     N/A     0xf88001200000  ksecdd.sys      -       -       -       -
N/A     N/A     0xf88001474000  cng.sys -       -       -       -
N/A     N/A     0xf880014e6000  pcw.sys -       -       -       -
N/A     N/A     0xf880014f7000  Fs_Rec.sys      -       -       -       -
N/A     N/A     0xf88001501000  ndis.sys        -       -       -       -
N/A     N/A     0xf88001400000  NETIO.SYS       -       -       -       -
N/A     N/A     0xf8800121b000  ksecpkg.sys     -       -       -       -
N/A     N/A     0xf88001637000  tcpip.sys       -       -       -       -
N/A     N/A     0xf8800183b000  fwpkclnt.sys    -       -       -       -
N/A     N/A     0xf88001885000  vmstorfl.sys    -       -       -       -
...
....
.....
```

- vol.exe -f .\OtterCTF.vmem windows.verinfo.VerInfo | findstr 3820
```
D:\Forensic\G140A006\VolatilityWorkbench>.\vol.exe -f .\OtterCTF.vmem windows.verinfo.VerInfo | findstr 3820
3820ressRick And Morty  0x400000PDB scanRick And Morty season 1 download.exe    -       -       --
3820    Rick And Morty  0x776f0000      ntdll.dll       -       -       -       -
3820    Rick And Morty  0x75210000      wow64.dll       -       -       -       -
3820    Rick And Morty  0x751b0000      wow64win.dll    -       -       -       -
3820    Rick And Morty  0x751a0000      wow64cpu.dll    -       -       -       -
```

- vol.exe -f .\OtterCTF.vmem windows.verinfo.VerInfo | findstr 3720
```
D:\Forensic\G140A006\VolatilityWorkbench>.\vol.exe -f .\OtterCTF.vmem windows.verinfo.VerInfo | findstr 3720
3720ressvmware-tray.ex  0xec0000PDB scanvmware-tray.exe 1       0       0       0
3720    vmware-tray.ex  0x776f0000      ntdll.dll       -       -       -       -
3720    vmware-tray.ex  0x75210000      wow64.dll       -       -       -       -
3720    vmware-tray.ex  0x751b0000      wow64win.dll    -       -       -       -
3720    vmware-tray.ex  0x751a0000      wow64cpu.dll    -       -       -       -
```

# windows.verinfo.VerInfo 分析

## 1. Plugin 功能說明

`windows.verinfo.VerInfo` 用來查看記憶體中 EXE / DLL 模組的版本資訊。

本次欄位如下：

| 欄位        | 說明             |
| --------- | -------------- |
| `PID`     | 行程編號           |
| `Process` | 行程名稱           |
| `Base`    | 模組載入到記憶體中的基底位址 |
| `Name`    | 模組名稱           |
| `Major`   | 主要版本號          |
| `Minor`   | 次要版本號          |
| `Product` | 產品版本號          |
| `Build`   | Build 編號       |

此 Plugin 可以用來判斷可疑程式是否有正常的版本資訊。
如果檔案偽裝成正常軟體，但版本資訊不完整或不合理，就需要特別注意。

---

## 2. 執行方式

`VerInfo` 不支援 `--pid`，因此本次使用 `findstr` 篩選指定 PID：

```bash id="69v2v6"
.\vol.exe -f .\OtterCTF.vmem windows.verinfo.VerInfo | findstr 3820
.\vol.exe -f .\OtterCTF.vmem windows.verinfo.VerInfo | findstr 3720
```

---

## 3. PID 3820 - Rick And Morty 分析

### 3.1 結果

```text id="z9w1br"
PID: 3820
Process: Rick And Morty
Base: 0x400000
Name: Rick And Morty season 1 download.exe
Major: -
Minor: -
Product: -
Build: -
```

### 3.2 分析

`Rick And Morty season 1 download.exe` 沒有版本資訊，`Major`、`Minor`、`Product`、`Build` 皆為 `-`。

這代表該檔案沒有正常軟體常見的版本標示。

此檔案名稱看起來像影片下載，但實際上是 `.exe`，因此具有偽裝特徵。

### 3.3 判斷

```text id="avzdrc"
PID 3820 Rick And Morty 沒有版本資訊，且檔名偽裝成影片下載，因此具有高度可疑性。
```

---

## 4. PID 3720 - vmware-tray.exe 分析

### 4.1 結果

```text id="7s0544"
PID: 3720
Process: vmware-tray.ex
Base: 0xec0000
Name: vmware-tray.exe
Major: 1
Minor: 0
Product: 0
Build: 0
```

### 4.2 分析

`vmware-tray.exe` 有版本號：

```text id="mggmih"
1.0.0.0
```

但是這個版本資訊非常簡單，只有基本數字，沒有顯示出明確的 VMware 產品資訊。

如果是真正 VMware Tools 元件，通常應該會有較完整的版本資訊。
再加上前面已確認它的路徑位於：

```text id="dqfbd3"
\Users\Rick\AppData\Local\Temp\RarSFX0\vmware-tray.exe
```

此路徑不是正常 VMware Tools 安裝路徑，因此仍然高度可疑。

### 4.3 判斷

```text id="dlbnj5"
PID 3720 vmware-tray.exe 雖然有版本號 1.0.0.0，但資訊過於簡單，且路徑位於 Temp\RarSFX0，因此不像正常 VMware 元件。
```

---

## 5. 比較表

|  PID | Process          | Name                                   | Major | Minor | Product | Build | 判斷             |
| ---: | ---------------- | -------------------------------------- | ----: | ----: | ------: | ----: | -------------- |
| 3820 | `Rick And Morty` | `Rick And Morty season 1 download.exe` |   `-` |   `-` |     `-` |   `-` | 無版本資訊，高度可疑     |
| 3720 | `vmware-tray.ex` | `vmware-tray.exe`                      |   `1` |   `0` |     `0` |   `0` | 版本資訊過於簡單，且路徑可疑 |

---

## 6. 綜合判斷

本次 `VerInfo` 分析顯示：

```text id="er3c7i"
Rick And Morty season 1 download.exe 沒有版本資訊。
vmware-tray.exe 只有簡單版本號 1.0.0.0。
```

這兩個結果都不符合正常可信軟體應有的完整版本資訊。

綜合前面已知的路徑與行程關係，可判斷：

```text id="kakutp"
Rick And Morty season 1 download.exe
↓
Temp\RarSFX0\vmware-tray.exe
```

這兩個檔案仍然屬於高度可疑執行鏈。
