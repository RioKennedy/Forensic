# 測試內容
- vol.exe -f .\OtterCTF.vmem windows.memmap.Memmap

```
D:\Forensic\G140A006\VolatilityWorkbench>.\vol.exe -f .\OtterCTF.vmem windows.memmap.Memmap
Volatility 3 Framework 2.5.0
Progress:  100.00               PDB scanning finished
Virtual Physical        Size    Offset in File  File output

0x10000 0x2d58a000      0x2000  0x0     Disabled
0x12000 0x2d54c000      0x4000  0x2000  Disabled
0x16000 0x2d590000      0x2000  0x6000  Disabled
0x18000 0x2d5d2000      0x3000  0x8000  Disabled
0x1b000 0x2d595000      0xa000  0xb000  Disabled
0x25000 0x2d55f000      0x1000  0x15000 Disabled
0x26000 0x2d5a0000      0x1000  0x16000 Disabled
0x27000 0x2d561000      0x4000  0x17000 Disabled
0x2b000 0x2d5a5000      0x2000  0x1b000 Disabled
0x2d000 0x2d567000      0x2000  0x1d000 Disabled
0x2f000 0x2d5a9000      0x3000  0x1f000 Disabled
0x32000 0x2d5ec000      0x1000  0x22000 Disabled
0x40000 0x2ca0d000      0x3000  0x23000 Disabled
0x43000 0x2c090000      0x1000  0x26000 Disabled
0x44000 0x2c0d1000      0x1000  0x27000 Disabled
0x45000 0x2c112000      0x3000  0x28000 Disabled
0x48000 0x2c0d5000      0x1000  0x2b000 Disabled
0x49000 0x2ca16000      0x5000  0x2c000 Disabled
0x4e000 0x2c09b000      0x1000  0x31000 Disabled
0x4f000 0x2c99c000      0x1000  0x32000 Disabled
0x50000 0x2c09d000      0x1000  0x33000 Disabled
0x51000 0x2c59e000      0x1000  0x34000 Disabled
0x52000 0x2c19f000      0x1000  0x35000 Disabled
0x53000 0x2c0a0000      0x1000  0x36000 Disabled
0x54000 0x2c0e1000      0x1000  0x37000 Disabled
0x55000 0x2c0a2000      0x1000  0x38000 Disabled
0x56000 0x11823000      0x1000  0x39000 Disabled
0x57000 0x2c0a4000      0x4000  0x3a000 Disabled
0x5b000 0x2c028000      0x1000  0x3e000 Disabled
0x5c000 0x2c0e9000      0x2000  0x3f000 Disabled
0x5e000 0x2c0ab000      0x1000  0x41000 Disabled
0x5f000 0x2c0ec000      0x1000  0x42000 Disabled
0x60000 0x2c12d000      0x1000  0x43000 Disabled
0x61000 0x1186e000      0x1000  0x44000 Disabled
0x62000 0x2c0ef000      0x1000  0x45000 Disabled
0x63000 0x2c070000      0x1000  0x46000 Disabled
0x64000 0x2c0b1000      0x1000  0x47000 Disabled
0x65000 0x2c072000      0x1000  0x48000 Disabled
0x66000 0x2ca33000      0x1000  0x49000 Disabled
0x67000 0x2c0f4000      0x1000  0x4a000 Disabled
0x68000 0x2ca75000      0x2000  0x4b000 Disabled
0x6a000 0x2ca37000      0x1000  0x4d000 Disabled
0x6b000 0x2ca78000      0x1000  0x4e000 Disabled
0x6c000 0x2ca39000      0x2000  0x4f000 Disabled
0x6e000 0x2ca7b000      0x2000  0x51000 Disabled
0x70000 0x2c87d000      0x1000  0x53000 Disabled
0x71000 0x2c67e000      0x1000  0x54000 Disabled
0x72000 0x2c33f000      0x1000  0x55000 Disabled
0x73000 0x2c980000      0x1000  0x56000 Disabled
0x74000 0x2c901000      0x1000  0x57000 Disabled
0x75000 0x2c082000      0x1000  0x58000 Disabled
0x76000 0x2c943000      0x2000  0x59000 Disabled
0x78000 0x2c985000      0x1000  0x5b000 Disabled
0x79000 0x2cb06000      0x1000  0x5c000 Disabled
0x7a000 0x2c047000      0x1000  0x5d000 Disabled
0x7b000 0x2c088000      0x1000  0x5e000 Disabled
0x7c000 0x2c049000      0x1000  0x5f000 Disabled
0x7d000 0x2c08a000      0x2000  0x60000 Disabled
0x7f000 0x2c04c000      0x1000  0x62000 Disabled
...
....
.....
```
# windows.memmap.Memmap 分析說明

