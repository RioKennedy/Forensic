# 測試內容
- .\vol.exe -f .\OtterCTF.vmem windows.registry.printkey.PrintKey


```
D:\Forensic\G140A006\VolatilityWorkbench>.\vol.exe -f .\OtterCTF.vmem windows.registry.printkey.PrintKey
Volatility 3 Framework 2.5.0
Progress:  100.00               PDB scanning finished
Last Write Time Hive Offset     Type    Key     Name    Data    Volatile

2018-08-04 19:25:54.000000      0xf8a00000f010  Key     [NONAME]        A               False
2018-08-04 19:25:54.000000      0xf8a00000f010  Key     [NONAME]        MACHINE         False
2018-08-04 19:25:54.000000      0xf8a00000f010  Key     [NONAME]        USER            False
2018-08-04 19:25:54.000000      0xf8a000024010  Key     \REGISTRY\MACHINE\SYSTEM        ControlSet001            False
2018-08-04 19:25:54.000000      0xf8a000024010  Key     \REGISTRY\MACHINE\SYSTEM        ControlSet002            False
2018-08-04 19:25:54.000000      0xf8a000024010  Key     \REGISTRY\MACHINE\SYSTEM        MountedDevices           False
2018-08-04 19:25:54.000000      0xf8a000024010  Key     \REGISTRY\MACHINE\SYSTEM        RNG     False
2018-08-04 19:25:54.000000      0xf8a000024010  Key     \REGISTRY\MACHINE\SYSTEM        Select  False
2018-08-04 19:25:54.000000      0xf8a000024010  Key     \REGISTRY\MACHINE\SYSTEM        Setup   False
2018-08-04 19:25:54.000000      0xf8a000024010  Key     \REGISTRY\MACHINE\SYSTEM        SoftwareFalse
2018-08-04 19:25:54.000000      0xf8a000024010  Key     \REGISTRY\MACHINE\SYSTEM        WPA     False
2018-08-04 19:25:54.000000      0xf8a000024010  Key     \REGISTRY\MACHINE\SYSTEM        CurrentControlSet                True
2018-08-04 19:25:54.000000      0xf8a000053320  Key     \REGISTRY\MACHINE\HARDWARE      ACPI    False
2018-08-04 19:25:54.000000      0xf8a000053320  Key     \REGISTRY\MACHINE\HARDWARE      DESCRIPTION              False
2018-08-04 19:25:54.000000      0xf8a000053320  Key     \REGISTRY\MACHINE\HARDWARE      DEVICEMAPFalse
2018-08-04 19:25:54.000000      0xf8a000053320  Key     \REGISTRY\MACHINE\HARDWARE      RESOURCEMAP              True
2018-08-04 19:26:14.000000      0xf8a000109410  Key     \SystemRoot\System32\Config\SECURITY    Policy           False
2018-08-04 19:26:14.000000      0xf8a000109410  Key     \SystemRoot\System32\Config\SECURITY    RXACT            False
2018-08-04 19:26:14.000000      0xf8a000109410  Key     \SystemRoot\System32\Config\SECURITY    SAM              True
2018-08-04 19:26:04.000000      0xf8a00033d410  Key     \Device\HarddiskVolume1\Boot\BCD        Description              False
2018-08-04 19:26:04.000000      0xf8a00033d410  Key     \Device\HarddiskVolume1\Boot\BCD        Objects          False
2018-06-02 09:28:52.000000      0xf8a0005d5010  Key     \SystemRoot\System32\Config\SOFTWARE    ATI Technologies         False
2018-06-02 09:28:52.000000      0xf8a0005d5010  Key     \SystemRoot\System32\Config\SOFTWARE    CBSTEST          False
2018-06-02 09:28:52.000000      0xf8a0005d5010  Key     \SystemRoot\System32\Config\SOFTWARE    Classes          False
2018-06-02 09:28:52.000000      0xf8a0005d5010  Key     \SystemRoot\System32\Config\SOFTWARE    Clients          False
2018-06-02 09:28:52.000000      0xf8a0005d5010  Key     \SystemRoot\System32\Config\SOFTWARE    Intel            False
2018-06-02 09:28:52.000000      0xf8a0005d5010  Key     \SystemRoot\System32\Config\SOFTWARE    Microsoft                False
2018-06-02 09:28:52.000000      0xf8a0005d5010  Key     \SystemRoot\System32\Config\SOFTWARE    ODBC             False
2018-06-02 09:28:52.000000      0xf8a0005d5010  Key     \SystemRoot\System32\Config\SOFTWARE    Policies         False
2018-06-02 09:28:52.000000      0xf8a0005d5010  Key     \SystemRoot\System32\Config\SOFTWARE    RegisteredApplications           False
2018-06-02 09:28:52.000000      0xf8a0005d5010  Key     \SystemRoot\System32\Config\SOFTWARE    Sonic            False
2018-06-02 09:28:52.000000      0xf8a0005d5010  Key     \SystemRoot\System32\Config\SOFTWARE    ThinPrint                False
2018-06-02 09:28:52.000000      0xf8a0005d5010  Key     \SystemRoot\System32\Config\SOFTWARE    VMware, Inc.             False
2018-06-02 09:28:52.000000      0xf8a0005d5010  Key     \SystemRoot\System32\Config\SOFTWARE    Wow6432Node              False
2009-07-14 04:57:10.000000      0xf8a001495010  Key     \SystemRoot\System32\Config\DEFAULT     Control Panel            False
2009-07-14 04:57:10.000000      0xf8a001495010  Key     \SystemRoot\System32\Config\DEFAULT     Environment              False
2009-07-14 04:57:10.000000      0xf8a001495010  Key     \SystemRoot\System32\Config\DEFAULT     EUDC             False
2009-07-14 04:57:10.000000      0xf8a001495010  Key     \SystemRoot\System32\Config\DEFAULT     Keyboard Layout          False
2009-07-14 04:57:10.000000      0xf8a001495010  Key     \SystemRoot\System32\Config\DEFAULT     Printers         False
2009-07-14 04:57:10.000000      0xf8a001495010  Key     \SystemRoot\System32\Config\DEFAULT     Software         False
2009-07-14 04:57:10.000000      0xf8a001495010  Key     \SystemRoot\System32\Config\DEFAULT     SYSTEM           False
2009-07-14 04:45:46.000000      0xf8a0016d4010  Key     \SystemRoot\System32\Config\SAM SAM     False
2009-07-14 04:45:47.000000      0xf8a00175b010  Key     \??\C:\Windows\ServiceProfiles\NetworkService\NTUSER.DAT AppEvents               False
2009-07-14 04:45:47.000000      0xf8a00175b010  Key     \??\C:\Windows\ServiceProfiles\NetworkService\NTUSER.DAT Console         False
2009-07-14 04:45:47.000000      0xf8a00175b010  Key     \??\C:\Windows\ServiceProfiles\NetworkService\NTUSER.DAT Control Panel           False
2009-07-14 04:45:47.000000      0xf8a00175b010  Key     \??\C:\Windows\ServiceProfiles\NetworkService\NTUSER.DAT Environment             False
2009-07-14 04:45:47.000000      0xf8a00175b010  Key     \??\C:\Windows\ServiceProfiles\NetworkService\NTUSER.DAT EUDC            False
2009-07-14 04:45:47.000000      0xf8a00175b010  Key     \??\C:\Windows\ServiceProfiles\NetworkService\NTUSER.DAT Keyboard Layout         False
2009-07-14 04:45:47.000000      0xf8a00175b010  Key     \??\C:\Windows\ServiceProfiles\NetworkService\NTUSER.DAT Network         False
2009-07-14 04:45:47.000000      0xf8a00175b010  Key     \??\C:\Windows\ServiceProfiles\NetworkService\NTUSER.DAT Printers                False
2009-07-14 04:45:47.000000      0xf8a00175b010  Key     \??\C:\Windows\ServiceProfiles\NetworkService\NTUSER.DAT Software                False
2009-07-14 04:45:47.000000      0xf8a00175b010  Key     \??\C:\Windows\ServiceProfiles\NetworkService\NTUSER.DAT System          False
2009-07-14 04:45:48.000000      0xf8a00176e410  Key     \??\C:\Windows\ServiceProfiles\LocalService\NTUSER.DAT   AppEvents               False
2009-07-14 04:45:48.000000      0xf8a00176e410  Key     \??\C:\Windows\ServiceProfiles\LocalService\NTUSER.DAT   Console         False
2009-07-14 04:45:48.000000      0xf8a00176e410  Key     \??\C:\Windows\ServiceProfiles\LocalService\NTUSER.DAT   Control Panel           False
2009-07-14 04:45:48.000000      0xf8a00176e410  Key     \??\C:\Windows\ServiceProfiles\LocalService\NTUSER.DAT   Environment             False
2009-07-14 04:45:48.000000      0xf8a00176e410  Key     \??\C:\Windows\ServiceProfiles\LocalService\NTUSER.DAT   EUDC            False
2009-07-14 04:45:48.000000      0xf8a00176e410  Key     \??\C:\Windows\ServiceProfiles\LocalService\NTUSER.DAT   Keyboard Layout         False
2009-07-14 04:45:48.000000      0xf8a00176e410  Key     \??\C:\Windows\ServiceProfiles\LocalService\NTUSER.DAT   Network         False
2009-07-14 04:45:48.000000      0xf8a00176e410  Key     \??\C:\Windows\ServiceProfiles\LocalService\NTUSER.DAT   Printers                False
2009-07-14 04:45:48.000000      0xf8a00176e410  Key     \??\C:\Windows\ServiceProfiles\LocalService\NTUSER.DAT   Software                False
2009-07-14 04:45:48.000000      0xf8a00176e410  Key     \??\C:\Windows\ServiceProfiles\LocalService\NTUSER.DAT   System          False
2018-08-04 19:26:57.000000      0xf8a002090010  Key     \??\C:\Users\Rick\ntuser.dat    AppEventsFalse
2018-08-04 19:26:57.000000      0xf8a002090010  Key     \??\C:\Users\Rick\ntuser.dat    Console False
2018-08-04 19:26:57.000000      0xf8a002090010  Key     \??\C:\Users\Rick\ntuser.dat    Control Panel            False
2018-08-04 19:26:57.000000      0xf8a002090010  Key     \??\C:\Users\Rick\ntuser.dat    Environment              False
2018-08-04 19:26:57.000000      0xf8a002090010  Key     \??\C:\Users\Rick\ntuser.dat    EUDC    False
2018-08-04 19:26:57.000000      0xf8a002090010  Key     \??\C:\Users\Rick\ntuser.dat    Identities               False
2018-08-04 19:26:57.000000      0xf8a002090010  Key     \??\C:\Users\Rick\ntuser.dat    Keyboard Layout          False
2018-08-04 19:26:57.000000      0xf8a002090010  Key     \??\C:\Users\Rick\ntuser.dat    Network False
2018-08-04 19:26:57.000000      0xf8a002090010  Key     \??\C:\Users\Rick\ntuser.dat    PrintersFalse
2018-08-04 19:26:57.000000      0xf8a002090010  Key     \??\C:\Users\Rick\ntuser.dat    SoftwareFalse
2018-08-04 19:26:57.000000      0xf8a002090010  Key     \??\C:\Users\Rick\ntuser.dat    System  False
2018-08-04 19:26:57.000000      0xf8a002090010  Key     \??\C:\Users\Rick\ntuser.dat    Volatile Environment             True
2018-07-07 10:23:46.000000      0xf8a0020ad410  Key     \??\C:\Users\Rick\AppData\Local\Microsoft\Windows\UsrClass.dat   .btapp          False
2018-07-07 10:23:46.000000      0xf8a0020ad410  Key     \??\C:\Users\Rick\AppData\Local\Microsoft\Windows\UsrClass.dat   .btinstall              False
2018-07-07 10:23:46.000000      0xf8a0020ad410  Key     \??\C:\Users\Rick\AppData\Local\Microsoft\Windows\UsrClass.dat   .btkey          False
2018-07-07 10:23:46.000000      0xf8a0020ad410  Key     \??\C:\Users\Rick\AppData\Local\Microsoft\Windows\UsrClass.dat   .btsearch               False
2018-07-07 10:23:46.000000      0xf8a0020ad410  Key     \??\C:\Users\Rick\AppData\Local\Microsoft\Windows\UsrClass.dat   .btskin         False
2018-07-07 10:23:46.000000      0xf8a0020ad410  Key     \??\C:\Users\Rick\AppData\Local\Microsoft\Windows\UsrClass.dat   .htm            False
2018-07-07 10:23:46.000000      0xf8a0020ad410  Key     \??\C:\Users\Rick\AppData\Local\Microsoft\Windows\UsrClass.dat   .html           False
2018-07-07 10:23:46.000000      0xf8a0020ad410  Key     \??\C:\Users\Rick\AppData\Local\Microsoft\Windows\UsrClass.dat   .shtml          False
2018-07-07 10:23:46.000000      0xf8a0020ad410  Key     \??\C:\Users\Rick\AppData\Local\Microsoft\Windows\UsrClass.dat   .torrent                False
2018-07-07 10:23:46.000000      0xf8a0020ad410  Key     \??\C:\Users\Rick\AppData\Local\Microsoft\Windows\UsrClass.dat   .xht            False
2018-07-07 10:23:46.000000      0xf8a0020ad410  Key     \??\C:\Users\Rick\AppData\Local\Microsoft\Windows\UsrClass.dat   .xhtml          False
2018-07-07 10:23:46.000000      0xf8a0020ad410  Key     \??\C:\Users\Rick\AppData\Local\Microsoft\Windows\UsrClass.dat   Applications            False
2018-07-07 10:23:46.000000      0xf8a0020ad410  Key     \??\C:\Users\Rick\AppData\Local\Microsoft\Windows\UsrClass.dat   BitTorrent              False
2018-07-07 10:23:46.000000      0xf8a0020ad410  Key     \??\C:\Users\Rick\AppData\Local\Microsoft\Windows\UsrClass.dat   FalconBetaAccount               False
2018-07-07 10:23:46.000000      0xf8a0020ad410  Key     \??\C:\Users\Rick\AppData\Local\Microsoft\Windows\UsrClass.dat   ftp             False
2018-07-07 10:23:46.000000      0xf8a0020ad410  Key     \??\C:\Users\Rick\AppData\Local\Microsoft\Windows\UsrClass.dat   http            False
2018-07-07 10:23:46.000000      0xf8a0020ad410  Key     \??\C:\Users\Rick\AppData\Local\Microsoft\Windows\UsrClass.dat   https           False
2018-07-07 10:23:46.000000      0xf8a0020ad410  Key     \??\C:\Users\Rick\AppData\Local\Microsoft\Windows\UsrClass.dat   Local Settings          False
2018-07-07 10:23:46.000000      0xf8a0020ad410  Key     \??\C:\Users\Rick\AppData\Local\Microsoft\Windows\UsrClass.dat   Magnet          False
2018-07-07 10:23:46.000000      0xf8a0020ad410  Key     \??\C:\Users\Rick\AppData\Local\Microsoft\Windows\UsrClass.dat   MIME            False
2018-07-07 10:23:46.000000      0xf8a0020ad410  Key     \??\C:\Users\Rick\AppData\Local\Microsoft\Windows\UsrClass.dat   Software                False
2018-07-07 10:23:46.000000      0xf8a0020ad410  Key     \??\C:\Users\Rick\AppData\Local\Microsoft\Windows\UsrClass.dat   VirtualStore            False
2018-08-04 19:33:07.000000      0xf8a00377d2d0  Key     \??\C:\System Volume Information\Syscache.hve    DefaultObjectStore              False
```


