# 測試內容

- vol.exe -f .\OtterCTF.vmem windows.skeleton_key_check.Skeleton_Key_Check

```
D:\Forensic\G140A006\VolatilityWorkbench>.\vol.exe -f .\OtterCTF.vmem windows.skeleton_key_check.Skeleton_Key_Check
Volatility 3 Framework 2.5.0
Progress:  100.00               PDB scanning finished
PID     Process Skeleton Key Found      rc4HmacInitialize       rc4HmacDecrypt
```

# windows.skeleton_key_check.Skeleton_Key_Check 分析

## 1. Plugin 功能說明

`windows.skeleton_key_check.Skeleton_Key_Check` 用來檢查 Windows 記憶體中是否存在 Skeleton Key 攻擊跡象。

Skeleton Key 是一種針對 Windows Domain Controller 的攻擊手法，攻擊者可能會修改 LSASS 記憶體中的驗證流程，使攻擊者能使用特定密碼登入多個帳號。

此 Plugin 主要會檢查與 Windows 認證相關的記憶體函式，例如：

```text id="x04xnd"
rc4HmacInitialize
rc4HmacDecrypt
```

如果這些函式被異常修改，可能代表系統遭受 Skeleton Key 類型攻擊。

---

## 2. 執行指令

```bash id="k53uow"
.\vol.exe -f .\OtterCTF.vmem windows.skeleton_key_check.Skeleton_Key_Check
```

---

## 3. 執行結果

本次執行結果如下：

```text id="07ypwb"
PID  Process  Skeleton Key Found  rc4HmacInitialize  rc4HmacDecrypt
```

結果只顯示欄位標題，沒有列出任何可疑 Process。

---

## 4. 結果分析

本次 `Skeleton_Key_Check` 沒有發現 Skeleton Key 攻擊跡象。

代表在記憶體中沒有偵測到與 Skeleton Key 相關的異常認證函式修改。

此結果可說明：

```text id="cuyh6d"
1. 沒有發現 Skeleton Key 攻擊跡象
2. 沒有發現 LSASS 認證函式被明顯 patch
3. 本案重點不在網域認證或帳號登入繞過
```
