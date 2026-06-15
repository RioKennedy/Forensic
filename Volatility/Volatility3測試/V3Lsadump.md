# 測試內容

- .\vol.exe -f .\OtterCTF.vmem windows.lsadump.Lsadump

```
D:\Forensic\G140A006\VolatilityWorkbench>.\vol.exe -f .\OtterCTF.vmem windows.lsadump.Lsadump
Volatility 3 Framework 2.5.0
Progress:  100.00               PDB scanning finished
Key     Secret  Hex

DefaultPassword (MortyIsReallyAnOtter   28 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 4d 00 6f 00 72 00 74 00 79 00 49 00 73 00 52 00 65 00 61 00 6c 00 6c 00 79 00 41 00 6e 00 4f 00 74 00 74 00 65 00 72 00 00 00 00 00 00 00 00 00
DPAPI_SYSTEM    ,6º©Uá  àcL tcØ KEZä¼òw¥%?G
                                           åM¥È5ÏÜ      2c 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 01 00 00 00 36 9b ba a9 55 e1 92 82 09 e0 63 4c 20 74 63 14 9e d8 a0 4b 45 87 5a e4 bc f2 77 a5 25 3f 47 12 0b e5 4d a5 c8 35 cf dc 00 00 00 00

```

# windows.lsadump.Lsadump 分析

## 1. Plugin 功能說明

`windows.lsadump.Lsadump` 用來擷取 Windows LSA Secrets。

LSA Secrets 是 Windows 用來儲存敏感資訊的位置，可能包含：

```text
自動登入密碼
服務帳號密碼
DPAPI_SYSTEM 金鑰
系統秘密資料
網域或本機認證相關資訊
```

在數位鑑識中，`Lsadump` 可用來確認系統是否保存明文密碼或其他敏感憑證。

---

## 2. 執行指令

```bash
.\vol.exe -f .\OtterCTF.vmem windows.lsadump.Lsadump
```

---

## 3. 執行結果

本次結果發現兩個主要項目：

```text
DefaultPassword
DPAPI_SYSTEM
```

其中最重要的是：

```text
DefaultPassword = MortyIsReallyAnOtter
```

另外也擷取到 `DPAPI_SYSTEM` secret，這通常與 Windows DPAPI 保護機制有關。

---

## 4. DefaultPassword 分析

`DefaultPassword` 的內容為：

```text
MortyIsReallyAnOtter
```

此欄位通常與 Windows 自動登入設定或預設登入密碼有關。

此結果表示系統中曾經保存一組明文密碼，並且 Volatility 成功從記憶體中的 LSA Secrets 解析出來。

這比 `Hashdump` 的 NTLM hash 更直接，因為 `Hashdump` 只能取得密碼雜湊，而 `Lsadump` 這次直接顯示可讀的明文 secret。

---

## 5. DPAPI_SYSTEM 分析

結果中也出現：

```text
DPAPI_SYSTEM
```

`DPAPI_SYSTEM` 是 Windows Data Protection API 使用的系統層級秘密資料。

DPAPI 常用來保護瀏覽器密碼、憑證、Wi-Fi 密碼或其他應用程式保存的敏感資料。

本次雖然成功取得 `DPAPI_SYSTEM`，但此項目本身不直接代表惡意行為。它主要表示系統中的 DPAPI 相關秘密資料可以被解析。

---

## 6. 與 Hashdump 的比較

前面 `Hashdump` 取得的結果顯示：

```text
Rick    NT Hash = 518172d012f97d3a8fcc089615283940
```

`Hashdump` 只能提供密碼 hash，不能直接看到明文密碼。

而本次 `Lsadump` 則取得：

```text
DefaultPassword = MortyIsReallyAnOtter
```

因此，`Lsadump` 提供了更直接的憑證證據。

不過，仍需要注意：`DefaultPassword` 不一定等於 Rick 帳號密碼，但它表示系統中確實存在一組被保存的明文密碼資料。
