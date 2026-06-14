# 測試內容
- vol.exe -f .\OtterCTF.vmem windows.mftscan.MftScan
```
D:\Forensic\G140A006\VolatilityWorkbench>.\vol.exe -f .\OtterCTF.vmem windows.mftscan.MFTScan
Volatility 3 Framework 2.5.0
Progress:  100.00               PDB scanning finished
Offset  Record Type     Record Number   Link Count      MFT Type        Permissions     Attribute Type   Created Modified        Updated Accessed        Filename

0xf88008155050  FILE    38724   2       File    N/A     STANDARD_INFORMATION    2009-07-13 23:42:38.000000       2009-07-14 01:16:20.000000      2018-06-02 20:20:29.000000      2009-07-13 23:42:38.000000       N/A
* 0xf880081550b0        FILE    38724   2       File    Archive FILE_NAME       2018-06-02 20:20:26.000000       2018-06-02 20:20:26.000000      2018-06-02 20:20:26.000000      2018-06-02 20:20:26.000000       wshext.dll
* 0xf88008155120        FILE    38724   2       File    Archive FILE_NAME       2018-06-02 20:20:26.000000       2018-06-02 20:20:26.000000      2018-06-02 20:20:26.000000      2018-06-02 20:20:26.000000       wshext.dll
0xf88008155450  FILE    38725   2       File    N/A     STANDARD_INFORMATION    2009-07-13 23:12:08.000000       2009-07-14 01:16:20.000000      2018-06-02 20:20:29.000000      2009-07-13 23:12:08.000000       N/A
* 0xf880081554b0        FILE    38725   2       File    Archive FILE_NAME       2018-06-02 20:20:26.000000       2018-06-02 20:20:26.000000      2018-06-02 20:20:26.000000      2018-06-02 20:20:26.000000       wship6.dll
* 0xf88008155520        FILE    38725   2       File    Archive FILE_NAME       2018-06-02 20:20:26.000000       2018-06-02 20:20:26.000000      2018-06-02 20:20:26.000000      2018-06-02 20:20:26.000000       wship6.dll
0xf88008155850  FILE    38726   2       File    N/A     STANDARD_INFORMATION    2009-07-14 02:59:34.000000       2009-07-14 02:58:55.000000      2018-06-02 20:20:29.000000      2009-07-14 02:58:55.000000       N/A
* 0xf880081558b0        FILE    38726   2       File    Archive FILE_NAME       2018-06-02 20:20:26.000000       2018-06-02 20:20:26.000000      2018-06-02 20:20:26.000000      2018-06-02 20:20:26.000000       x86_microsoft-windows-winsock-helper-tcpip_31bf3856ad364e35_6.1.7600.16385_none_cb895be592db1acb_wship6.dll_db4127c3
* 0xf880081559f8        FILE    38726   2       File    Archive FILE_NAME       2018-06-02 20:20:26.000000       2018-06-02 20:20:26.000000      2018-06-02 20:20:26.000000      2018-06-02 20:20:26.000000       X845BB~1.DLL
0xf88008155c50  FILE    38727   2       File    N/A     STANDARD_INFORMATION    2010-11-21 03:24:33.000000       2010-11-21 03:24:33.000000      2018-06-02 20:20:29.000000      2010-11-21 03:24:33.000000       N/A
* 0xf88008155cb0        FILE    38727   2       File    Archive FILE_NAME       2018-06-02 20:20:26.000000       2018-06-02 20:20:26.000000      2018-06-02 20:20:26.000000      2018-06-02 20:20:26.000000       wshirda.dll
* 0xf88008155d20        FILE    38727   2       File    Archive FILE_NAME       2018-06-02 20:20:26.000000       2018-06-02 20:20:26.000000      2018-06-02 20:20:26.000000      2018-06-02 20:20:26.000000       wshirda.dll
0xf88008159050  FILE    39880   3       File    N/A     STANDARD_INFORMATION    2010-11-21 07:06:17.000000       2010-11-21 07:06:17.000000      2018-06-02 20:20:33.000000      2010-11-21 07:06:17.000000       N/A
* 0xf880081590b0        FILE    39880   3       File    Archive FILE_NAME       2018-06-02 20:20:33.000000       2018-06-02 20:20:33.000000      2018-06-02 20:20:33.000000      2018-06-02 20:20:33.000000       TYPEPE~1.MUI
* 0xf88008159128        FILE    39880   3       File    Archive FILE_NAME       2018-06-02 20:20:33.000000       2018-06-02 20:20:33.000000      2018-06-02 20:20:33.000000      2018-06-02 20:20:33.000000       typeperf.exe.mui
* 0xf880081591a8        FILE    39880   3       File    Archive FILE_NAME       2018-06-02 20:20:33.000000       2018-06-02 20:20:33.000000      2018-06-02 20:20:33.000000      2018-06-02 20:20:33.000000       typeperf.exe.mui
0xf88008159450  FILE    39881   3       File    N/A     STANDARD_INFORMATION    2010-11-21 07:06:20.000000       2010-11-21 07:06:20.000000      2018-06-02 20:20:33.000000      2010-11-21 07:06:20.000000       N/A
* 0xf880081594b0        FILE    39881   3       File    Archive FILE_NAME       2018-06-02 20:20:33.000000       2018-06-02 20:20:33.000000      2018-06-02 20:20:33.000000      2018-06-02 20:20:33.000000       tzres.dll.mui
* 0xf88008159528        FILE    39881   3       File    Archive FILE_NAME       2018-06-02 20:20:33.000000       2018-06-02 20:20:33.000000      2018-06-02 20:20:33.000000      2018-06-02 20:20:33.000000       TZRESD~1.MUI
* 0xf880081595a0        FILE    39881   3       File    Archive FILE_NAME       2018-06-02 20:20:33.000000       2018-06-02 20:20:33.000000      2018-06-02 20:20:33.000000      2018-06-02 20:20:33.000000       tzres.dll.mui
0xf88008159850  FILE    39882   3       File    N/A     STANDARD_INFORMATION    2010-11-21 07:06:20.000000       2010-11-21 07:06:20.000000      2018-06-02 20:20:33.000000      2010-11-21 07:06:20.000000       N/A
* 0xf880081598b0        FILE    39882   3       File    Archive FILE_NAME       2018-06-02 20:20:33.000000       2018-06-02 20:20:33.000000      2018-06-02 20:20:33.000000      2018-06-02 20:20:33.000000       TZUTIL~1.MUI
* 0xf88008159928        FILE    39882   3       File    Archive FILE_NAME       2018-06-02 20:20:33.000000       2018-06-02 20:20:33.000000      2018-06-02 20:20:33.000000      2018-06-02 20:20:33.000000       tzutil.exe.mui
* 0xf880081599a0        FILE    39882   3       File    Archive FILE_NAME       2018-06-02 20:20:33.000000       2018-06-02 20:20:33.000000      2018-06-02 20:20:33.000000      2018-06-02 20:20:33.000000       tzutil.exe.mui
0xf88008159c50  FILE    39883   3       File    N/A     STANDARD_INFORMATION    2010-11-21 07:06:18.000000       2010-11-21 07:06:18.000000      2018-06-02 20:20:33.000000      2010-11-21 07:06:19.000000       N/A
* 0xf88008159cb0        FILE    39883   3       File    Archive FILE_NAME       2018-06-02 20:20:33.000000       2018-06-02 20:20:33.000000      2018-06-02 20:20:33.000000      2018-06-02 20:20:33.000000       ubpm.dll.mui
* 0xf88008159d28        FILE    39883   3       File    Archive FILE_NAME       2018-06-02 20:20:33.000000       2018-06-02 20:20:33.000000      2018-06-02 20:20:33.000000      2018-06-02 20:20:33.000000       UBPMDL~1.MUI
* 0xf88008159da0        FILE    39883   3       File    Archive FILE_NAME       2018-06-02 20:20:33.000000       2018-06-02 20:20:33.000000      2018-06-02 20:20:33.000000      2018-06-02 20:20:33.000000       ubpm.dll.muiTraceback
...
....
.....
```


