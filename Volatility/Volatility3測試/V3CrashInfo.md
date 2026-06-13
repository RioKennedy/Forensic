## windows.crashinfo.Crashinfo 執行結果

執行 `windows.crashinfo.Crashinfo` 時，Volatility 顯示錯誤訊息：

```text
This plugin requires a Windows crash dump

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
