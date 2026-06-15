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

`windows.registry.hivelist.HiveList` 用來列出記憶體中已載入的 Windows Registry Hive。

Registry Hive 是 Windows 登錄檔的主要資料庫，裡面可能包含系統設定、使用者設定、帳號資訊、服務設定、軟體資訊，以及使用者操作紀錄。

在數位鑑識中，`HiveList` 主要用來確認目前系統中有哪些 Registry Hive 被載入，並找出後續分析 Registry 所需要的 Hive 路徑。

---

## 2. 執行指令

```bash
.\vol.exe -f .\OtterCTF.vmem windows.registry.hivelist.HiveList
```

---

## 3. 欄位說明

| 欄位             | 說明                                                                       |
| -------------- | ------------------------------------------------------------------------ |
| `Offset`       | Registry Hive 在記憶體中的位置，可作為識別該 Hive 的參考。                                  |
| `FileFullPath` | Registry Hive 對應的完整路徑，可判斷該 Hive 屬於系統或使用者。                                |
| `File output`  | 是否有將 Hive 匯出成檔案。若顯示 `Disabled`，代表本次只是列出 Hive，沒有 dump 出 Registry Hive 檔案。 |

---

## 4. 執行結果

本次執行結果如下：

```text
Offset          FileFullPath                                                    File output

0xf8a00000f010                                                                  Disabled
0xf8a000024010  \REGISTRY\MACHINE\SYSTEM                                        Disabled
0xf8a000053320  \REGISTRY\MACHINE\HARDWARE                                      Disabled
0xf8a000109410  \SystemRoot\System32\Config\SECURITY                            Disabled
0xf8a00033d410  \Device\HarddiskVolume1\Boot\BCD                                Disabled
0xf8a0005d5010  \SystemRoot\System32\Config\SOFTWARE                            Disabled
0xf8a001495010  \SystemRoot\System32\Config\DEFAULT                             Disabled
0xf8a0016d4010  \SystemRoot\System32\Config\SAM                                 Disabled
0xf8a00175b010  \??\C:\Windows\ServiceProfiles\NetworkService\NTUSER.DAT        Disabled
0xf8a00176e410  \??\C:\Windows\ServiceProfiles\LocalService\NTUSER.DAT          Disabled
0xf8a002090010  \??\C:\Users\Rick\ntuser.dat                                    Disabled
0xf8a0020ad410  \??\C:\Users\Rick\AppData\Local\Microsoft\Windows\UsrClass.dat  Disabled
0xf8a00377d2d0  \??\C:\System Volume Information\Syscache.hve                   Disabled
```

---

## 5. 重要 Hive 說明

| Hive                                                         | 說明                                         |
| ------------------------------------------------------------ | ------------------------------------------ |
| `\REGISTRY\MACHINE\SYSTEM`                                   | 系統設定、控制集、服務與開機相關設定。                        |
| `\REGISTRY\MACHINE\HARDWARE`                                 | 硬體相關資訊。                                    |
| `\SystemRoot\System32\Config\SECURITY`                       | 系統安全性設定與原則。                                |
| `\SystemRoot\System32\Config\SOFTWARE`                       | 已安裝軟體與系統軟體設定。                              |
| `\SystemRoot\System32\Config\SAM`                            | 本機帳號與使用者資訊。                                |
| `\SystemRoot\System32\Config\DEFAULT`                        | 預設使用者設定。                                   |
| `C:\Users\Rick\ntuser.dat`                                   | Rick 使用者個人 Registry Hive，可能包含使用者執行程式與操作紀錄。 |
| `C:\Users\Rick\AppData\Local\Microsoft\Windows\UsrClass.dat` | Rick 使用者 Shell、檔案總管、捷徑與使用者介面相關紀錄。          |
| `Syscache.hve`                                               | 系統快取 Hive，可能包含程式執行或檔案相關快取資訊。               |
| `Boot\BCD`                                                   | Windows 開機設定資料。                            |

---

## 6. 本案重點 Hive

本案最重要的是 Rick 使用者相關 Hive：

```text
0xf8a002090010  \??\C:\Users\Rick\ntuser.dat
0xf8a0020ad410  \??\C:\Users\Rick\AppData\Local\Microsoft\Windows\UsrClass.dat
```

原因是前面分析已經發現多個與 Rick 使用者相關的可疑路徑：

```text
C:\Users\Rick\
C:\Torrents\Rick And Morty season 1 download.exe
C:\Users\Rick\AppData\Local\Temp\RarSFX0\vmware-tray.exe
C:\Users\Rick\Desktop\READ_IT.txt
C:\Users\Rick\AppData\Roaming\Microsoft\Windows\Recent\Flag.txt.WINDOWS.lnk
```

因此，Rick 的 `ntuser.dat` 與 `UsrClass.dat` 可能包含後續分析所需的使用者操作紀錄。

---

## 7. File output 欄位分析

本次結果中的 `File output` 都顯示為：

```text
Disabled
```

這代表本次執行 `HiveList` 時，Volatility 只是列出 Registry Hive，並沒有將 Hive 匯出成檔案。

這不是錯誤，也不影響本次分析。

如果後續需要匯出 Registry Hive，再另外使用 dump 相關參數或其他 Registry 分析工具處理。
