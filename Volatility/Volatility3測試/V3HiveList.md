# 測試內容
- vol.exe -f .\OtterCTF.vmem windows.registry.hivelist.HiveList

```
D:\Forensic\G140A006\VolatilityWorkbench>.\vol.exe -f .\OtterCTF.vmem windows.registry.hivelist.HiveList
Volatility 3 Framework 2.5.0
Progress:  100.00               PDB scanning finished
Offset  FileFullPath    File output

0xf8a00000f010          Disabled
0xf8a000024010  \REGISTRY\MACHINE\SYSTEM        Disabled
0xf8a000053320  \REGISTRY\MACHINE\HARDWARE      Disabled
0xf8a000109410  \SystemRoot\System32\Config\SECURITY    Disabled
0xf8a00033d410  \Device\HarddiskVolume1\Boot\BCD        Disabled
0xf8a0005d5010  \SystemRoot\System32\Config\SOFTWARE    Disabled
0xf8a001495010  \SystemRoot\System32\Config\DEFAULT     Disabled
0xf8a0016d4010  \SystemRoot\System32\Config\SAM Disabled
0xf8a00175b010  \??\C:\Windows\ServiceProfiles\NetworkService\NTUSER.DAT        Disabled
0xf8a00176e410  \??\C:\Windows\ServiceProfiles\LocalService\NTUSER.DAT  Disabled
0xf8a002090010  \??\C:\Users\Rick\ntuser.dat    Disabled
0xf8a0020ad410  \??\C:\Users\Rick\AppData\Local\Microsoft\Windows\UsrClass.dat  Disabled
0xf8a00377d2d0  \??\C:\System Volume Information\Syscache.hve   Disabled
```


# windows.registry.hivelist.HiveList 分析

## 1. Plugin 功能說明

`windows.registry.hivelist.HiveList` 用來列出記憶體中載入的 Windows Registry Hive。

Registry Hive 是 Windows 系統的重要設定資料庫，包含系統設定、使用者設定、服務資訊、帳號資訊，以及使用者操作痕跡。

此 Plugin 可協助確認系統中有哪些 Registry Hive 被載入，並找出後續 Registry 分析所需的 Hive 路徑。

---

## 2. 執行指令

```bash
.\vol.exe -f .\OtterCTF.vmem windows.registry.hivelist.HiveList
```

---

## 3. 執行結果重點

本次掃描發現多個 Registry Hive，包含：

```text
\REGISTRY\MACHINE\SYSTEM
\REGISTRY\MACHINE\HARDWARE
\SystemRoot\System32\Config\SECURITY
\SystemRoot\System32\Config\SOFTWARE
\SystemRoot\System32\Config\DEFAULT
\SystemRoot\System32\Config\SAM
\??\C:\Users\Rick\ntuser.dat
\??\C:\Users\Rick\AppData\Local\Microsoft\Windows\UsrClass.dat
\??\C:\System Volume Information\Syscache.hve
```

其中最重要的是：

```text
0xf8a002090010  \??\C:\Users\Rick\ntuser.dat
0xf8a0020ad410  \??\C:\Users\Rick\AppData\Local\Microsoft\Windows\UsrClass.dat
```

---

## 4. 重要 Hive 分析

| Hive                | 用途                            |
| ------------------- | ----------------------------- |
| `SYSTEM`            | 系統服務、控制集、硬體與開機設定              |
| `SOFTWARE`          | 已安裝軟體、Windows 系統軟體設定          |
| `SAM`               | 本機帳號資訊                        |
| `SECURITY`          | 安全性原則與憑證相關資訊                  |
| `Rick\ntuser.dat`   | Rick 使用者個人 Registry 設定與操作紀錄   |
| `Rick\UsrClass.dat` | Rick 使用者 Shell、檔案總管與使用者介面相關紀錄 |

---

## 5. 鑑識判斷

本次 `HiveList` 確認系統中存在使用者 `Rick` 的 Registry Hive：

```text
\??\C:\Users\Rick\ntuser.dat
\??\C:\Users\Rick\AppData\Local\Microsoft\Windows\UsrClass.dat
```

這與前面發現的可疑檔案路徑一致：

```text
C:\Users\Rick\
C:\Torrents\
C:\Users\Rick\AppData\Local\Temp\RarSFX0\
```

因此，後續可針對 Rick 使用者 Registry 進行分析，以確認是否有程式執行紀錄、近期檔案開啟紀錄或使用者操作痕跡。

---

## 6. File output 欄位說明

本次結果中的 `File output` 顯示為：

```text
Disabled
```

這代表本次只是列出 Hive，沒有將 Registry Hive dump 成檔案。

這不是錯誤，不影響 `HiveList` 的分析結果。

---

## 7. 結論

`windows.registry.hivelist.HiveList` 成功列出系統與使用者 Registry Hive。

其中 `C:\Users\Rick\ntuser.dat` 與 `UsrClass.dat` 是後續分析的重點，因為它們可能包含 Rick 使用者執行程式與操作檔案的紀錄。

下一步應針對 `UserAssist` 進行分析，以確認可疑程式是否曾被 Rick 使用者執行。