- vol.exe -f .\OtterCTF.vmem windows.mftscan.MftScan | findstr "Flag READ_IT"
```
D:\Forensic\G140A006\VolatilityWorkbench>.\vol.exe -f .\OtterCTF.vmem windows.mftscan.MFTScan | findstr "Flag READ_IT"
* 0xf98001ca1d280       FILE    62343can2ing finFiled   Archive FILE_NAME       2018-08-04 19:34:11.000000       2018-08-04 19:34:11.000000      2018-08-04 19:34:11.000000      2018-08-04 19:34:11.000000       Flag.txt.WINDOWS.lnk
```

- vol.exe -f .\OtterCTF.vmem windows.mftscan.MftScan | findstr "Rick Morty"
```
D:\Forensic\G140A006\VolatilityWorkbench>.\vol.exe -f .\OtterCTF.vmem windows.mftscan.MFTScan | findstr "Rick Morty"
* 0xf980011349280       FILE    60114can2ing finFiled   Archive FILE_NAME       2018-07-31 20:54:11.000000       2018-07-31 20:54:11.000000      2018-07-31 20:54:11.000000      2018-07-31 20:54:11.000000       Rick And Morty season 1 download.lnk
```
# windows.mftscan.MFTScan 分析

## 1. Plugin 功能說明