# windows.registry.printkey.PrintKey 分析

## 1. Plugin 功能說明

`windows.registry.printkey.PrintKey` 用來讀取並列出 Registry Hive 中的 Key 與 Value。

在數位鑑識中，`PrintKey` 可用來分析系統設定、使用者設定、軟體關聯、檔案副檔名關聯、服務設定與使用者操作痕跡。

本次分析主要用來確認 Rick 使用者的 Registry Key，以及是否存在與 BitTorrent、torrent 檔案或可疑程式相關的登錄紀錄。

---

## 2. 執行指令

```bash id="xkeg6s"
.\vol.exe -f .\OtterCTF.vmem windows.registry.printkey.PrintKey
```

---

## 3. 欄位說明

| 欄位                | 說明                                          |
| ----------------- | ------------------------------------------- |
| `Last Write Time` | Registry Key 最後寫入時間，可用來判斷該 Key 最近被修改或建立的時間。 |
| `Hive Offset`     | Registry Hive 在記憶體中的位置。                     |
| `Type`            | Registry 物件類型，例如 `Key`。                     |
| `Key`             | Registry Hive 或 Registry 路徑。                |
| `Name`            | 該 Registry Key 底下的子 Key 或 Value 名稱。         |
| `Data`            | Value 的資料內容。若為 Key，通常沒有資料內容。                |
| `Volatile`        | 是否為暫時性 Registry Key。`True` 代表重開機後可能不保留。     |