## 1. Plugin 功能說明

`windows.memmap.Memmap` 是 Volatility 3 中用來顯示記憶體映射關係的 Plugin。

它主要會列出記憶體映像檔中的：

* 虛擬位址 Virtual Address
* 實體位址 Physical Address
* 記憶體區段大小 Size
* 記憶體位址對應關係
* 是否可以將該記憶體區段輸出

簡單來說，`memmap` 是用來查看 Windows 記憶體中「虛擬記憶體位址」如何對應到「實體記憶體位址」的工具。

---

## 2. 為什麼結果很多？

執行 `windows.memmap.Memmap` 後，結果通常會非常多，這是正常情況。

原因是 Windows 系統在執行時，每個 Process 都會有自己的記憶體空間，而且每個 Process 內又會包含許多不同的記憶體區段，例如：

* 程式本身的記憶體區段
* DLL 載入區段
* Heap 記憶體
* Stack 記憶體
* Shared Memory
* Memory Mapped File
* Kernel Memory
* Cache

因此，如果直接執行：

```bash
.\vol.exe -f .\OtterCTF.vmem windows.memmap.Memmap
```

Volatility 會列出大量記憶體映射資料，導致結果非常龐大，不適合人工逐行查看。

---

## 3. 常見欄位說明

`windows.memmap.Memmap` 的結果通常會包含以下欄位：

| 欄位          | 說明            |
| ----------- | ------------- |
| PID         | 行程編號          |
| Process     | 行程名稱          |
| Virtual     | 虛擬記憶體位址       |
| Physical    | 實體記憶體位址       |
| Size        | 記憶體區段大小       |
| Offset      | 在記憶體映像檔中的偏移位置 |
| File output | 是否可以輸出記憶體內容   |

---

## 4. 重要欄位分析

### 4.1 PID

`PID` 是 Process ID，也就是行程編號。

在記憶體鑑識中，PID 很重要，因為我們通常會先透過其他 Plugin 找出可疑行程，再針對特定 PID 進行深入分析。

例如：

```bash
.\vol.exe -f .\OtterCTF.vmem windows.memmap.Memmap --pid 708
```

這樣可以只分析 PID 708 的記憶體映射，避免結果太多。

---

### 4.2 Process

`Process` 是行程名稱。

它可以協助分析人員知道目前這些記憶體區段屬於哪一個行程。

例如，如果某個可疑行程名稱是：

```text
malware.exe
```

或是不正常的位置出現：

```text
explorer.exe
cmd.exe
powershell.exe
```

就可以針對該 Process 的記憶體進一步分析。

---

### 4.3 Virtual Address

`Virtual Address` 是虛擬記憶體位址。

每個 Process 在 Windows 中都有自己的虛擬記憶體空間，因此不同 Process 可能會看到相同的虛擬位址，但實際上對應到不同的實體記憶體位置。

在鑑識分析中，Virtual Address 可以用來定位某個 Process 內部的記憶體區段。

如果後續 `malfind` 或 `vadinfo` 發現某段可疑記憶體，就可以利用 Virtual Address 進一步比對。

---

### 4.4 Physical Address

`Physical Address` 是實體記憶體位址。

Volatility 會透過 Windows 的分頁結構，把 Process 的 Virtual Address 轉換成 Physical Address。

如果某個 Virtual Address 找不到對應的 Physical Address，可能代表：