`windows.mftscan.MFTScan` 用來掃描記憶體中的 NTFS MFT（Master File Table）紀錄。

MFT 是 NTFS 檔案系統中用來記錄檔案與資料夾資訊的重要結構，包含檔名、時間戳記、檔案屬性與紀錄編號等資訊。

此 Plugin 可用來確認：

```text
檔案是否曾存在於檔案系統中
檔案建立、修改、更新、存取時間
檔案名稱與 MFT Record Number
是否有捷徑檔、可疑檔案或使用者操作痕跡
```

---

## 2. Plugin 欄位說明

| 欄位               | 說明                                             |
| ---------------- | ---------------------------------------------- |
| `Offset`         | MFT 紀錄在記憶體中的位置                                 |
| `Record Type`    | 紀錄類型，例如 FILE                                   |
| `Record Number`  | MFT Record 編號                                  |
| `Link Count`     | 硬連結數量                                          |
| `MFT Type`       | MFT 類型，例如 File                                 |
| `Permissions`    | 檔案權限或屬性                                        |
| `Attribute Type` | MFT 屬性類型，例如 `STANDARD_INFORMATION`、`FILE_NAME` |
| `Created`        | 建立時間                                           |
| `Modified`       | 修改時間                                           |
| `Updated`        | MFT 紀錄更新時間                                     |
| `Accessed`       | 存取時間                                           |
| `Filename`       | 檔案名稱                                           |

---

## 3. 執行方式

原始執行指令如下：

```bash
.\vol.exe -f .\OtterCTF.vmem windows.mftscan.MFTScan
```

由於 `MFTScan` 輸出內容非常多，因此本次不逐筆分析所有 MFT 紀錄，而是使用 `findstr` 針對案件關鍵字進行篩選。

---

## 4. Flag 相關紀錄

### 執行指令

```bash
.\vol.exe -f .\OtterCTF.vmem windows.mftscan.MFTScan | findstr "Flag READ_IT"
```

### 結果

```text
* 0xf98001ca1d280  FILE  62343  ...  FILE_NAME  2018-08-04 19:34:11  2018-08-04 19:34:11  2018-08-04 19:34:11  2018-08-04 19:34:11  Flag.txt.WINDOWS.lnk
```

### 分析

`MFTScan` 找到 `Flag.txt.WINDOWS.lnk`，代表該捷徑檔曾存在於 NTFS 檔案系統中。

此檔案時間為：

| 時間欄位     | 時間                    |
| -------- | --------------------- |
| Created  | `2018-08-04 19:34:11` |
| Modified | `2018-08-04 19:34:11` |
| Updated  | `2018-08-04 19:34:11` |
| Accessed | `2018-08-04 19:34:11` |

此時間接近記憶體擷取時間，代表在事件發生期間，系統曾產生或存取過 Flag 相關捷徑。

