# 測試內容
- vol.exe -f .\OtterCTF.vmem windows.netscan.NetScan

```
D:\Forensic\G140A006\VolatilityWorkbench>.\vol.exe -f .\OtterCTF.vmem windows.netscan.NetScan
Volatility 3 Framework 2.5.0
Progress:  100.00               PDB scanning finished
Offset  Proto   LocalAddr       LocalPort       ForeignAddr     ForeignPort     State   PID     Owner    Created

0x7d42ba90      TCPv4   -       0       56.219.196.26   0       CLOSED  2836    BitTorrent.exe  N/A
0x7d60f010      UDPv4   0.0.0.0 1900    *       0               2836    BitTorrent.exe  2018-08-04 19:27:17.000000
0x7d6124d0      TCPv4   192.168.202.131 49530   77.102.199.102  7575    CLOSED  708     LunarMS.exe      -
0x7d62b3f0      UDPv4   192.168.202.131 6771    *       0               2836    BitTorrent.exe  2018-08-04 19:27:22.000000
0x7d62d690      TCPv4   192.168.202.131 49229   169.1.143.215   8999    CLOSED  2836    BitTorrent.exe   N/A
0x7d62f4c0      UDPv4   127.0.0.1       62307   *       0               2836    BitTorrent.exe  2018-08-04 19:27:17.000000
0x7d62f920      UDPv4   192.168.202.131 62306   *       0               2836    BitTorrent.exe  2018-08-04 19:27:17.000000
0x7d634350      TCPv6   -       0       38db:c41a:80fa:ffff:38db:c41a:80fa:ffff 0       CLOSED  2836     BitTorrent.exe  N/A
0x7d6424c0      UDPv4   0.0.0.0 50762   *       0               4076    chrome.exe      2018-08-04 19:33:37.000000
0x7d6b4250      UDPv6   ::1     1900    *       0               164     svchost.exe     2018-08-04 19:28:42.000000
0x7d6e3230      UDPv4   127.0.0.1       6771    *       0               2836    BitTorrent.exe  2018-08-04 19:27:22.000000
0x7d6ed650      UDPv4   0.0.0.0 5355    *       0               620     svchost.exe     2018-08-04 19:34:22.000000
0x7d6f27f0      TCPv4   192.168.202.131 50381   71.198.155.180  34674   CLOSED  2836    BitTorrent.exe   -
0x7d704010      TCPv4   192.168.202.131 50382   92.251.23.204   6881    CLOSED  2836    BitTorrent.exe   -
0x7d708cf0      TCPv4   192.168.202.131 50364   91.140.89.116   31847   CLOSED  2836    BitTorrent.exe   -
0x7d71c8a0      UDPv4   0.0.0.0 0       *       0               868     svchost.exe     2018-08-04 19:34:22.000000
0x7d71c8a0      UDPv6   ::      0       *       0               868     svchost.exe     2018-08-04 19:34:22.000000
0x7d729620      TCPv4   -       50034   142.129.37.27   24578   CLOSED  2836    BitTorrent.exe  -
0x7d72cbe0      TCPv4   192.168.202.131 50340   23.37.43.27     80      CLOSED  3496    Lavasoft.WCAss   -
0x7d7365a0      TCPv4   192.168.202.131 50358   23.37.43.27     80      CLOSED  3856    WebCompanion.e   -
0x7d74a390      UDPv4   127.0.0.1       52847   *       0               2624    bittorrentie.e  2018-08-04 19:27:24.000000
0x7d7602c0      UDPv4   127.0.0.1       52846   *       0               2308    bittorrentie.e  2018-08-04 19:27:24.000000
0x7d787010      UDPv4   0.0.0.0 65452   *       0               4076    chrome.exe      2018-08-04 19:33:42.000000
0x7d789b50      UDPv4   0.0.0.0 50523   *       0               620     svchost.exe     2018-08-04 19:34:22.000000
0x7d789b50      UDPv6   ::      50523   *       0               620     svchost.exe     2018-08-04 19:34:22.000000
0x7d81c890      TCPv4   192.168.202.131 50335   185.154.111.20  60405   CLOSED  2836    BitTorrent.exe   -
0x7d8bb390      TCPv4   0.0.0.0 9008    0.0.0.0 0       LISTENING       4       System  -
0x7d8bb390      TCPv6   ::      9008    ::      0       LISTENING       4       System  -
0x7d8fd530      TCPv4   192.168.202.131 50327   23.37.43.27     80      CLOSED  3496    Lavasoft.WCAss   -
0x7d92a230      UDPv4   0.0.0.0 0       *       0               868     svchost.exe     2018-08-04 19:34:22.000000
0x7d92a230      UDPv6   ::      0       *       0               868     svchost.exe     2018-08-04 19:34:22.000000
0x7d9a9240      TCPv4   0.0.0.0 8733    0.0.0.0 0       LISTENING       4       System  -
0x7d9a9240      TCPv6   ::      8733    ::      0       LISTENING       4       System  -
0x7d9cecf0      TCPv4   192.168.202.131 50373   173.239.232.46  2997    CLOSED  2836    BitTorrent.exe   -
0x7d9d7cf0      TCPv4   192.168.202.131 50371   191.253.122.149 59163   CLOSED  2836    BitTorrent.exe   -
0x7d9e19e0      TCPv4   0.0.0.0 20830   0.0.0.0 0       LISTENING       2836    BitTorrent.exe  -
0x7d9e19e0      TCPv6   ::      20830   ::      0       LISTENING       2836    BitTorrent.exe  -
0x7d9e1c90      TCPv4   0.0.0.0 20830   0.0.0.0 0       LISTENING       2836    BitTorrent.exe  -
0x7d9e8b50      UDPv4   0.0.0.0 20830   *       0               2836    BitTorrent.exe  2018-08-04 19:27:15.000000
0x7d9f4560      UDPv4   0.0.0.0 0       *       0               3856    WebCompanion.e  2018-08-04 19:34:22.000000
0x7d9f8cb0      UDPv4   0.0.0.0 20830   *       0               2836    BitTorrent.exe  2018-08-04 19:27:15.000000
0x7d9f8cb0      UDPv6   ::      20830   *       0               2836    BitTorrent.exe  2018-08-04 19:27:15.000000
0x7daefec0      UDPv4   0.0.0.0 0       *       0               3856    WebCompanion.e  2018-08-04 19:34:22.000000
0x7daefec0      UDPv6   ::      0       *       0               3856    WebCompanion.e  2018-08-04 19:34:22.000000
0x7db000a0      TCPv4   -       50091   93.142.197.107  32645   CLOSED  2836    BitTorrent.exe  -
0x7db132e0      TCPv4   192.168.202.131 50280   72.55.154.81    80      CLOSED  3880    WebCompanionIn   N/A
0x7db83b90      UDPv4   0.0.0.0 0       *       0               3880    WebCompanionIn  2018-08-04 19:33:30.000000
0x7db83b90      UDPv6   ::      0       *       0               3880    WebCompanionIn  2018-08-04 19:33:30.000000
0x7db9cdd0      UDPv4   0.0.0.0 0       *       0               2844    WebCompanion.e  2018-08-04 19:30:05.000000
0x7db9cdd0      UDPv6   ::      0       *       0               2844    WebCompanion.e  2018-08-04 19:30:05.000000
0x7dbc3010      TCPv6   -       0       4847:d418:80fa:ffff:4847:d418:80fa:ffff 0       CLOSED  4076     chrome.exe      N/A
0x7dc2dc30      UDPv4   0.0.0.0 50879   *       0               4076    chrome.exe      2018-08-04 19:30:41.000000
0x7dc2dc30      UDPv6   ::      50879   *       0               4076    chrome.exe      2018-08-04 19:30:41.000000
0x7dc4ad30      TCPv4   0.0.0.0 49155   0.0.0.0 0       LISTENING       500     lsass.exe       -
0x7dc4ad30      TCPv6   ::      49155   ::      0       LISTENING       500     lsass.exe       -
0x7dc4b370      TCPv4   0.0.0.0 49155   0.0.0.0 0       LISTENING       500     lsass.exe       -
0x7dc83080      TCPv4   192.168.202.131 50377   179.108.238.10  19761   CLOSED  2836    BitTorrent.exe   -
0x7dc83810      UDPv4   0.0.0.0 5355    *       0               620     svchost.exe     2018-08-04 19:34:22.000000
0x7dc83810      UDPv6   ::      5355    *       0               620     svchost.exe     2018-08-04 19:34:22.000000
0x7dd451f0      TCPv4   192.168.202.131 50321   45.27.208.145   51414   CLOSED  2836    BitTorrent.exe   -
0x7dd71010      TCPv4   0.0.0.0 445     0.0.0.0 0       LISTENING       4       System  -
0x7dd71010      TCPv6   ::      445     ::      0       LISTENING       4       System  -
0x7dd82c30      UDPv4   0.0.0.0 5355    *       0               620     svchost.exe     2018-08-04 19:26:38.000000
0x7ddae890      TCPv4   -       50299   212.92.105.227  8999    CLOSED  2836    BitTorrent.exe  -
0x7ddca6b0      TCPv4   0.0.0.0 49156   0.0.0.0 0       LISTENING       492     services.exe    -
0x7ddcbc00      TCPv4   0.0.0.0 49156   0.0.0.0 0       LISTENING       492     services.exe    -
0x7ddcbc00      TCPv6   ::      49156   ::      0       LISTENING       492     services.exe    -
0x7ddff010      TCPv4   192.168.202.131 50379   23.37.43.27     80      CLOSED  3856    WebCompanion.e   -
0x7de09c30      TCPv4   0.0.0.0 49152   0.0.0.0 0       LISTENING       396     wininit.exe     -
0x7de09c30      TCPv6   ::      49152   ::      0       LISTENING       396     wininit.exe     -
0x7de0d7b0      TCPv4   0.0.0.0 49152   0.0.0.0 0       LISTENING       396     wininit.exe     -
0x7de424e0      TCPv4   0.0.0.0 49153   0.0.0.0 0       LISTENING       808     svchost.exe     -
0x7de45ef0      TCPv4   0.0.0.0 49153   0.0.0.0 0       LISTENING       808     svchost.exe     -
0x7de45ef0      TCPv6   ::      49153   ::      0       LISTENING       808     svchost.exe     -
0x7df00980      UDPv4   0.0.0.0 0       *       0               620     svchost.exe     2018-08-04 19:34:22.000000
0x7df00980      UDPv6   ::      0       *       0               620     svchost.exe     2018-08-04 19:34:22.000000
0x7df04cc0      UDPv4   0.0.0.0 5355    *       0               620     svchost.exe     2018-08-04 19:26:38.000000
0x7df04cc0      UDPv6   ::      5355    *       0               620     svchost.exe     2018-08-04 19:26:38.000000
0x7df3d270      TCPv4   0.0.0.0 49154   0.0.0.0 0       LISTENING       868     svchost.exe     -
0x7df3eef0      TCPv4   0.0.0.0 49154   0.0.0.0 0       LISTENING       868     svchost.exe     -
0x7df3eef0      TCPv6   ::      49154   ::      0       LISTENING       868     svchost.exe     -
0x7df5f010      UDPv4   0.0.0.0 55175   *       0               620     svchost.exe     2018-08-04 19:34:22.000000
0x7dfab010      UDPv4   0.0.0.0 58383   *       0               620     svchost.exe     2018-08-04 19:34:22.000000
0x7dfab010      UDPv6   ::      58383   *       0               620     svchost.exe     2018-08-04 19:34:22.000000
0x7e0057d0      TCPv4   192.168.202.131 50353   85.242.139.158  51413   CLOSED  2836    BitTorrent.exe   -
0x7e0114b0      TCPv4   192.168.202.131 50339   77.65.111.216   8306    CLOSED  2836    BitTorrent.exe   -
0x7e042cf0      TCPv4   192.168.202.131 50372   83.44.27.35     52103   CLOSED  2836    BitTorrent.exe   -
0x7e08a010      TCPv4   192.168.202.131 50374   89.46.49.163    20133   CLOSED  2836    BitTorrent.exe   -
0x7e092010      TCPv4   192.168.202.131 50378   120.29.114.41   13155   CLOSED  2836    BitTorrent.exe   -
0x7e094b90      TCPv4   192.168.202.131 50365   52.91.1.182     55125   CLOSED  2836    BitTorrent.exe   N/A
0x7e09ba90      TCPv6   -       0       68f0:181b:80fa:ffff:68f0:181b:80fa:ffff 0       CLOSED  2836     BitTorrent.exe  -
0x7e0a8b90      TCPv4   192.168.202.131 50341   72.55.154.81    80      CLOSED  3880    WebCompanionIn   N/A
0x7e0d6180      TCPv4   192.168.202.131 50349   196.250.217.22  32815   CLOSED  2836    BitTorrent.exe   -
0x7e108100      TCPv4   192.168.202.131 50360   174.0.234.77    31240   CLOSED  2836    BitTorrent.exe   -
0x7e124910      TCPv4   192.168.202.131 50366   89.78.106.196   51413   CLOSED  2836    BitTorrent.exe   -
0x7e12c1c0      UDPv4   0.0.0.0 0       *       0               3880    WebCompanionIn  2018-08-04 19:33:27.000000
0x7e14dcf0      TCPv4   192.168.202.131 50363   122.62.218.159  11627   CLOSED  2836    BitTorrent.exe   N/A
0x7e163a40      UDPv4   0.0.0.0 0       *       0               3880    WebCompanionIn  2018-08-04 19:33:27.000000
0x7e163a40      UDPv6   ::      0       *       0               3880    WebCompanionIn  2018-08-04 19:33:27.000000
0x7e18bcf0      TCPv4   192.168.202.131 50333   191.177.124.34  21011   CLOSED  2836    BitTorrent.exe   -
0x7e1cf010      UDPv4   192.168.202.131 137     *       0               4       System  2018-08-04 19:26:35.000000
0x7e1da010      UDPv4   192.168.202.131 138     *       0               4       System  2018-08-04 19:26:35.000000
0x7e1f6010      TCPv4   0.0.0.0 135     0.0.0.0 0       LISTENING       712     svchost.exe     -
0x7e1f6010      TCPv6   ::      135     ::      0       LISTENING       712     svchost.exe     -
0x7e1f8ef0      TCPv4   0.0.0.0 135     0.0.0.0 0       LISTENING       712     svchost.exe     -
0x7e413a40      TCPv4   -       0       -       0       CLOSED  708     LunarMS.exe     -
0x7e415010      TCPv4   192.168.202.131 50346   89.64.10.176    10589   CLOSED  2836    BitTorrent.exe   -
0x7e4202d0      TCPv4   192.168.202.131 50217   104.18.21.226   80      CLOSED  3880    WebCompanionIn   N/A
0x7e45f110      TCPv4   192.168.202.131 50211   104.18.20.226   80      CLOSED  3880    WebCompanionIn   N/A
0x7e48d9c0      UDPv6   fe80::b06b:a531:ec88:457f       1900    *       0               164     svchost.exe      2018-08-04 19:28:42.000000
0x7e4ad870      UDPv4   127.0.0.1       1900    *       0               164     svchost.exe     2018-08-04 19:28:42.000000
0x7e4cc910      TCPv4   192.168.202.131 50228   104.18.20.226   80      CLOSED  3880    WebCompanionIn   N/A
0x7e511bb0      UDPv4   0.0.0.0 60005   *       0               620     svchost.exe     2018-08-04 19:34:22.000000
0x7e512950      TCPv4   192.168.202.131 50345   77.126.30.221   13905   CLOSED  2836    BitTorrent.exe   -
0x7e521b50      TCPv4   -       0       -       0       CLOSED  708     LunarMS.exe     -
0x7e5228d0      TCPv4   192.168.202.131 50075   70.65.116.120   52700   CLOSED  2836    BitTorrent.exe   -
0x7e52f010      TCPv4   192.168.202.131 50343   86.121.4.189    46392   CLOSED  2836    BitTorrent.exe   -
0x7e563860      TCPv4   192.168.202.131 50170   103.232.25.44   25384   CLOSED  2836    BitTorrent.exe   -
0x7e572cf0      TCPv4   192.168.202.131 50125   122.62.218.159  11627   CLOSED  2836    BitTorrent.exe   -
0x7e5d6cf0      TCPv4   192.168.202.131 50324   54.197.8.177    49420   CLOSED  2836    BitTorrent.exe   -
0x7e5dc3b0      UDPv6   fe80::b06b:a531:ec88:457f       546     *       0               808     svchost.exe      2018-08-04 19:33:28.000000
0x7e71b010      TCPv4   192.168.202.131 50344   70.27.98.75     6881    CLOSED  2836    BitTorrent.exe   -
0x7e71d010      TCPv4   192.168.202.131 50351   99.251.199.160  1045    CLOSED  2836    BitTorrent.exe   -
0x7e7469c0      UDPv4   0.0.0.0 50878   *       0               4076    chrome.exe      2018-08-04 19:30:39.000000
0x7e7469c0      UDPv6   ::      50878   *       0               4076    chrome.exe      2018-08-04 19:30:39.000000
0x7e74b010      TCPv4   192.168.202.131 50385   209.236.6.89    56500   CLOSED  2836    BitTorrent.exe   -
0x7e77cb00      UDPv4   0.0.0.0 50748   *       0               4076    chrome.exe      2018-08-04 19:30:07.000000
0x7e77cb00      UDPv6   ::      50748   *       0               4076    chrome.exe      2018-08-04 19:30:07.000000
0x7e78b7f0      TCPv4   192.168.202.131 50238   72.55.154.82    80      CLOSED  3880    WebCompanionIn   N/A
0x7e79f3f0      UDPv4   0.0.0.0 5353    *       0               4076    chrome.exe      2018-08-04 19:29:35.000000
0x7e7a0ec0      UDPv4   0.0.0.0 5353    *       0               4076    chrome.exe      2018-08-04 19:29:35.000000
0x7e7a0ec0      UDPv6   ::      5353    *       0               4076    chrome.exe      2018-08-04 19:29:35.000000
0x7e7a3960      UDPv4   0.0.0.0 0       *       0               3880    WebCompanionIn  2018-08-04 19:33:30.000000
0x7e7ae380      TCPv4   192.168.202.131 50361   5.34.21.181     8999    CLOSED  2836    BitTorrent.exe   -
0x7e7b0380      TCPv6   -       0       4847:d418:80fa:ffff:4847:d418:80fa:ffff 0       CLOSED  2836     BitTorrent.exe  N/A
0x7e7b9010      TCPv4   192.168.202.131 50334   188.129.94.129  25128   CLOSED  2836    BitTorrent.exe   N/A
0x7e7dd010      UDPv6   ::1     58340   *       0               164     svchost.exe     2018-08-04 19:28:42.000000
0x7e94b010      TCPv4   192.168.202.131 50356   77.126.30.221   13905   CLOSED  2836    BitTorrent.exe   -
0x7e9ad840      TCPv4   192.168.202.131 50380   84.52.144.29    56299   CLOSED  2836    BitTorrent.exe   -
0x7e9bacf0      TCPv4   192.168.202.131 50350   77.253.242.0    5000    CLOSED  2836    BitTorrent.exe   -
0x7eaac5e0      TCPv4   192.168.202.131 50387   93.184.220.29   80      CLOSED  3856    WebCompanion.e   -
0x7eab4cf0      TCPv4   -       0       56.219.196.26   0       CLOSED  2836    BitTorrent.exe  N/A
0x7fb9cec0      UDPv4   192.168.202.131 1900    *       0               164     svchost.exe     2018-08-04 19:28:42.000000
0x7fb9d430      UDPv4   127.0.0.1       58341   *       0               164     svchost.exe     2018-08-04 19:28:42.000000
```