---

## 4. 執行結果重點

本次 `PrintKey` 列出多個系統與使用者 Registry Hive 的 Key，包含：

```text id="356anl"
\REGISTRY\MACHINE\SYSTEM
\REGISTRY\MACHINE\HARDWARE
\SystemRoot\System32\Config\SECURITY
\SystemRoot\System32\Config\SOFTWARE
\SystemRoot\System32\Config\SAM
\SystemRoot\System32\Config\DEFAULT
\??\C:\Users\Rick\ntuser.dat
\??\C:\Users\Rick\AppData\Local\Microsoft\Windows\UsrClass.dat
\??\C:\System Volume Information\Syscache.hve
```

其中本案最重要的是 Rick 使用者相關 Registry：

```text id="n0mk16"
\??\C:\Users\Rick\ntuser.dat
\??\C:\Users\Rick\AppData\Local\Microsoft\Windows\UsrClass.dat
```

---

## 5. Rick 使用者 Registry 發現

在 `C:\Users\Rick\ntuser.dat` 中，發現多個使用者 Registry Key：

```text id="9lkljg"
AppEvents
Console
Control Panel
Environment
EUDC
Identities
Keyboard Layout
Network
Printers
Software
System
Volatile Environment
```

這代表 Rick 使用者的個人 Registry Hive 已載入記憶體中，可作為後續分析使用者操作紀錄的來源。

