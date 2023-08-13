Rhysida Ransomware

Encrypted files will have file extension as ".rhysida" 
This Ransomware arrives on a system as a file dropped by other malware or as a file downloaded unknowingly by users when visiting malicious sites.
</br>It drops the following file(s) as ransom note:</br>
CriticalBreachDetected.pdf

Knowledge Base:</br>
Initial Access: Phishing,Remote Desktop Protocol,Public-facing applications,Brokers </br>
Tunneling : Utilize "Chisel" tools: which is a fast TCP/UDP tunnel, transported over HTTP, secured via SSH </br>
Lateral Movement: PsExec  </br>
persistence: AnyDesk, LogMeIn, Atera </br>
Data Exfiltration: Cobalt Strike,Ursnif/Gozi </br>
vssadmin.exe to delete volume Shadow Copy</br>

| S.No | Indicator            | Type   | Comment |
|:-----:|:----------------|:---------|:--------------------|
|1  |C:\Temp\ | Folder Location  |  Check for any suspicious or unusual files in the given Location |

|77|2598e8adb87976abe48f0eba4bbb9a7cb69439e0c133b21aee3845dfccf3fb8f |SHA256  |  - |

</br>
Note: Before blocking any IP Address, Please investigate it </br>
</br>
<ul>
<li>
This Ransomware avoids encrypting files with the following strings in their file name:
</br>CriticalBreachDetected.pdf
</br>CriticalBreachDetected
</li>

<li>
It avoids encrypting files found in the following folders:</br>
Recycle.Bin</br>
Boot</br>
Documents and Settings</br>
PerfLogs</br>
System Volume Information</br>
Windows</br>
AppDat</br>
</li>

<li>
It avoids encrypting files with the following file extensions:

.bat
.bin
.cab
.cmd
.com
.cur
.diagcab
.diagcfg
.diagpkg
.drv
.dll
.exe
.hlp
.hta
.ico
.lnk
.msi
.ocx
.ps1
.psm1
.scr
.sys
.sys
.ini
.db
.url
.iso
.rhysida
</li>

</ul>
Reference:</br>
1.https://www.trendmicro.com/vinfo/us/threat-encyclopedia/malware/Ransom.PS1.RHYSIDA.SM/</br>