# windows.netscan.NetScan 分析

## 1. Plugin 功能說明

`windows.netscan.NetScan` 用來掃描記憶體中的網路連線資訊。

它可以查看：

* TCP / UDP 連線
* Local IP 與 Local Port
* Foreign IP 與 Foreign Port
* 連線狀態
* 對應的 PID 與 Process
* 連線建立時間

此 Plugin 可用來判斷哪個 Process 有網路活動，以及是否存在可疑外連行為。

---

## 2. Plugin 欄位說明

| 欄位            | 說明                         |
| ------------- | -------------------------- |
| `Offset`      | 網路連線物件在記憶體中的位置             |
| `Proto`       | 通訊協定，例如 TCPv4、UDPv4、TCPv6  |
| `LocalAddr`   | 本機 IP 位址                   |
| `LocalPort`   | 本機 Port                    |
| `ForeignAddr` | 遠端 IP 位址                   |
| `ForeignPort` | 遠端 Port                    |
| `State`       | TCP 狀態，例如 LISTENING、CLOSED |
| `PID`         | 對應 Process ID              |
| `Owner`       | 對應 Process 名稱              |
| `Created`     | 連線建立時間                     |

---

## 3. 本機 IP 判斷

本次主要本機 IP 為：

```text
192.168.202.131
```

