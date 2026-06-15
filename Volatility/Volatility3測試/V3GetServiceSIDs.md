# 測試內容
- .\vol.exe -f .\OtterCTF.vmem windows.getservicesids.GetServiceSIDs

```
D:\Forensic\G140A006\VolatilityWorkbench>.\vol.exe -f .\OtterCTF.vmem windows.getservicesids.GetServiceSIDs
Volatility 3 Framework 2.5.0
Progress:  100.00               PDB scanning finished
SID     Service

S-1-5-80-4151353957-356578678-4163131872-800126167-2037860865   .NET CLR Networking 4.0.0.0
S-1-5-80-1135273183-3738781202-689480478-891280274-255333391    .NET Memory Cache 4.0
S-1-5-80-712059680-203367400-2977813368-4125985704-79366942     ASP.NET
S-1-5-80-2913627202-1669313743-594640567-3758707557-1808359087  ASP.NET_4.0.30319
S-1-5-80-2132180438-3108490898-1075229718-3888178202-2916226535 aspnet_state
S-1-5-80-2676549577-1911656217-2625096541-4178041876-1366760775 AudioSrv
S-1-5-80-957945053-4060038483-2323299089-2025834768-4289255912  b57nd60a
S-1-5-80-3742302039-178175996-3312716580-300089339-184318439    BthEnum
S-1-5-80-1566322655-4174396379-2133637435-1403765164-753964829  BthPan
S-1-5-80-3533787624-3536623824-1878644040-3113243162-1610647180 BTHUSB
S-1-5-80-289285388-4137671665-1240080895-2344186716-3552465961  clr_optimization_v2.0.50727_64
S-1-5-80-2611951811-1959136347-1062071333-3982815153-2811717512 clr_optimization_v4.0.30319_32
S-1-5-80-2839768381-3691089589-2614646340-3191585287-3380622033 clr_optimization_v4.0.30319_64
S-1-5-80-2597136289-665204401-1725106016-1253143166-1853691573  dmvsc
S-1-5-80-1628851891-332911214-942992855-2381080451-357317118    gupdate
S-1-5-80-1391398224-2746689181-3888380295-1755171859-6364376    gupdatem
S-1-5-80-1708301557-710215499-1045718168-382692165-3542596111   HdAudAddService
S-1-5-80-2876499719-392125430-158013367-819050375-2387260967    ksthunk
S-1-5-80-61387632-1770052757-913906803-2764154990-1232092381    MSDTC Bridge 4.0.0.0
S-1-5-80-89244771-1762554971-1007993102-348796144-2203111529    NetMsmqActivator
S-1-5-80-2943419899-937267781-4189664001-1229628381-3982115073  NetPipeActivator
S-1-5-80-3579033775-2824656752-1522793541-1960352512-462907086  NetTcpActivator
S-1-5-80-3596911058-2952229928-1888671852-1743692427-614402820  PerfHost
S-1-5-80-3239442711-4074742016-684152919-2253013163-2274039561  PNPMEM
S-1-5-80-1934309797-2043993622-339923705-3871978825-766431271   RDPUDD
S-1-5-80-3072462152-34466603-861212222-1753422877-4071721522    RdpVideoMiniport
S-1-5-80-2932307366-730193993-4255125875-3321969383-2534286350  RFCOMM
S-1-5-80-217413056-3833387362-178569430-1954288181-1272411947   SMSvcHost 4.0.0.0
S-1-5-80-3182985763-1431228038-2757062859-428472846-3914011746  stisvc
S-1-5-80-927584136-3246479672-3996289350-2713334021-2098405977  Synth3dVsc
S-1-5-80-3141112300-3466319987-880208219-2791244925-2953947883  terminpt
S-1-5-80-3547539953-1452514991-991928397-2821742631-2888215071  TsUsbFlt
S-1-5-80-651631395-3385332028-373277408-2457879084-1955742111   TsUsbGD
S-1-5-80-2292203918-1506848946-3955473809-4024494573-4108135173 tsusbhub
S-1-5-80-2597382502-3270435603-1328819508-2748651462-4181269338 VGAuthService
S-1-5-80-2542079741-2155339696-3470491486-1213005944-2703664652 VGPU
S-1-5-80-776895389-3455876703-3891955142-3754958615-2990024371  vmusbmouse
S-1-5-80-2779368448-1793250562-3292802066-585056660-3968973768  VMware Physical Disk Helper Service
S-1-5-80-2242439072-2748315084-1023843057-2543101977-728157120  vsock
S-1-5-80-1265045923-1690381133-1036424829-2091130558-4079062526 WCAssistantService
S-1-5-80-3488966095-3237316714-2152248236-3202922946-3275547626 Windows Workflow Foundation 4.0.0.0
S-1-5-80-749397962-861781995-899314213-1199340968-2672934077    {7F5B9219-B869-4AEA-84AF-CC6E4C2486FA}
S-1-5-80-4220328718-4250916089-1197843894-617057750-164674738   {965ABEC5-556B-460C-8CE4-11F9DA96FBAC}

```

# windows.getservicesids.GetServiceSIDs 分析

## 1. Plugin 功能說明

