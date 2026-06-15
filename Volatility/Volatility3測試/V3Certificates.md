# 測試內容

- vol.exe -f .\OtterCTF.vmem windows.registry.certificates.Certificates

```
D:\Forensic\G140A006\VolatilityWorkbench>.\vol.exe -f .\OtterCTF.vmem windows.registry.certificates.Certificates
Volatility 3 Framework 2.5.0
Progress:  100.00               PDB scanning finished
Certificate path        Certificate section     Certificate ID  Certificate name

Microsoft\SystemCertificates    AuthRoot        02FAF3E291435468607857694DF5E45B68851868        The USERTrust Network™
Microsoft\SystemCertificates    AuthRoot        2796BAE63F1801E277261BA0D77770028F20EEE4        Go Daddy Class 2 Certification Authority
Microsoft\SystemCertificates    AuthRoot        47BEABC922EAE80E78783462A79F45C254FDE68B        Go Daddy Root Certificate Authority – G2
Microsoft\SystemCertificates    AuthRoot        4EB6D578499B1CCF5F581EAD56BE3D9B6744A5E5        VeriSign
Microsoft\SystemCertificates    AuthRoot        5FB7EE0633E259DBAD0C4C9AE6D38F1A61C7DC25        DigiCert
Microsoft\SystemCertificates    AuthRoot        627F8D7827656399D27D7F9044C9FEB3F33EFA9A        thawte
Microsoft\SystemCertificates    AuthRoot        742C3192E607E424EB4549542BE1BBC53E6174E2        VeriSign Class 3 Public Primary CA
Microsoft\SystemCertificates    AuthRoot        75E0ABB6138512271C04F85FDDDE38E4B7242EFE        Google Trust Services - GlobalSign Root CA-R2
Microsoft\SystemCertificates    AuthRoot        85A408C09C193E5D51587DCDD61330FD8CDE37BF        Deutsche Telekom Root CA 2
Microsoft\SystemCertificates    AuthRoot        8782C6C304353BCFD29692D2593E7D44D934FF11        Trustwave
Microsoft\SystemCertificates    AuthRoot        91C6D6EE3E8AC86384E548C299295C756C817B81        thawte
Microsoft\SystemCertificates    AuthRoot        97817950D81C9670CC34D809CF794431367EF474        DigiCert Global Root
Microsoft\SystemCertificates    AuthRoot        A8985D3A65E5E5C4B2D7D66D40C6DD2FB19C5436        DigiCert
Microsoft\SystemCertificates    AuthRoot        AD7E1C28B064EF8F6003402014C3D0E3370EB58A        Starfield Class 2 Certification Authority
Microsoft\SystemCertificates    AuthRoot        B1BC968BD4F49D622AA89A81F2150152A41D829C        GlobalSign Root CA - R1
Microsoft\SystemCertificates    AuthRoot        B51C067CEE2B0C3DF855AB2D92F4FE39D4E70F0E        Starfield Root Certificate Authority – G2
Microsoft\SystemCertificates    AuthRoot        D4DE20D05E66FC53FE1A50882C78DB2852CAE474        DigiCert Baltimore Root
Microsoft\SystemCertificates    AuthRoot        D69B561148F01C77C54578C10926DF5B856976AD        GlobalSign Root CA - R3
Microsoft\SystemCertificates    AuthRoot        DAC9024F54D8F6DF94935FB1732638CA6AD77C13        DST Root CA X3
Microsoft\SystemCertificates    AuthRoot        DE28F4A4FFE5B92FA3C503D1A349A7F9962A8212        GeoTrust Global CA
Microsoft\SystemCertificates    AuthRoot        E12DFB4B41D7D9C32B30514BAC1D81D8385E2D46        USERTrust (Code Signing)
Microsoft\SystemCertificates    CA      109F1CAED645BB78B3EA2B94C0697C740733031C        -
Microsoft\SystemCertificates    CA      D559A586669B08F46A30A133F8A9ED3D038E2EA8        -
Microsoft\SystemCertificates    CA      FEE449EE0E3965A5246F000E87FDE2A065FD89D4        -
Microsoft\SystemCertificates    CA      A377D1B1C0538833035211F4083D00FECC414DAB        -
Microsoft\SystemCertificates    Disallowed      637162CC59A3A1E25956FA5FA8F60D2E1C52EAC6        Fraudulent, NOT Microsoft
Microsoft\SystemCertificates    Disallowed      7D7F4414CCEF168ADF6BF40753B5BECD78375931        Fraudulent, NOT Microsoft
Microsoft\SystemCertificates    ROOT    18F7C1FCC3090203FD5BAA2F861A754976C8DD25        VeriSign Time Stamping CA
Microsoft\SystemCertificates    ROOT    245C97DF7514E7CF2DF8BE72AE957B9E04741E85        Microsoft Timestamp Root
Microsoft\SystemCertificates    ROOT    7F88CD7223F3C813818C994614A89C99FA3B5247        Microsoft Authenticode(tm) Root
Microsoft\SystemCertificates    ROOT    A43489159A520F0D93D032CCAF37E7FE20A8B419        Microsoft Root Authority
Microsoft\SystemCertificates    ROOT    BE36A4562FB2EE05DBB3D32323ADF445084ED656        Thawte Timestamping CA
Microsoft\SystemCertificates    ROOT    CDD4EEAE6000AC7F40C3802C171E30148030C072        Microsoft Root Certificate Authority
Software\Microsoft\SystemCertificates   Root    ProtectedRoots  -
Software\Microsoft\SystemCertificates   Root    ProtectedRoots  -
Software\Microsoft\SystemCertificates   CA      7CCC2A87E3949F20572B18482980505FA90CAC3B        -
Software\Microsoft\SystemCertificates   CA      F5AD0BCC1AD56CD150725B1C866C30AD92EF21B0        -
Software\Microsoft\SystemCertificates   Root    ProtectedRoots  -
```