此 IP 應為虛擬機中的內部網路位址。

---

## 4. BitTorrent.exe 網路活動

### 4.1 主要發現

`PID 2836 BitTorrent.exe` 有大量 TCP 與 UDP 連線紀錄。

```
D:\Forensic\G140A006\VolatilityWorkbench>.\vol.exe -f .\OtterCTF.vmem windows.netscan.NetScan | findstr 2836
0x7d42ba90 100.0TCPv4   -       0DB scan56.219.196.26   0       CLOSED  2836    BitTorrent.exe  N/A
0x7d60f010      UDPv4   0.0.0.0 1900    *       0               2836    BitTorrent.exe  2018-08-04 19:27:17.000000
0x7d62b3f0      UDPv4   192.168.202.131 6771    *       0               2836    BitTorrent.exe  2018-08-04 19:27:22.000000
0x7d62d690      TCPv4   192.168.202.131 49229   169.1.143.215   8999    CLOSED  2836    BitTorrent.exe   N/A
0x7d62f4c0      UDPv4   127.0.0.1       62307   *       0               2836    BitTorrent.exe  2018-08-04 19:27:17.000000
0x7d62f920      UDPv4   192.168.202.131 62306   *       0               2836    BitTorrent.exe  2018-08-04 19:27:17.000000
0x7d634350      TCPv6   -       0       38db:c41a:80fa:ffff:38db:c41a:80fa:ffff 0       CLOSED  2836     BitTorrent.exe  N/A
0x7d6e3230      UDPv4   127.0.0.1       6771    *       0               2836    BitTorrent.exe  2018-08-04 19:27:22.000000
0x7d6f27f0      TCPv4   192.168.202.131 50381   71.198.155.180  34674   CLOSED  2836    BitTorrent.exe   -
0x7d704010      TCPv4   192.168.202.131 50382   92.251.23.204   6881    CLOSED  2836    BitTorrent.exe   -
0x7d708cf0      TCPv4   192.168.202.131 50364   91.140.89.116   31847   CLOSED  2836    BitTorrent.exe   -
0x7d729620      TCPv4   -       50034   142.129.37.27   24578   CLOSED  2836    BitTorrent.exe  -
0x7d81c890      TCPv4   192.168.202.131 50335   185.154.111.20  60405   CLOSED  2836    BitTorrent.exe   -
0x7d9cecf0      TCPv4   192.168.202.131 50373   173.239.232.46  2997    CLOSED  2836    BitTorrent.exe   -
0x7d9d7cf0      TCPv4   192.168.202.131 50371   191.253.122.149 59163   CLOSED  2836    BitTorrent.exe   -
0x7d9e19e0      TCPv4   0.0.0.0 20830   0.0.0.0 0       LISTENING       2836    BitTorrent.exe  -
0x7d9e19e0      TCPv6   ::      20830   ::      0       LISTENING       2836    BitTorrent.exe  -
0x7d9e1c90      TCPv4   0.0.0.0 20830   0.0.0.0 0       LISTENING       2836    BitTorrent.exe  -
0x7d9e8b50      UDPv4   0.0.0.0 20830   *       0               2836    BitTorrent.exe  2018-08-04 19:27:15.000000
0x7d9f8cb0      UDPv4   0.0.0.0 20830   *       0               2836    BitTorrent.exe  2018-08-04 19:27:15.000000
0x7d9f8cb0      UDPv6   ::      20830   *       0               2836    BitTorrent.exe  2018-08-04 19:27:15.000000
0x7db000a0      TCPv4   -       50091   93.142.197.107  32645   CLOSED  2836    BitTorrent.exe  -
0x7dc83080      TCPv4   192.168.202.131 50377   179.108.238.10  19761   CLOSED  2836    BitTorrent.exe   -
0x7dd451f0      TCPv4   192.168.202.131 50321   45.27.208.145   51414   CLOSED  2836    BitTorrent.exe   -
0x7ddae890      TCPv4   -       50299   212.92.105.227  8999    CLOSED  2836    BitTorrent.exe  -
0x7e0057d0      TCPv4   192.168.202.131 50353   85.242.139.158  51413   CLOSED  2836    BitTorrent.exe   -
0x7e0114b0      TCPv4   192.168.202.131 50339   77.65.111.216   8306    CLOSED  2836    BitTorrent.exe   -
0x7e042cf0      TCPv4   192.168.202.131 50372   83.44.27.35     52103   CLOSED  2836    BitTorrent.exe   -
0x7e08a010      TCPv4   192.168.202.131 50374   89.46.49.163    20133   CLOSED  2836    BitTorrent.exe   -
0x7e092010      TCPv4   192.168.202.131 50378   120.29.114.41   13155   CLOSED  2836    BitTorrent.exe   -
0x7e094b90      TCPv4   192.168.202.131 50365   52.91.1.182     55125   CLOSED  2836    BitTorrent.exe   N/A
0x7e09ba90      TCPv6   -       0       68f0:181b:80fa:ffff:68f0:181b:80fa:ffff 0       CLOSED  2836     BitTorrent.exe  -
0x7e0d6180      TCPv4   192.168.202.131 50349   196.250.217.22  32815   CLOSED  2836    BitTorrent.exe   -
0x7e108100      TCPv4   192.168.202.131 50360   174.0.234.77    31240   CLOSED  2836    BitTorrent.exe   -
0x7e124910      TCPv4   192.168.202.131 50366   89.78.106.196   51413   CLOSED  2836    BitTorrent.exe   -
0x7e14dcf0      TCPv4   192.168.202.131 50363   122.62.218.159  11627   CLOSED  2836    BitTorrent.exe   N/A
0x7e18bcf0      TCPv4   192.168.202.131 50333   191.177.124.34  21011   CLOSED  2836    BitTorrent.exe   -
0x7e415010      TCPv4   192.168.202.131 50346   89.64.10.176    10589   CLOSED  2836    BitTorrent.exe   -
0x7e512950      TCPv4   192.168.202.131 50345   77.126.30.221   13905   CLOSED  2836    BitTorrent.exe   -
0x7e5228d0      TCPv4   192.168.202.131 50075   70.65.116.120   52700   CLOSED  2836    BitTorrent.exe   -
0x7e52f010      TCPv4   192.168.202.131 50343   86.121.4.189    46392   CLOSED  2836    BitTorrent.exe   -
0x7e563860      TCPv4   192.168.202.131 50170   103.232.25.44   25384   CLOSED  2836    BitTorrent.exe   -
0x7e572cf0      TCPv4   192.168.202.131 50125   122.62.218.159  11627   CLOSED  2836    BitTorrent.exe   -
0x7e5d6cf0      TCPv4   192.168.202.131 50324   54.197.8.177    49420   CLOSED  2836    BitTorrent.exe   -
0x7e71b010      TCPv4   192.168.202.131 50344   70.27.98.75     6881    CLOSED  2836    BitTorrent.exe   -
0x7e71d010      TCPv4   192.168.202.131 50351   99.251.199.160  1045    CLOSED  2836    BitTorrent.exe   -
0x7e74b010      TCPv4   192.168.202.131 50385   209.236.6.89    56500   CLOSED  2836    BitTorrent.exe   -
0x7e7ae380      TCPv4   192.168.202.131 50361   5.34.21.181     8999    CLOSED  2836    BitTorrent.exe   -
0x7e7b0380      TCPv6   -       0       4847:d418:80fa:ffff:4847:d418:80fa:ffff 0       CLOSED  2836     BitTorrent.exe  N/A
0x7e7b9010      TCPv4   192.168.202.131 50334   188.129.94.129  25128   CLOSED  2836    BitTorrent.exe   N/A
0x7e94b010      TCPv4   192.168.202.131 50356   77.126.30.221   13905   CLOSED  2836    BitTorrent.exe   -
0x7e9ad840      TCPv4   192.168.202.131 50380   84.52.144.29    56299   CLOSED  2836    BitTorrent.exe   -
0x7e9bacf0      TCPv4   192.168.202.131 50350   77.253.242.0    5000    CLOSED  2836    BitTorrent.exe   -
0x7eab4cf0      TCPv4   -       0       56.219.196.26   0       CLOSED  2836    BitTorrent.exe  N/A
```