### 判斷

```text
Flag.txt.WINDOWS.lnk 可作為使用者曾開啟或存取 Flag 相關檔案的證據。
```

---

## 5. Rick And Morty 相關紀錄

### 執行指令

```bash
.\vol.exe -f .\OtterCTF.vmem windows.mftscan.MFTScan | findstr "Rick Morty"
```

### 結果

```text
* 0xf980011349280  FILE  60114  ...  FILE_NAME  2018-07-31 20:54:11  2018-07-31 20:54:11  2018-07-31 20:54:11  2018-07-31 20:54:11  Rick And Morty season 1 download.lnk
```

### 分析

`MFTScan` 找到 `Rick And Morty season 1 download.lnk`，代表系統中曾存在與可疑檔案相關的捷徑紀錄。

此檔案時間為：

| 時間欄位     | 時間                    |
| -------- | --------------------- |
| Created  | `2018-07-31 20:54:11` |
| Modified | `2018-07-31 20:54:11` |
| Updated  | `2018-07-31 20:54:11` |
| Accessed | `2018-07-31 20:54:11` |

此紀錄可與前面 `CmdLine`、`FileScan` 的結果交叉比對。

前面已發現可疑執行檔：

```text
\Torrents\Rick And Morty season 1 download.exe
```

而本次 `MFTScan` 發現：

```text
Rick And Morty season 1 download.lnk
```

這代表系統曾產生與該可疑程式相關的捷徑，進一步支持該檔案曾被使用者開啟或執行。

### 判斷

```text
Rick And Morty season 1 download.lnk 可補強 Rick And Morty 可疑程式曾被使用者操作的證據。
```

---

## 6. Traceback / 輸出異常說明

完整執行 `MFTScan` 時，輸出內容非常多，後段出現 `Traceback` 或輸出中斷情況。

此問題主要與輸出量過大、終端機顯示或編碼問題有關，不代表 `MFTScan` 完全失敗。

因為透過 `findstr` 仍成功取得關鍵紀錄，所以本次分析採用關鍵字篩選結果作為重點證據。

---

## 7. 與 FileScan 的比較

| Plugin     | 主要用途                | 本次發現                                                             |
| ---------- | ------------------- | ---------------------------------------------------------------- |
| `FileScan` | 掃描記憶體中的 File Object | 找到 `READ_IT.txt`、`Flag.txt.WINDOWS.lnk`、可疑 EXE                   |
| `MFTScan`  | 掃描 NTFS MFT 檔案系統紀錄  | 找到 `Flag.txt.WINDOWS.lnk`、`Rick And Morty season 1 download.lnk` |

`FileScan` 偏向記憶體中的檔案物件，`MFTScan` 則偏向檔案系統紀錄。

兩者互相補強，可以證明相關檔案不只是出現在記憶體中，也曾存在於 NTFS 檔案系統紀錄內。

---

## 8. 鑑識判斷

本次 `MFTScan` 結果支持以下判斷：

```text
1. 系統中曾存在 Flag.txt.WINDOWS.lnk
2. 使用者可能曾開啟或存取 Flag 相關檔案
3. 系統中曾存在 Rick And Morty season 1 download.lnk
4. Rick And Morty 可疑檔案曾被使用者操作或執行
```

---

## 9. 結論

`windows.mftscan.MFTScan` 結果顯示，系統中存在與本案相關的 MFT 紀錄。

其中 `Flag.txt.WINDOWS.lnk` 可作為 Flag 相關檔案曾被存取的證據。

`Rick And Morty season 1 download.lnk` 則可補強 `Rick And Morty season 1 download.exe` 曾被使用者操作或執行的證據。

結合前面 `FileScan`、`DumpFiles`、`CmdLine` 與 `Pstree` 結果，可以建立以下事件關聯：

```text
Rick 下載或執行 Rick And Morty season 1 download.exe
↓
系統產生 Rick And Morty season 1 download.lnk
↓
可疑程式執行後造成檔案加密
↓
桌面出現 READ_IT.txt
↓
系統留下 Flag.txt.WINDOWS.lnk 紀錄
```