# windows.registry.certificates.Certificates 分析

## 1. Plugin 功能說明

`windows.registry.certificates.Certificates` 用來列出 Windows Registry 中的系統憑證資訊。

此 Plugin 主要可以協助分析：

```text
系統信任的 Root CA 憑證
中繼憑證 CA
被禁止或撤銷信任的憑證
是否存在可疑或異常新增的憑證
```

在惡意程式鑑識中，攻擊者有時可能會新增惡意 Root Certificate，使系統信任偽造網站、惡意代理或中間人攻擊憑證。因此檢查憑證儲存區可以用來確認是否有憑證層級的異常。

---

## 2. 執行指令

```bash
.\vol.exe -f .\OtterCTF.vmem windows.registry.certificates.Certificates
```

---

## 3. 欄位說明

| 欄位                    | 說明                                          |
| --------------------- | ------------------------------------------- |
| `Certificate path`    | 憑證所在的 Registry 路徑                           |
| `Certificate section` | 憑證分類，例如 `AuthRoot`、`CA`、`ROOT`、`Disallowed` |
| `Certificate ID`      | 憑證的雜湊識別值                                    |
| `Certificate name`    | 憑證名稱或發行單位                                   |

---

## 4. 執行結果重點

本次結果中發現多個系統憑證項目，主要包含：

```text
Microsoft\SystemCertificates\AuthRoot
Microsoft\SystemCertificates\CA
Microsoft\SystemCertificates\Disallowed
Microsoft\SystemCertificates\ROOT
Software\Microsoft\SystemCertificates\Root
Software\Microsoft\SystemCertificates\CA
```

其中 `AuthRoot` 與 `ROOT` 中出現多個常見信任憑證，例如：

```text
DigiCert
VeriSign
GlobalSign
Go Daddy
GeoTrust
thawte
Microsoft Root Authority
Microsoft Root Certificate Authority
Google Trust Services
```

這些通常屬於正常的系統信任憑證。

---

## 5. Disallowed 憑證

結果中也發現 `Disallowed` 區段：

```text
Microsoft\SystemCertificates    Disallowed    637162CC59A3A1E25956FA5FA8F60D2E1C52EAC6    Fraudulent, NOT Microsoft
Microsoft\SystemCertificates    Disallowed    7D7F4414CCEF168ADF6BF40753B5BECD78375931    Fraudulent, NOT Microsoft
```

`Disallowed` 代表這些憑證已被系統列為不信任或禁止使用。

此結果本身不一定是惡意跡象，反而代表系統中有紀錄被禁止信任的憑證。

---

## 6. 分析結果

本次 `Certificates` 結果主要顯示系統內建或正常存在的憑證項目。

目前未發現以下可疑情況：

```text
與 Rick And Morty season 1 download.exe 相關的憑證
與 vmware-tray.exe 相關的憑證
異常新增的 Root Certificate
可疑的自簽憑證
明顯與惡意程式名稱相關的憑證
```

因此，憑證分析目前沒有提供本案主要感染來源的直接證據。

---

## 7. 鑑識判斷

`Certificates` 在本案中屬於輔助檢查項目。

其主要目的為確認系統是否存在憑證層級的異常，例如惡意 Root CA 或不正常的信任憑證。

根據目前結果，未發現明顯異常憑證，也未發現與本案可疑程式直接相關的憑證紀錄。

因此，本案目前仍較符合使用者透過 BitTorrent 下載並執行可疑程式，導致檔案加密的情境，而不是憑證遭竄改或憑證信任鏈被濫用。

---

## 8. 結論

`windows.registry.certificates.Certificates` 成功列出系統中的憑證資訊。

本次結果多數為正常的系統 Root CA、AuthRoot、CA 與 Microsoft 相關憑證。

雖然有出現 `Disallowed` 憑證項目，但其名稱顯示為 `Fraudulent, NOT Microsoft`，屬於系統已禁止信任的憑證紀錄，未發現其與本案可疑程式有直接關聯。

因此，本 Plugin 未發現明顯惡意憑證或憑證層級感染跡象。

本案主要證據仍集中於：

```text
BitTorrent 下載活動
Rick And Morty season 1 download.exe
Temp\RarSFX0\vmware-tray.exe
READ_IT.txt 加密提示檔
UserAssist 執行紀錄
```