常見遠端 Port 包含：

```text
6881
8999
51413
51414
60405
59163
34674
```

這些連線多數為 `CLOSED`，代表在記憶體擷取前曾經存在過連線。

### 4.2 監聽 Port

`BitTorrent.exe` 也有監聽行為：

```text
0.0.0.0:20830 LISTENING PID 2836 BitTorrent.exe
:::20830 LISTENING PID 2836 BitTorrent.exe
```

另外也有 UDP：

```text
0.0.0.0:20830 PID 2836 BitTorrent.exe
```

### 4.3 分析判斷

`BitTorrent.exe` 的大量外部 IP 連線與監聽 Port 符合 P2P 軟體行為。

此結果支持前面判斷：

```text
系統當時有 BitTorrent 下載活動。
```

由於本案中可疑檔案 `Rick And Morty season 1 download.exe` 位於 `Torrents` 目錄，因此 BitTorrent 活動可能與可疑檔案來源有關。

---

## 5. WebCompanion 相關連線

### 5.1 WebCompanionInstaller.exe

`PID 3880 WebCompanionIn` 有多筆 HTTP 連線：

```
D:\Forensic\G140A006\VolatilityWorkbench>.\vol.exe -f .\OtterCTF.vmem windows.netscan.NetScan | findstr 3880
0x7db132e0 100.0TCPv4   192.168.202.131n50280fin72.55.154.81    80      CLOSED  3880    WebCompanionIn   N/A
0x7db83b90      UDPv4   0.0.0.0 0       *       0               3880    WebCompanionIn  2018-08-04 19:33:30.000000
0x7db83b90      UDPv6   ::      0       *       0               3880    WebCompanionIn  2018-08-04 19:33:30.000000
0x7e0a8b90      TCPv4   192.168.202.131 50341   72.55.154.81    80      CLOSED  3880    WebCompanionIn   N/A
0x7e12c1c0      UDPv4   0.0.0.0 0       *       0               3880    WebCompanionIn  2018-08-04 19:33:27.000000
0x7e163a40      UDPv4   0.0.0.0 0       *       0               3880    WebCompanionIn  2018-08-04 19:33:27.000000
0x7e163a40      UDPv6   ::      0       *       0               3880    WebCompanionIn  2018-08-04 19:33:27.000000
0x7e4202d0      TCPv4   192.168.202.131 50217   104.18.21.226   80      CLOSED  3880    WebCompanionIn   N/A
0x7e45f110      TCPv4   192.168.202.131 50211   104.18.20.226   80      CLOSED  3880    WebCompanionIn   N/A
0x7e4cc910      TCPv4   192.168.202.131 50228   104.18.20.226   80      CLOSED  3880    WebCompanionIn   N/A
0x7e78b7f0      TCPv4   192.168.202.131 50238   72.55.154.82    80      CLOSED  3880    WebCompanionIn   N/A
0x7e7a3960      UDPv4   0.0.0.0 0       *       0               3880    WebCompanionIn  2018-08-04 19:33:30.000000
```

