# 測試內容

- .\vol.exe -f .\OtterCTF.vmem windows.registry.hivelist.HiveList

```
D:\Forensic\G140A006\VolatilityWorkbench>.\vol.exe -f .\OtterCTF.vmem windows.callbacks.Callbacks
Volatility 3 Framework 2.5.0
Progress:  100.00               PDB scanning finished
Type    Callback        Module  Symbol  Detail

PspLoadImageNotifyRoutine       0xf80002deecc0  ntoskrnl        EtwpTraceLoadImage      N/A
PspCreateProcessNotifyRoutine   0xf80002a9daf0  ntoskrnl        ViCreateProcessCallback N/A
PspCreateProcessNotifyRoutine   0xf880012121e0  ksecdd  -       N/A
PspCreateProcessNotifyRoutine   0xf880014803d0  cng     -       N/A
PspCreateProcessNotifyRoutine   0xf880016b93c0  tcpip   -       N/A
PspCreateProcessNotifyRoutine   0xf88000cf7ba0  CI      MiPurgeImageSection     N/A
PspCreateProcessNotifyRoutine   0xf880034c3d2c  peauth  -       N/A
KeBugCheckCallbackListHead      0xf88001526b00  ndis    -       Ndis miniport
KeBugCheckCallbackListHead      0xf88001526b00  ndis    -       Ndis miniport
KeBugCheckCallbackListHead      0xf88001526b00  ndis    -       Ndis miniport
KeBugCheckCallbackListHead      0xf88001526b00  ndis    -       Ndis miniport
KeBugCheckCallbackListHead      0xf88001526b00  ndis    -       Ndis miniport
KeBugCheckCallbackListHead      0xf80002a1c02c  hal     -       ACPI x64 platform
KeBugCheckReasonCallbackListHead        0xf88000f74054  Wdf01000        -       -
KeBugCheckReasonCallbackListHead        0xf88000f74054  Wdf01000        -       -
KeBugCheckReasonCallbackListHead        0xf88004530c58  BthEnum -       -
KeBugCheckReasonCallbackListHead        0xf88004519970  rfcomm  -       -
KeBugCheckReasonCallbackListHead        0xf880044d1228  bthport -       -
KeBugCheckReasonCallbackListHead        0xf8800438ee98  BTHUSB  -       -
KeBugCheckReasonCallbackListHead        0xf88004370f40  mouhid  -       -
KeBugCheckReasonCallbackListHead        0xf88004356d84  HIDCLASS        -       -
KeBugCheckReasonCallbackListHead        0xf88004341d70  hidusb  -       -
KeBugCheckReasonCallbackListHead        0xf880042d7204  crashdmp        -       -
KeBugCheckReasonCallbackListHead        0xf88003fbf738  usbhub  -       -
KeBugCheckReasonCallbackListHead        0xf88003fbf6dc  usbhub  -       -
KeBugCheckReasonCallbackListHead        0xf88000f74054  Wdf01000        -       -
KeBugCheckReasonCallbackListHead        0xf88000f74054  Wdf01000        -       -
KeBugCheckReasonCallbackListHead        0xf88000f74054  Wdf01000        -       -
KeBugCheckReasonCallbackListHead        0xf88000f74054  Wdf01000        -       -
KeBugCheckReasonCallbackListHead        0xf88003c6d2d8  USBPORT -       -
KeBugCheckReasonCallbackListHead        0xf88003c6d3b4  USBPORT -       -
KeBugCheckReasonCallbackListHead        0xf88003c6d348  USBPORT -       -
KeBugCheckReasonCallbackListHead        0xf88003cf9f3c  dxgkrnl -       -
KeBugCheckReasonCallbackListHead        0xf88003b9b51c  mouclass        -       -
KeBugCheckReasonCallbackListHead        0xf88003b84828  kbdclass        -       -
KeBugCheckReasonCallbackListHead        0xf88003b6dcf4  i8042prt        -       -
KeBugCheckReasonCallbackListHead        0xf88003a7211c  mssmbios        -       -
KeBugCheckReasonCallbackListHead        0xf88003a720d4  mssmbios        -       -
KeBugCheckReasonCallbackListHead        0xf88003a72034  mssmbios        -       -
KeBugCheckReasonCallbackListHead        0xf88003a71ff0  mssmbios        -       -
KeBugCheckReasonCallbackListHead        0xf8800108b620  VIDEOPRT        -       -
KeBugCheckReasonCallbackListHead        0xf88000f74054  Wdf01000        -       -
KeBugCheckReasonCallbackListHead        0xf8800106bcf4  cdrom   -       -
KeBugCheckReasonCallbackListHead        0xf8800199dd70  CLASSPNP        -       -
KeBugCheckReasonCallbackListHead        0xf88000f74054  Wdf01000        -       -
KeBugCheckReasonCallbackListHead        0xf88000f74054  Wdf01000        -       -
KeBugCheckReasonCallbackListHead        0xf88000f74054  Wdf01000        -       -
KeBugCheckReasonCallbackListHead        0xf88000f7433c  Wdf01000        -       -
KeBugCheckReasonCallbackListHead        0xf880010b00dc  ataport -       -

```

# windows.callbacks.Callbacks 分析

## 1. Plugin 功能說明

