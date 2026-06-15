# 測試內容

- .\vol.exe -f .\OtterCTF.vmem windows.getsids.GetSIDs --pid 3820

```
D:\Forensic\G140A006\VolatilityWorkbench>.\vol.exe -f .\OtterCTF.vmem windows.getsids.GetSIDs --pid 3820
Volatility 3 Framework 2.5.0
Progress:  100.00               PDB scanning finished
PID     Process SID     Name

3820    Rick And Morty  S-1-5-21-1923827501-2510115606-422599235-1000   Rick
3820    Rick And Morty  S-1-5-21-1923827501-2510115606-422599235-513    Domain Users
3820    Rick And Morty  S-1-1-0 Everyone
3820    Rick And Morty  S-1-5-32-544    Administrators
3820    Rick And Morty  S-1-5-32-545    Users
3820    Rick And Morty  S-1-5-4 Interactive
3820    Rick And Morty  S-1-2-1 Console Logon (Users who are logged onto the physical console)
3820    Rick And Morty  S-1-5-11        Authenticated Users
3820    Rick And Morty  S-1-5-15        This Organization
3820    Rick And Morty  S-1-5-5-0-332191        Logon Session
3820    Rick And Morty  S-1-2-0 Local (Users with the ability to log in locally)
3820    Rick And Morty  S-1-5-64-10     NTLM Authentication
3820    Rick And Morty  S-1-16-8192     Medium Mandatory Level
```

- .\vol.exe -f .\OtterCTF.vmem windows.getsids.GetSIDs --pid 3820

```
D:\Forensic\G140A006\VolatilityWorkbench>.\vol.exe -f .\OtterCTF.vmem windows.getsids.GetSIDs --pid 3720
Volatility 3 Framework 2.5.0
Progress:  100.00               PDB scanning finished
PID     Process SID     Name

3720    vmware-tray.ex  S-1-5-21-1923827501-2510115606-422599235-1000   Rick
3720    vmware-tray.ex  S-1-5-21-1923827501-2510115606-422599235-513    Domain Users
3720    vmware-tray.ex  S-1-1-0 Everyone
3720    vmware-tray.ex  S-1-5-32-544    Administrators
3720    vmware-tray.ex  S-1-5-32-545    Users
3720    vmware-tray.ex  S-1-5-4 Interactive
3720    vmware-tray.ex  S-1-2-1 Console Logon (Users who are logged onto the physical console)
3720    vmware-tray.ex  S-1-5-11        Authenticated Users
3720    vmware-tray.ex  S-1-5-15        This Organization
3720    vmware-tray.ex  S-1-5-5-0-332191        Logon Session
3720    vmware-tray.ex  S-1-2-0 Local (Users with the ability to log in locally)
3720    vmware-tray.ex  S-1-5-64-10     NTLM Authentication
3720    vmware-tray.ex  S-1-16-12288    High Mandatory Level

```

# windows.getsids.GetSIDs 分析

## 1. Plugin 功能說明

`windows.getsids.GetSIDs` 用來列出指定 Process Token 中的 SID，也就是該 Process 所屬的使用者與群組身分。

SID 可以協助判斷 Process 是由哪個使用者執行，以及它是否屬於特定群組，例如：

```text
Administrators
Users
Authenticated Users
Interactive
Console Logon
```

在數位鑑識中，`GetSIDs` 可以用來確認可疑 Process 的使用者身分與權限群組。

---

## 2. 執行指令

```bash
.\vol.exe -f .\OtterCTF.vmem windows.getsids.GetSIDs --pid 3820
```

```bash
.\vol.exe -f .\OtterCTF.vmem windows.getsids.GetSIDs --pid 3720
```

---

## 3. PID 3820：Rick And Morty 分析

PID 3820 `Rick And Morty` 的 SID 結果顯示，此 Process 屬於使用者：

```text
S-1-5-21-1923827501-2510115606-422599235-1000   Rick
```

同時也屬於以下群組：

```text
Domain Users
Everyone
Administrators
Users
Interactive
Console Logon
Authenticated Users
Local
NTLM Authentication
```

其中最重要的是：

```text
S-1-16-8192     Medium Mandatory Level
```

這表示 PID 3820 `Rick And Morty` 是以 Medium Integrity Level 執行，屬於一般互動式使用者層級。

---

## 4. PID 3720：vmware-tray.ex 分析

PID 3720 `vmware-tray.ex` 的 SID 結果同樣顯示，此 Process 屬於使用者：

```text
S-1-5-21-1923827501-2510115606-422599235-1000   Rick
```

它也同樣屬於以下群組：

```text
Domain Users
Everyone
Administrators
Users
Interactive
Console Logon
Authenticated Users
Local
NTLM Authentication
```

這表示 `vmware-tray.ex` 也是在 Rick 使用者環境下執行。

但與 PID 3820 不同的是，PID 3720 的完整性等級為：

```text
S-1-16-12288    High Mandatory Level
```

這表示 PID 3720 `vmware-tray.ex` 是以 High Integrity Level 執行，權限層級高於 PID 3820。

---

## 5. 重要差異比較

| PID  | Process        | User | Group                  | Integrity Level |
| ---- | -------------- | ---- | ---------------------- | --------------- |
| 3820 | Rick And Morty | Rick | Administrators / Users | Medium          |
| 3720 | vmware-tray.ex | Rick | Administrators / Users | High            |

從結果來看，兩個 Process 都屬於 Rick 使用者，且都在互動式登入環境下執行。

但是：

```text
Rick And Morty = Medium Integrity Level
vmware-tray.ex = High Integrity Level
```

這代表 `vmware-tray.ex` 具有比 `Rick And Morty` 更高的完整性層級。

---

## 6. 鑑識判斷

本次 `GetSIDs` 結果提供了兩個重要判斷：

```text
1. Rick And Morty 與 vmware-tray.ex 都屬於 Rick 使用者
2. vmware-tray.ex 的 Integrity Level 為 High，高於 Rick And Morty 的 Medium
```

第一點可以補強本案是 Rick 使用者執行可疑程式所產生的感染鏈。

第二點表示 `vmware-tray.exe` 可能在較高權限狀態下執行，這使其進行檔案操作或系統操作時具有更高能力。

不過，單靠 `GetSIDs` 不能直接證明權限提升行為，仍需要與 `Privs`、`Handles`、`Pstree`、`CmdLine`、`Malfind` 等結果一起判斷。