```text
192.168.202.131:50280 → 72.55.154.81:80
192.168.202.131:50341 → 72.55.154.81:80
192.168.202.131:50217 → 104.18.21.226:80
192.168.202.131:50211 → 104.18.20.226:80
192.168.202.131:50228 → 104.18.20.226:80
192.168.202.131:50238 → 72.55.154.82:80
```

### 5.2 WebCompanion.exe / Lavasoft.WCAss

也看到：

```text
PID 3856 WebCompanion.e → 23.37.43.27:80
PID 3856 WebCompanion.e → 93.184.220.29:80
PID 3496 Lavasoft.WCAss → 23.37.43.27:80
```

### 5.3 分析判斷

這些連線多為 HTTP Port 80，符合 WebCompanion 安裝、更新或下載資料的行為。

WebCompanion 相關 Process 先前已出現服務操作線索，因此這些網路連線可以判斷為：

```text
WebCompanion 安裝 / 更新 / 下載行為
```

可疑程度低於 `Rick And Morty` 執行鏈，但仍可列為 PUP 或軟體更新行為。

---

## 6. LunarMS.exe 網路活動

`PID 708 LunarMS.exe` 有 TCP 連線紀錄：

```
D:\Forensic\G140A006\VolatilityWorkbench>.\vol.exe -f .\OtterCTF.vmem windows.netscan.NetScan | findstr 708
0x7d6124d0 100.0TCPv4   192.168.202.131n49530fin77.102.199.102  7575    CLOSED  708     LunarMS.exe      -
0x7d708cf0      TCPv4   192.168.202.131 50364   91.140.89.116   31847   CLOSED  2836    BitTorrent.exe   -
0x7e413a40      TCPv4   -       0       -       0       CLOSED  708     LunarMS.exe     -
0x7e521b50      TCPv4   -       0       -       0       CLOSED  708     LunarMS.exe     -

```

