8Base ransomware
It appends encrypted files with the extension “.8base”. Uses AES to Encrypt Files

| S.No | Indicator            | Type   | Comment |
|:-----:|:----------------|:---------|:--------------------|
|1  | wlaexfpxrs[.]org  | Domain  |  Web Request |
|2  | admhexlogs25[.]xyz	  | Domain  |  Web Request |
|3  | admlogs25[.]xyz		  | Domain  |  Web Request |
|4  | admlog2[.]xyz		  | Domain  |  Web Request |
|5  | dnm777[.]xyz			  | Domain  |  Web Request |
|6  | serverlogs37[.]xyz			  | Domain  |  Web Request |
|7  | dexblog[.]xyz				  | Domain  |  Web Request |
|8  | blogstat355[.]xyz				  | Domain  |  Web Request |
|9  | blogstatserv25[.]xyz				  | Domain  |  Web Request |
|10  | 9f1a.exe				  | File  |  - |
|11  | d6ff.exe			  | File  |  - |
|12  | 3c1e.exe			  | File  |  - |
|13  | 3c1e.exe			  | File  |  - |
|14  | 518544e56e8ccee401ffa1b0a01a10ce23e49ec21ec441c6c7c3951b01c1b19c  | SHA256  |  - |
|15 | 5BA74A5693F4810A8EB9B9EEB1D69D943CF5BBC46F319A32802C23C7654194B0  | SHA256  |  - |
|16 | 20110FF550A2290C5992A5BB6BB44056  | MD5  |  - |
|17 | 9769c181ecef69544bbb2f974b8c0e10  | MD5  |  - |
|18 | 3D2B088A397E9C7E9AD130E178F885FEEBD9688B  | SHA-1  |  - |
|19 | e142f4e8eb3fb4323fb377138f53db66e3e6ec9e82930f4b23dd91a5f7bd45d0  | SHA256  |  - |
|20  | C6BD5B8E14551EB899BBE4DECB6942581D28B2A42B159146BBC28316E6E14A64  | SHA256  |  - |
|21  | 518544E56E8CCEE401FFA1B0A01A10CE23E49EC21EC441C6C7C3951B01C1B19C  | SHA256  |  - |
|22  | AFDDEC37CDC1D196A1136E2252E925C0DCFE587963069D78775E0F174AE9CFE3  | SHA256  |  - |
|23  | 5d0f447f4ccc89d7d79c0565372195240cdfa25f  | SHA-1  |  - |


Knowledge Base:</br>
Network Share Discovery -> WNetEnumResource()</br> 
"Obfuscated File or Information-> SmokeLoader" </br>
"wmic shadowcopy delete"</br>
"wbadmin delete catalog -quiet"</br>
"vssadmin delete shadows /all /quiet"</br>
"bcdedit /set {default} recoveryenabled no"</br>
"bcdedit /set {default} bootstatuspolicy ignoreallfailures"</br>



Reference:
1. https://blogs.vmware.com/security/2023/06/8base-ransomware-a-heavy-hitting-player.html
2. https://www.bleepingcomputer.com/news/security/8base-ransomware-gang-escalates-double-extortion-attacks-in-june/