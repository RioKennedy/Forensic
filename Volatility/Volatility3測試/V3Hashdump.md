# 測試內容
- .\vol.exe -f .\OtterCTF.vmem windows.hashdump.Hashdump

```
D:\Forensic\G140A006\VolatilityWorkbench>.\vol.exe -f .\OtterCTF.vmem windows.hashdump.Hashdump
Volatility 3 Framework 2.5.0
Progress:  100.00               PDB scanning finished
User    rid     lmhash  nthash

Administrator   500     aad3b435b51404eeaad3b435b51404ee        31d6cfe0d16ae931b73c59d7e0c089c0
Guest   501     aad3b435b51404eeaad3b435b51404ee        31d6cfe0d16ae931b73c59d7e0c089c0
Rick    1000    aad3b435b51404eeaad3b435b51404ee        518172d012f97d3a8fcc089615283940

```

# windows.hashdump.Hashdump 分析

## 1. Plugin 功能說明

`windows.hashdump.Hashdump` 用來從記憶體中的 Registry Hive 解析本機帳號的密碼雜湊值。

此 Plugin 通常會從 SAM、SYSTEM 等 Registry Hive 中取得本機使用者帳號資訊，包含：

```text
User
RID
LM Hash
NT Hash
```

在數位鑑識中，`Hashdump` 可用來確認系統中有哪些本機帳號，以及帳號是否存在密碼雜湊資料。

---

## 2. 執行指令

```bash
.\vol.exe -f .\OtterCTF.vmem windows.hashdump.Hashdump
```

---

## 3. 執行結果

本次結果如下：

```text
User            RID     LM Hash                             NT Hash
Administrator   500     aad3b435b51404eeaad3b435b51404ee    31d6cfe0d16ae931b73c59d7e0c089c0
Guest           501     aad3b435b51404eeaad3b435b51404ee    31d6cfe0d16ae931b73c59d7e0c089c0
Rick            1000    aad3b435b51404eeaad3b435b51404ee    518172d012f97d3a8fcc089615283940
```

---

## 4. 欄位說明

| 欄位        | 說明                          |
| --------- | --------------------------- |
| `User`    | 本機使用者帳號名稱                   |
| `RID`     | Relative Identifier，本機帳號識別碼 |
| `LM Hash` | 舊式 LAN Manager 密碼雜湊         |
| `NT Hash` | NTLM 密碼雜湊                   |

---

## 5. 帳號分析

### 5.1 Administrator

```text
Administrator   RID 500
```

`Administrator` 是 Windows 內建管理員帳號，RID 通常為 `500`。

其 NT Hash 為：

```text
31d6cfe0d16ae931b73c59d7e0c089c0
```

此值通常代表空密碼的 NTLM hash。

但需要注意，Hashdump 只能顯示密碼雜湊，不能單獨判斷帳號是否啟用或是否可登入。

---

### 5.2 Guest

```text
Guest   RID 501
```

`Guest` 是 Windows 內建訪客帳號，RID 通常為 `501`。

其 NT Hash 同樣為：

```text
31d6cfe0d16ae931b73c59d7e0c089c0
```

此值通常代表空密碼的 NTLM hash。

但 Guest 帳號在 Windows 中通常預設停用，因此不能只靠此結果判斷它能被使用。

---

### 5.3 Rick

```text
Rick    RID 1000
```

`Rick` 是本案最重要的使用者帳號。

其 NT Hash 為：

```text
518172d012f97d3a8fcc089615283940
```

這表示 Rick 帳號有可用的 NTLM 密碼雜湊值，與前面多個 Plugin 顯示的 Rick 使用者活動相符。

前面證據已顯示：

```text
Rick 使用者執行 BitTorrent
Rick 使用者執行 Rick And Morty season 1 download.exe
Rick And Morty 啟動 Temp\RarSFX0\vmware-tray.exe
READ_IT.txt 出現在 Rick Desktop
```

因此，Hashdump 可用來補充說明本機存在 Rick 帳號，且該帳號是本案主要使用者。

---

## 6. LM Hash 觀察

三個帳號的 LM Hash 都是：

```text
aad3b435b51404eeaad3b435b51404ee
```

這通常代表 LM Hash 未使用或為空值。

在較新的 Windows 系統中，LM Hash 通常會停用，因此這個結果屬於常見現象。

---

## 7. 鑑識判斷

本次 `Hashdump` 結果顯示系統中至少存在以下本機帳號：

```text
Administrator
Guest
Rick
```

其中 `Rick` 是主要使用者帳號，RID 為 `1000`，並且具有 NTLM hash。

此結果與前面 `GetSIDs`、`UserAssist`、`CmdLine`、`Handles` 等結果一致，支持本案主要行為發生在 Rick 使用者環境下。

不過，`Hashdump` 本身沒有直接顯示惡意程式執行、檔案加密或網路連線行為，因此它不是本案主要惡意證據。

---

## 8. 與本案關聯

`Hashdump` 可與前面結果交叉確認：

```text
GetSIDs：Rick And Morty 與 vmware-tray.ex 都屬於 Rick 使用者
UserAssist：Rick 使用者執行過 Rick And Morty season 1 download.exe
Filescan：Rick 使用者目錄下存在 READ_IT.txt 與 RarSFX0\vmware-tray.exe
Handles：Rick And Morty 與 vmware-tray.exe 都與 Rick 使用者環境有關
Hashdump：系統中存在 Rick 本機帳號
```

因此，`Hashdump` 的角色主要是補充帳號背景與使用者身分，不是用來證明惡意行為本身。

---

## 9. 結論

`windows.hashdump.Hashdump` 成功擷取本機帳號雜湊資訊。

結果顯示系統中存在 `Administrator`、`Guest` 與 `Rick` 三個帳號。

其中 `Rick` 的 RID 為 `1000`，並具有 NTLM hash，與前面分析中大量 Rick 使用者活動相符。

綜合判斷，本案主要活動發生在 Rick 使用者環境下。

但 `Hashdump` 並未直接提供惡意程式執行或加密行為證據，因此應作為帳號與身分背景的輔助證據。

本案主要證據仍為：

```text
Rick 使用者
→ BitTorrent 下載活動
→ Rick And Morty season 1 download.exe
→ Temp\RarSFX0\vmware-tray.exe
→ 可疑記憶體區段
→ READ_IT.txt 加密提示
```