```text
192.168.202.131:49530 → 77.102.199.102:7575 CLOSED
```

另外也有幾筆 `LocalAddr` 與 `ForeignAddr` 不完整的 CLOSED 紀錄。

### 分析判斷

`LunarMS.exe` 可能是遊戲程式，因此存在網路連線不一定異常。

但因為前面 `LdrModules` 發現它載入多個 Temp `.tmp` 模組，所以此 Process 仍建議保留為中等注意項目。

---

## 7. Chrome 網路活動

`PID 4076 chrome.exe` 有多筆 UDP 連線，例如：

```text
0.0.0.0:50762
0.0.0.0:65452
0.0.0.0:5353
```

```
D:\Forensic\G140A006\VolatilityWorkbench>.\vol.exe -f .\OtterCTF.vmem windows.netscan.NetScan | findstr 4076
0x7d6424c0 100.0UDPv4   0.0.0.0 50762can*ing fin0shed           4076    chrome.exe      2018-08-04 19:33:37.000000
0x7d787010      UDPv4   0.0.0.0 65452   *       0               4076    chrome.exe      2018-08-04 19:33:42.000000
0x7dbc3010      TCPv6   -       0       4847:d418:80fa:ffff:4847:d418:80fa:ffff 0       CLOSED  4076     chrome.exe      N/A
0x7dc2dc30      UDPv4   0.0.0.0 50879   *       0               4076    chrome.exe      2018-08-04 19:30:41.000000
0x7dc2dc30      UDPv6   ::      50879   *       0               4076    chrome.exe      2018-08-04 19:30:41.000000
0x7e7469c0      UDPv4   0.0.0.0 50878   *       0               4076    chrome.exe      2018-08-04 19:30:39.000000
0x7e7469c0      UDPv6   ::      50878   *       0               4076    chrome.exe      2018-08-04 19:30:39.000000
0x7e77cb00      UDPv4   0.0.0.0 50748   *       0               4076    chrome.exe      2018-08-04 19:30:07.000000
0x7e77cb00      UDPv6   ::      50748   *       0               4076    chrome.exe      2018-08-04 19:30:07.000000
0x7e79f3f0      UDPv4   0.0.0.0 5353    *       0               4076    chrome.exe      2018-08-04 19:29:35.000000
0x7e7a0ec0      UDPv4   0.0.0.0 5353    *       0               4076    chrome.exe      2018-08-04 19:29:35.000000
0x7e7a0ec0      UDPv6   ::      5353    *       0               4076    chrome.exe      2018-08-04 19:29:35.000000

```