其中 `Volatile Environment` 顯示為 `True`，代表這是暫時性的使用者環境資訊。

---

## 6. UsrClass.dat 發現

在 Rick 的 `UsrClass.dat` 中，發現多個與檔案關聯與應用程式相關的 Key：

```text id="r7vbti"
.btapp
.btinstall
.btkey
.btsearch
.btskin
.torrent
Applications
BitTorrent
Magnet
http
https
VirtualStore
```

這些項目具有鑑識意義，尤其是：

```text id="s4kc1e"
.torrent
BitTorrent
Magnet
```

這代表系統中存在與 torrent 檔案、BitTorrent 應用程式，以及 Magnet 連結相關的登錄紀錄。

---

## 7. 與前面證據的關聯

前面分析已經發現：

```text id="lm4l3i"
BitTorrent.exe
bittorrentie.exe
Rick And Morty season 1 download.exe.torrent
\Torrents\Rick And Morty season 1 download.exe
```

本次 `PrintKey` 又在 `UsrClass.dat` 中發現：

```text id="onab8s"
.torrent
BitTorrent
Magnet
```

因此，Registry 結果可以補強前面 FileScan、CmdLine、PsList 與 NetScan 的分析，證明這台主機確實存在 BitTorrent / torrent 使用痕跡。

