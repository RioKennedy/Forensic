## 測試內容
 - .\vol.exe -f .\OtterCTF.vmem windows.crashinfo.Crashinfo

## windows.crashinfo.Crashinfo 執行結果

執行 `windows.crashinfo.Crashinfo` 時，Volatility 顯示錯誤訊息：

```text
This plugin requires a Windows crash dump
```
此錯誤代表該 Plugin 只能用於 Windows Crash Dump 檔案，例如 MEMORY.DMP 或 .dmp 檔案。

本次分析的檔案為 OtterCTF.vmem，屬於一般記憶體映像檔，並不是 Windows Crash Dump 格式，因此無法使用 windows.crashinfo.Crashinfo 進行分析。

這不代表記憶體映像檔損壞，也不影響後續分析。

```
D:\Forensic\G140A006\VolatilityWorkbench>.\vol.exe -f .\OtterCTF.vmem windows.crashinfo.Crashinfo
Volatility 3 Framework 2.5.0
ERROR    volatility3.plugins.windows.crashinfo: This plugin requires a Windows crash dump
Traceback (most recent call last):
  File "vol.py", line 10, in <module>
  File "volatility3\cli\__init__.py", line 790, in main
  File "volatility3\cli\__init__.py", line 447, in run
  File "volatility3\framework\plugins\windows\crashinfo.py", line 86, in run
RuntimeError: No active exception to reraise
[9048] Failed to execute script 'vol' due to unhandled exception!
```