`windows.getservicesids.GetServiceSIDs` 用來列出 Windows Service SID 與服務名稱的對應關係。

Windows 服務會有自己的 Service SID，格式通常為：

```text
S-1-5-80-...
```

此 SID 可用來代表某個特定 Windows Service 的安全識別身分。

在數位鑑識中，此 Plugin 可用來協助判斷某些 Process、Token 或權限是否與特定服務有關。

---

## 2. 執行指令

```bash
.\vol.exe -f .\OtterCTF.vmem windows.getservicesids.GetServiceSIDs
```

---

## 3. 欄位說明

| 欄位        | 說明                  |
| --------- | ------------------- |
| `SID`     | Windows Service SID |
| `Service` | 對應的服務名稱             |

---

## 4. 執行結果摘要

本次結果列出多個 Windows 服務與其 Service SID，例如：

```text
.NET CLR Networking 4.0.0.0
.NET Memory Cache 4.0
ASP.NET
AudioSrv
BthEnum
BTHUSB
gupdate
gupdatem
VGAuthService
VMware Physical Disk Helper Service
vmusbmouse
vsock
WCAssistantService
Windows Workflow Foundation 4.0.0.0
```

這些服務大多屬於 Windows 系統、.NET Framework、藍牙、Google Update、VMware Tools 或 WebCompanion / Lavasoft 相關服務。

---

## 5. VMware 相關服務

結果中出現多個 VMware 相關服務，例如：

```text
VGAuthService
VMware Physical Disk Helper Service
vmusbmouse
vsock
```

由於本案記憶體映像來自 VMware 環境，因此這些 VMware 相關服務屬於合理現象，不能直接視為異常。

這也與前面 `modules`、`driverscan`、`driversirp` 中看到的 VMware Driver 結果相符。

---

## 6. WCAssistantService 觀察

結果中也出現：

```text
WCAssistantService
```

此服務名稱與前面 Process 分析中看到的 WebCompanion / Lavasoft 相關程式有關，例如：

```text
WebCompanionIn
WebCompanion.e
Lavasoft.WCAss
```

前面 `netscan` 中也看到這些程式有對外 HTTP 連線。

因此，`WCAssistantService` 可作為 WebCompanion / Lavasoft 軟體存在於系統中的輔助證據。

不過，目前本案主要感染鏈仍是 `Rick And Morty` 與 `vmware-tray.exe`，因此 `WCAssistantService` 不是主要惡意證據。

---

## 7. 與 Rick And Morty / vmware-tray.exe 的關係

本次 Service SID 結果中，沒有看到以下與本案主線直接相關的服務名稱：

```text
Rick And Morty
vmware-tray
RarSFX0
READ_IT
ransom
crypt
encrypt
```

因此，目前沒有證據顯示 `Rick And Morty` 或 `vmware-tray.exe` 是以 Windows Service 身分執行。

這點可以配合前面的 `GetSIDs` 結果判斷：

```text
Rick And Morty 與 vmware-tray.exe 都屬於 Rick 使用者
```

也就是說，本案較偏向 Rick 使用者互動式執行可疑程式，而不是透過 Windows Service 啟動惡意程式。

---

## 8. 鑑識判斷

本次 `GetServiceSIDs` 結果主要提供服務 SID 與服務名稱對照，屬於輔助性證據。

重要判斷如下：

```text
1. 系統存在多個正常 Windows / .NET / VMware 相關服務
2. VMware 相關 Service SID 與虛擬機環境相符
3. WCAssistantService 可對應前面看到的 WebCompanion / Lavasoft 程式
4. 未發現 Rick And Morty 或 vmware-tray.exe 相關 Service SID
5. 沒有證據顯示主要可疑程式是以 Windows Service 身分執行
```

---

## 9. 與其他 Plugin 的關聯

此結果可與前面 Plugin 交叉比對：

```text
GetSIDs：Rick And Morty 與 vmware-tray.exe 都屬於 Rick 使用者
Handles：Rick And Morty 持有 vmware-tray.exe 的 Process handle
Pstree：Rick And Morty 啟動 vmware-tray.exe
CmdLine：vmware-tray.exe 位於 Temp\RarSFX0
Driverscan / DriverIrp：VMware Driver 與服務符合虛擬機環境
Privs：未發現主要可疑 Process 大量高權限濫用
```

因此，`GetServiceSIDs` 的主要用途是確認服務環境，而不是直接證明惡意行為。

---

## 10. 結論

`windows.getservicesids.GetServiceSIDs` 成功列出系統中的 Service SID 與服務名稱對應。

結果中可看到多個正常 Windows、.NET Framework、VMware、Google Update 與 WebCompanion / Lavasoft 相關服務。

未發現與 `Rick And Morty`、`vmware-tray.exe` 或 `RarSFX0` 直接相關的 Service SID。

因此，此 Plugin 結果顯示本案主要可疑程式不像是以 Windows Service 身分執行，而是更偏向 Rick 使用者互動式執行可疑 EXE 後造成的感染鏈。

本案主線仍為：

```text
Rick 使用者
→ Rick And Morty season 1 download.exe
→ Temp\RarSFX0\vmware-tray.exe
→ 可疑記憶體區段
→ READ_IT.txt 加密提示
```