---

## 8. Syscache.hve 發現

結果中也出現：

```text id="qkmjww"
\??\C:\System Volume Information\Syscache.hve
```

其 Last Write Time 為：

```text id="n5xpqp"
2018-08-04 19:33:07
```

此時間接近事件發生與記憶體擷取時間，因此可作為輔助參考。

不過本次輸出只看到 `DefaultObjectStore`，尚未直接看到與可疑執行檔名稱相關的資料，因此不作為主要證據。

---

## 9. 鑑識判斷

本次 `PrintKey` 結果支持以下判斷：

```text id="nlpxhn"
1. Rick 使用者 Registry Hive 已載入記憶體。
2. Rick 使用者環境中存在 BitTorrent / torrent / Magnet 相關 Registry Key。
3. Registry 結果與前面 BitTorrent 程序、torrent 檔案與可疑下載檔案互相補強。
4. 目前 PrintKey 尚未直接證明 Rick And Morty season 1 download.exe 被執行，但可以證明 torrent 關聯環境存在。
```

---

## 10. 結論

`windows.registry.printkey.PrintKey` 成功列出系統與 Rick 使用者相關的 Registry Key。

本次最重要的發現是 Rick 的 `UsrClass.dat` 中存在：

```text id="u4bj9j"
.torrent
BitTorrent
Magnet
```

這些 Registry Key 可補強本案中 BitTorrent 下載活動的證據。

結合前面發現的 `.torrent` 檔案、BitTorrent 連線與 `Rick And Morty season 1 download.exe`，可以推論可疑程式很可能與 torrent 下載活動有關。

不過，`PrintKey` 本身只能證明 Registry 中存在相關 Key，尚不能單獨證明可疑程式已被執行。

下一步應使用 `windows.registry.userassist.UserAssist` 來確認使用者是否曾執行相關程式。
