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
