# 測試內容

- .\vol.exe -f .\OtterCTF.vmem windows.cachedump.Cachedump

```
D:\Forensic\G140A006\VolatilityWorkbench>.\vol.exe -f .\OtterCTF.vmem windows.cachedump.Cachedump
Volatility 3 Framework 2.5.0
Progress:  100.00               PDB scanning finished
Username        Domain  Domain name     Hash
WARNING  volatility3.plugins.windows.cachedump: Unable to find nlkma key
```

# windows.cachedump.Cachedump 分析

## 1. Plugin 功能說明

`windows.cachedump.Cachedump` 用來擷取 Windows 系統中的 Domain Cached Credentials。

當 Windows 電腦曾經登入網域帳號時，系統可能會在本機保存快取登入資訊，讓使用者在無法連線到網域控制站時仍可登入。

此 Plugin 主要用來分析是否存在網域帳號快取憑證。

---

## 2. 執行指令

```bash
.\vol.exe -f .\OtterCTF.vmem windows.cachedump.Cachedump
```

---

## 3. 執行結果

本次執行結果如下：

```text
Username        Domain  Domain name     Hash
WARNING  volatility3.plugins.windows.cachedump: Unable to find nlkma key
```

結果中沒有列出任何 Username、Domain 或 Hash。

同時出現警告：

```text
Unable to find nlkma key
```

---

## 4. 結果說明

`Cachedump` 需要找到系統中用來解密 cached credentials 的 key，通常與 `NL$KM` 相關。

本次出現 `Unable to find nlkma key`，表示 Volatility 沒有成功找到或解析該 key，因此無法解出 Domain Cached Credentials。

可能原因包括：

```text
系統沒有網域快取登入資料
記憶體中缺少必要 Registry Hive 或 Key
記憶體映像取得時相關資料不完整
此機器主要使用本機帳號登入，而非網域帳號
```

---

## 5. 鑑識判斷

本次 `Cachedump` 沒有取得任何網域快取憑證。

因此，目前沒有證據顯示本案涉及網域帳號快取憑證擷取或網域登入憑證分析。

此結果與前面 `Hashdump` 的結果相比，`Hashdump` 成功列出本機帳號：

```text
Administrator
Guest
Rick
```

因此，本案使用者身分分析仍以本機帳號 `Rick` 為主。