`windows.callbacks.Callbacks` 用來列出 Windows Kernel 中註冊的 Callback 函式。

Callback 是核心或驅動程式向 Windows 註冊的通知機制，例如：

```text id="rajnga"
Process 建立通知
Image 載入通知
BugCheck 當機回呼
Kernel 事件通知
```

在惡意程式或 Rootkit 分析中，攻擊者可能會註冊惡意 Callback，用來監控 Process 建立、DLL 載入，或干擾系統行為。

因此，此 Plugin 可用來檢查是否存在可疑 Kernel Callback 或可疑 Driver Hook。

---

## 2. 執行指令

```bash id="zaqdr5"
.\vol.exe -f .\OtterCTF.vmem windows.callbacks.Callbacks
```

---

## 3. 欄位說明

| 欄位         | 說明               |
| ---------- | ---------------- |
| `Type`     | Callback 類型      |
| `Callback` | Callback 函式位址    |
| `Module`   | Callback 所屬模組或驅動 |
| `Symbol`   | 對應的函式名稱          |
| `Detail`   | 其他細節說明           |

---

## 4. 執行結果摘要

本次結果中主要看到以下 Callback 類型：

```text id="m3m9go"
PspLoadImageNotifyRoutine
PspCreateProcessNotifyRoutine
KeBugCheckCallbackListHead
KeBugCheckReasonCallbackListHead
```

其中出現的模組包含：

```text id="7ea13i"
ntoskrnl
ksecdd
cng
tcpip
CI
peauth
ndis
hal
Wdf01000
BthEnum
rfcomm
bthport
BTHUSB
mouhid
HIDCLASS
hidusb
crashdmp
usbhub
USBPORT
dxgkrnl
mouclass
kbdclass
i8042prt
mssmbios
VIDEOPRT
cdrom
CLASSPNP
ataport
```

這些大多屬於 Windows 系統核心、網路、藍牙、USB、鍵盤滑鼠、顯示、磁碟與硬體相關的正常驅動模組。

---

## 5. 重要結果分析

### 5.1 Process / Image 相關 Callback

本次結果中出現：

```text id="7hpyhj"
PspLoadImageNotifyRoutine
PspCreateProcessNotifyRoutine
```

這類 Callback 通常用來監控：

```text id="ee97yl"
Process 建立
Image / DLL 載入
系統核心事件通知
```

結果中對應的模組包含：

```text id="o9nhh0"
ntoskrnl
ksecdd
cng
tcpip
CI
peauth
```

這些都屬於 Windows 正常核心元件或系統安全相關模組，沒有看到明顯陌生或可疑的 Driver 名稱。

---

### 5.2 BugCheck 相關 Callback

結果中也有大量：

```text id="8i50w9"
KeBugCheckCallbackListHead
KeBugCheckReasonCallbackListHead
```

這類 Callback 主要與系統當機、藍屏、硬體或驅動錯誤時的資訊記錄有關。

出現的模組包含：

```text id="uft6d0"
ndis
hal
Wdf01000
USBPORT
usbhub
mouclass
kbdclass
dxgkrnl
CLASSPNP
ataport
```

這些大多是正常 Windows 驅動或硬體相關模組，未發現明顯異常。

---

## 6. 鑑識判斷

本次 `Callbacks` 結果沒有看到以下可疑情況：

```text id="ij21hl"
未知 Driver 註冊 Callback
可疑模組名稱
明顯非 Windows 系統路徑的 Kernel Callback
Rootkit 常見 Hook 痕跡
與 Rick And Morty 或 vmware-tray.exe 相關的核心 Callback
```

因此，目前沒有證據顯示本案存在 Kernel Callback Hook 或 Rootkit 行為。

---

## 7. 與本案關聯

本案主要證據集中於 User-mode 執行鏈：

```text id="jmt3ow"
BitTorrent 下載活動
Rick And Morty season 1 download.exe
Temp\RarSFX0\vmware-tray.exe
Malfind / VadInfo 可疑記憶體區段
READ_IT.txt 加密提示檔
```

而 `Callbacks` 主要檢查 Kernel 層級行為。

本次沒有發現可疑 Kernel Callback，因此可判斷本案目前較不像是 Kernel Rootkit 或 Driver 層攻擊，而是使用者執行可疑 EXE 後造成的 User-mode 感染與加密行為。

---

## 8. 結論

`windows.callbacks.Callbacks` 成功列出系統中的 Kernel Callback。

本次結果中出現的 Callback 多數屬於 Windows 正常核心、硬體、USB、網路與驅動相關模組，例如：

```text id="tu2shg"
ntoskrnl
ksecdd
tcpip
CI
peauth
ndis
Wdf01000
USBPORT
CLASSPNP
ataport
```

未發現明顯可疑或未知的 Kernel Callback。

因此，此 Plugin 結果可作為排除證據，表示目前沒有發現 Kernel Callback Hook 或 Rootkit 層級攻擊跡象。

本案重點仍應放在：

```text id="6xzjvq"
Rick 使用者執行可疑 Torrent EXE
Rick And Morty 啟動 vmware-tray.exe
vmware-tray.exe 出現可疑記憶體區段
READ_IT.txt 顯示檔案遭加密
```