* 該記憶體頁面不存在於目前記憶體映像檔中
* 該記憶體頁面已被交換出去
* 該記憶體頁面無法被解析
* 記憶體擷取時沒有完整保存該區段

---

### 4.5 Size

`Size` 表示該記憶體區段的大小。

如果某些記憶體區段特別大，可能代表：

* 程式載入大型模組
* Process 使用大量 Heap
* 有大型 Memory Mapped File
* 有可疑記憶體配置

但是單看 Size 不能直接判斷是否為惡意，需要搭配其他 Plugin 交叉分析。

---

## 5. 鑑識分析重點

`windows.memmap.Memmap` 的重點不是直接找出惡意程式，而是用來輔助分析特定 Process 的記憶體配置。

它比較重要的用途包含：

1. 查看某個 Process 的記憶體映射範圍
2. 確認虛擬位址與實體位址的對應關係
3. 輔助 Dump 特定記憶體區段
4. 搭配 `malfind` 分析可疑記憶體
5. 搭配 `vadinfo` 查看 Process 的 VAD 記憶體區段

---

## 6. 不建議直接分析全部結果

如果直接執行：

```bash
.\vol.exe -f .\OtterCTF.vmem windows.memmap.Memmap
```

結果會非常多，因此不建議人工逐行分析全部內容。

比較好的方法是先透過以下 Plugin 找出可疑 PID：

```bash
.\vol.exe -f .\OtterCTF.vmem windows.pslist.PsList
.\vol.exe -f .\OtterCTF.vmem windows.pstree.PsTree
.\vol.exe -f .\OtterCTF.vmem windows.cmdline.CmdLine
.\vol.exe -f .\OtterCTF.vmem windows.netscan.NetScan
.\vol.exe -f .\OtterCTF.vmem windows.malfind.Malfind
```

找到可疑 PID 後，再針對單一 PID 執行：

```bash
.\vol.exe -f .\OtterCTF.vmem windows.memmap.Memmap --pid <PID>
```

例如：

```bash
.\vol.exe -f .\OtterCTF.vmem windows.memmap.Memmap --pid 708
```

這樣可以縮小分析範圍，讓結果更容易判讀。

---

## 7. 與其他 Plugin 的關係

`windows.memmap.Memmap` 通常不會單獨使用，而是搭配其他 Plugin 一起分析。

| 搭配 Plugin                     | 用途                     |
| ----------------------------- | ---------------------- |
| `windows.pslist.PsList`       | 找出目前活動中的 Process       |
| `windows.pstree.PsTree`       | 查看 Process 父子關係        |
| `windows.cmdline.CmdLine`     | 查看 Process 執行參數        |
| `windows.netscan.NetScan`     | 找出有網路連線的 Process       |
| `windows.malfind.Malfind`     | 找出可能被注入的記憶體區段          |
| `windows.vadinfo.VadInfo`     | 查看 Process 的 VAD 記憶體資訊 |
| `windows.dumpfiles.DumpFiles` | Dump 記憶體中的檔案內容         |

---

## 8. 建議分析流程

建議分析流程如下：

```text
windows.info.Info
        ↓
windows.pslist.PsList
        ↓
windows.pstree.PsTree
        ↓
windows.cmdline.CmdLine
        ↓
windows.netscan.NetScan
        ↓
windows.malfind.Malfind
        ↓
windows.memmap.Memmap --pid <可疑 PID>
```

也就是說，先找出可疑行程，再針對特定 PID 使用 `memmap` 進一步分析。

---

## 9. 本次分析判斷

本次如果執行 `windows.memmap.Memmap` 後產生大量結果，屬於正常現象。

因為 `memmap` 會列出大量虛擬記憶體與實體記憶體的對應關係，而 Windows 系統本身與各個 Process 都會產生許多記憶體區段。

因此，本次不建議直接逐行分析全部 `memmap` 結果，而是應該先透過 `pslist`、`pstree`、`cmdline`、`netscan` 或 `malfind` 找出可疑 Process，再針對特定 PID 執行 `memmap`。