### 分析判斷

Chrome 出現 UDP 與瀏覽器相關連線屬於常見行為，目前不是主要可疑點。

---

## 8. 系統正常監聽服務

結果中也有多個 Windows 正常服務監聽 Port，例如：

```text
0.0.0.0:135   svchost.exe
0.0.0.0:445   System
0.0.0.0:49152 wininit.exe
0.0.0.0:49153 svchost.exe
0.0.0.0:49154 svchost.exe
0.0.0.0:49155 lsass.exe
0.0.0.0:49156 services.exe
```

### 分析判斷

這些多屬於 Windows RPC、SMB、系統服務或動態 Port，沒有明顯異常。

---

## 9. 可疑程度整理

|  PID | Process          | 網路行為               | 判斷                |
| ---: | ---------------- | ------------------ | ----------------- |
| 2836 | `BitTorrent.exe` | 大量 P2P 連線、監聽 20830 | 與可疑下載來源有關         |
| 3880 | `WebCompanionIn` | 多筆 HTTP 80 連線      | 安裝 / 更新 / 下載行為    |
| 3856 | `WebCompanion.e` | HTTP 80 連線         | WebCompanion 行為   |
| 3496 | `Lavasoft.WCAss` | HTTP 80 連線         | WebCompanion 服務行為 |
|  708 | `LunarMS.exe`    | 對外 TCP 連線          | 中等注意              |
| 4076 | `chrome.exe`     | 一般瀏覽器 UDP 連線       | 較正常               |

---

## 10. 結論

`windows.netscan.NetScan` 結果顯示，系統中最明顯的網路活動來自 `BitTorrent.exe`。

`BitTorrent.exe` 有大量外部 IP 連線，並且監聽 `20830` Port，符合 P2P 下載軟體行為。這與前面發現的可疑檔案：

```text
\Torrents\Rick And Morty season 1 download.exe
```

具有關聯性，表示該可疑 EXE 可能來自 Torrent 下載活動。

另外，`WebCompanionInstaller.exe`、`WebCompanion.exe` 與 `Lavasoft.WCAss` 有多筆 HTTP Port 80 連線，符合安裝、更新或下載資料行為。

`LunarMS.exe` 也有對外連線紀錄，但目前可疑程度低於 BitTorrent 與 `Rick And Morty` 執行鏈。

整體判斷，本次 `netscan` 支持以下重點：

```text
BitTorrent.exe 存在大量 P2P 網路活動。
可疑檔案 Rick And Morty season 1 download.exe 可能與 Torrent 下載活動有關。
WebCompanion 相關 Process 有 HTTP 更新 / 下載行為。
目前主要可疑線索仍集中在 Rick And Morty 與 vmware-tray.exe 執行鏈。
```
