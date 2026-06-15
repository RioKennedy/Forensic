# 測試內容

- vol.exe -f .\OtterCTF.vmem windows.vadyarascan.VadYaraScan --pid 3820 --yara-rules "rule r1 { strings: $a = 'encrypted' ascii wide nocase condition: $a }"
- vol.exe -f .\OtterCTF.vmem windows.vadyarascan.VadYaraScan --pid 3720 --yara-rules "rule r1 { strings: $a = 'encrypted' ascii wide nocase condition: $a }"


```
D:\Forensic\G140A006\VolatilityWorkbench>.\vol.exe -f .\OtterCTF.vmem windows.vadyarascan.VadYaraScan --pid 3820 --yara-rules "rule r1 { strings: $a = 'encrypted' ascii wide nocase condition: $a }"
Volatility 3 Framework 2.5.0
Progress:  100.00               PDB scanning finished
Offset  PID     Rule    Component       Value


D:\Forensic\G140A006\VolatilityWorkbench>.\vol.exe -f .\OtterCTF.vmem windows.vadyarascan.VadYaraScan --pid 3720 --yara-rules "rule r1 { strings: $a = 'encrypted' ascii wide nocase condition: $a }"
Volatility 3 Framework 2.5.0
Progress:  100.00               PDB scanning finished
Offset  PID     Rule    Component       Value

```

# windows.vadyarascan.VadYaraScan 分析

## 1. Plugin 功能說明

`windows.vadyarascan.VadYaraScan` 用來針對 Process 的 VAD 記憶體區段進行 YARA 規則掃描。

YARA 規則可以用來比對特定字串、惡意程式特徵、加密提示文字或可疑記憶體內容。

本案使用 `VadYaraScan` 針對兩個可疑行程進行掃描：

```text
PID 3820：Rick And Morty season 1 download.exe
PID 3720：vmware-tray.exe
```

---

## 2. 執行指令

本次使用的 YARA 規則是搜尋字串：

```text
encrypted
```

執行指令如下：

```bash
.\vol.exe -f .\OtterCTF.vmem windows.vadyarascan.VadYaraScan --pid 3820 --yara-rules "rule r1 { strings: $a = 'encrypted' ascii wide nocase condition: $a }"
```

```bash
.\vol.exe -f .\OtterCTF.vmem windows.vadyarascan.VadYaraScan --pid 3720 --yara-rules "rule r1 { strings: $a = 'encrypted' ascii wide nocase condition: $a }"
```

---

## 3. 執行結果

兩次執行結果皆只顯示欄位標題：

```text
Offset  PID  Rule  Component  Value
```

結果中沒有出現任何命中資料。

這代表在 PID 3820 與 PID 3720 的 VAD 記憶體區段中，沒有找到符合 YARA 規則的 `encrypted` 字串。

---

## 4. 結果分析

本次 `VadYaraScan` 未命中，表示：

```text
1. PID 3820 的記憶體中沒有掃到 encrypted 字串
2. PID 3720 的記憶體中沒有掃到 encrypted 字串
3. 加密提示文字可能沒有留存在這兩個 Process 的 VAD 記憶體中
4. encrypted 字串可能只存在於 READ_IT.txt 檔案內容或其他記憶體區域
```

因此，這個結果不能直接證明程式正常，也不能排除惡意行為。
