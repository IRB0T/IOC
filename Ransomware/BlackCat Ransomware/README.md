BlackCat ransomware (aka ALPHV)
BlackCat/ALPHV ransomware leverages previously compromised user credentials to gain initial access to the victim system.

| S.No | Indicator            | Type   | Comment |
|:-----:|:----------------|:---------|:--------------------|
|1  | amd - Copy.ps1  | Filename  |  PowerShell Script |
|2  | ipscan.ps1  | Filename  |  PowerShell Script |
|3  | Run1.ps1  | Filename  |  PowerShell Script |
|4  | [###].ps1  | Filename  |  PowerShell Script |
|5  | [#].ps1  | Filename  |  PowerShell Script |
|6  | mim.ps1  | Filename  |  PowerShell Script |
|7  | psexec.ps1  | Filename  |  PowerShell Script |
|8  | System.ps1  | Filename  |  PowerShell Script |
|9  | CME.ps1  | Filename  |  PowerShell Script |
|10  | Systems.ps1  | Filename  |  PowerShell Script |
|11  | CheckVuln.bat  | Filename  |  Batch Script |
|12  | Create-share-RunAsAdmin.bat  | Filename  |  Batch Script |
|13  | LPE-Exploit-RunAsUser.bat  | Filename  |  Batch Script |
|14  | RCE-Exploit-RunAsUser.bat  | Filename  |  Batch Script |
|15  | est.bat  | Filename  |  Batch Script |
|16  | runav.bat  | Filename  |  Batch Script |
|17  | http_x64.exe  | Filename  |  Executable/Dlls |
|18  | spider.dll  | Filename  |  Executable/Dlls |
|19  | spider_32.dll  | Filename  |  Executable/Dlls |
|20  | powershell.dll  | Filename  |  Executable/Dlls |
|21  | rpcdump.exe  | Filename  |  Executable/Dlls |
|22  | mimikatz.exe  | Filename  |  Executable/Dlls |
|23  | run.exe  | Filename  |  Executable/Dlls |
|24  | zakrep_plink.exe  | Filename  |  Executable/Dlls |
|25  | beacon.exe  | Filename  |  Executable/Dlls |
|26  | win1999.exe  | Filename  |  Executable/Dlls |
|27  | test.exe  | Filename  |  Executable/Dlls |
|28  | Mim.exe  | Filename  |  Executable/Dlls |
|29  | crackmapexec.exe  | Filename  |  Executable/Dlls |
|30  | plink.exe  | Filename  |  Executable/Dlls |
|31  | PsExec64.exe  | Filename  |  Executable/Dlls |
|32  | xxx.exe  | Filename  |  Executable/Dlls |
|33  | xxxw.exe  | Filename  |  Executable/Dlls |
|34  | Services.exe  | Filename  |  Executable/Dlls |
|35  | Systems.exe  | Filename  |  Executable/Dlls |
|36  | 731adcf2d7fb61a8335e23dbee2436249e5d5753977ec465754c6b699e9bf161| SHA256  |  - |
|37  | f837f1cd60e9941aa60f7be50a8f2aaaac380f560db8ee001408f35c1b7a97cb| SHA256  |  - |
|38  | 80dd44226f60ba5403745ba9d18490eb8ca12dbc9be0a317dd2b692ec041da28| SHA256  |  - |
|39  | 67d1f4077e929385cfd869bf279892bf10a2c8f0af4119e4bc15a2add9461fec| SHA256  |  - |
|40  | 0a609fa2db910615b2c1ad235ca46562ff4034800c44802a63a28826669a7eee| SHA256  |  - |
|41  | cda37b13d1fdee1b4262b5a6146a35d8fc88fa572e55437a47a950037cc65d40| SHA256  |  - |
|42  | bacedbb23254934b736a9daf6de52620c9250a49686d519ceaf0a8d25da0a97f| SHA256  |  - |
|43  | 89.44.9.243  | IP Address  |  Malicious/Suspicious IPs (C2) |
|44  | 37.120.238.58  | IP Address  |  Malicious/Suspicious IPs (C2) |
|45  | 45.153.160.140  | IP Address  |  Malicious/Suspicious IPs (C2) |
|46  | 94.232.41.155  | IP Address  |  Malicious/Suspicious IPs (C2) |
|47  | 142.234.157.246  | IP Address  |  Malicious/Suspicious IPs (C2) |
|48  | 152.89.247.207  | IP Address  |  Malicious/Suspicious IPs (C2) |
|49  | 23.106.223.97 | IP Address  |  Malicious/Suspicious IPs (C2) |
|50  | 45.134.20.66 | IP Address  |  Malicious/Suspicious IPs (C2) |
|51  | 198.144.121.93 | IP Address  |  Malicious/Suspicious IPs (C2) |
|52  | 139.60.161.161 | IP Address  |  Malicious/Suspicious IPs (C2) |
|53  | 185.220.102.253 | IP Address  |  Malicious/Suspicious IPs (C2) |
|54  | 89.163.252.230 | IP Address  |  Malicious/Suspicious IPs (C2) |
|55  | 146.0.77.15 | IP Address  |  Malicious/Suspicious IPs (C2) |
|56  | 51.83.57.149 | IP Address  |  Malicious/Suspicious IPs (C2) |
|57  | 5.255.100.242 | IP Address  |  Malicious/Suspicious IPs (C2) |

Knowledge Base:</br>
Windows Task Scheduler is used to configure malicious Group Policy Objects (GPOs) to deploy ransomware. </br>
Cobalt Strike </br>
Review domain controllers, servers, workstations, and active directories for new or unrecognized user accounts. </br>
Review antivirus logs for indications they were unexpectedly turned off. </br>



Reference:
1.https://www.ic3.gov/Media/News/2022/220420.pdf
2.https://documents.trendmicro.com/assets/txt/IOCs-BlackCat-Ransomware-Spotlight-XUzqSpm.txt
3.https://www.csk.gov.in/alerts/BlackCat_ransomware.html