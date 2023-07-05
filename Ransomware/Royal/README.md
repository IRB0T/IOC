Royal Ransomware

Encrypted files will have file extension as ".royal " 
Royal ransomware uses a unique partial encryption approach that allows the threat actor to choose a specific percentage of data in a file to encrypt.

| S.No | Indicator            | Type   | Comment |
|:-----:|:----------------|:---------|:--------------------|
|1  |C:\Temp\ | Folder Location  |  Check for any suspicious or unusual files in the given Location |
|2  |C:\Users\<user>\AppData\Roaming\ | Folder Location  |  Check for any suspicious or unusual files in the given Location |
|3  |C:\Users\<users>\ | Folder Location  |  Check for any suspicious or unusual files in the given Location |
|4  |C:\ProgramData\ | Folder Location  |  Check for any suspicious or unusual files in the given Location |
|5  | 94.232.41.105  | IP Address  |  Suspicious IP |
|6|102.157.44.105|IP Address  |  Suspicious IP |
|7|105.158.118.241|IP Address  |  Suspicious IP |
|8|105.69.155.85|IP Address  |  Suspicious IP |
|9|113.169.187.159|IP Address  |  Suspicious IP |
|10|134.35.9.209|IP Address  |  Suspicious IP |
|11|139.195.43.166|IP Address  |  Suspicious IP |
|12|139.60.161.213|IP Address  |  Suspicious IP |
|13|148.213.109.165|IP Address  |  Suspicious IP |
|14|163.182.177.80|IP Address  |  Suspicious IP |
|15|181.141.3.126|IP Address  |  Suspicious IP |
|16|181.164.194.228|IP Address  |  Suspicious IP |
|17|185.143.223.69|IP Address  |  Suspicious IP |
|18|186.64.67.6|IP Address  |  Suspicious IP |
|19|186.86.212.138|IP Address  |  Suspicious IP |
|20|190.193.180.228|IP Address  |  Suspicious IP |
|21|196.70.77.11|IP Address  |  Suspicious IP |
|22|197.11.134.255|IP Address  |  Suspicious IP |
|23|197.158.89.85|IP Address  |  Suspicious IP |
|24|197.204.247.7|IP Address  |  Suspicious IP |
|25|197.207.181.147|IP Address  |  Suspicious IP |
|26|197.207.218.27|IP Address  |  Suspicious IP |
|27|197.94.67.207|IP Address  |  Suspicious IP |
|28|23.111.114.52|IP Address  |  Suspicious IP |
|29|41.100.55.97|IP Address  |  Suspicious IP |
|30|41.107.77.67|IP Address  |  Suspicious IP |
|31|41.109.11.80|IP Address  |  Suspicious IP |
|32|41.251.121.35|IP Address  |  Suspicious IP |
|33|41.97.65.51|IP Address  |  Suspicious IP |
|34|42.189.12.36|IP Address  |  Suspicious IP |
|35|45.227.251.167|IP Address  |  Suspicious IP |
|36|5.44.42.20|IP Address  |  Suspicious IP |
|37|61.166.221.46|IP Address  |  Suspicious IP |
|38|68.83.169.91|IP Address  |  Suspicious IP |
|39|81.184.181.215|IP Address  |  Suspicious IP |
|40|82.12.196.197|IP Address  |  Suspicious IP |
|41|98.143.70.147|IP Address  |  Suspicious IP |
|42|140.82.48.158|IP Address  |  Suspicious IP |
|43|147.135.36.162|IP Address  |  Suspicious IP |
|44|147.135.11.223|IP Address  |  Suspicious IP |
|45|152.89.247.50|IP Address  |  Suspicious IP |
|46|179.43.167.10|IP Address  |  Suspicious IP |
|47|185.7.214.218|IP Address  |  Suspicious IP |
|48|193.149.176.157|IP Address  |  Suspicious IP |
|49|193.235.146.104|IP Address  |  Suspicious IP |
|50|209.141.36.116|IP Address  |  Suspicious IP |
|51|45.61.136.47|IP Address  |  Suspicious IP |
|52|45.8.158.104|IP Address  |  Suspicious IP |
|53|5.181.234.58|IP Address  |  Suspicious IP |
|54|5.188.86.195|IP Address  |  Suspicious IP |
|55|77.73.133.84|IP Address  |  Suspicious IP |
|56|89.108.65.136|IP Address  |  Suspicious IP |
|57|94.232.41.105|IP Address  |  Suspicious IP |
|58|47.87.229.39|IP Address  |  Suspicious IP |
|59|ciborkumari[.]xyz|Domain  |  Domain IP |
|60|sombrat[.]com|Domain  |  Domain IP |
|61|gororama[.]com|Domain  |  Domain IP |
|62|softeruplive[.]com|Domain  |  Domain IP |
|63|altocloudzone[.]live |Domain  |  Domain IP |
|64|ciborkumari[.]xyz |Domain  |  Domain IP |
|65|myappearinc[.]com |Domain  |  Domain IP |
|66|parkerpublic[.]com |Domain  |  Domain IP |
|67|pastebin.mozilla[.]org/Z54Vudf9/raw |Domain  |  Domain IP |
|68|tumbleproperty[.]com |Domain  |  Domain IP |
|69|myappearinc[.]com/acquire/draft/c7lh0s5jv |Domain  |  Domain IP |
|70|250bcbfa58da3e713b4ca12edef4dc06358e8986cad15928aa30c44fe4596488 |SHA256  |  - |
|71|9db958bc5b4a21340ceeeb8c36873aa6bd02a460e688de56ccbba945384b1926 |SHA256  |  - |
|72|c24c59c8f4e7a581a5d45ee181151ec0a3f0b59af987eacf9b363577087c9746 |SHA256  |  - |
|73|5fda381a9884f7be2d57b8a290f389578a9d2f63e2ecb98bd773248a7eb99fa2 |SHA256  |  - |
|74|312f34ee8c7b2199a3e78b4a52bd87700cc8f3aa01aa641e5d899501cb720775 |SHA256  |  - |
|75|f484f919ba6e36ff33e4fb391b8859a94d89c172a465964f99d6113b55ced429 |SHA256  |  - |
|76|7cbfea0bff4b373a175327d6cc395f6c176dab1cedf9075e7130508bec4d5393 |SHA256  |  - |
|77|2598e8adb87976abe48f0eba4bbb9a7cb69439e0c133b21aee3845dfccf3fb8f |SHA256  |  - |



Knowledge Base:</br>
Initial Access: Phishing,Remote Desktop Protocol,Public-facing applications,Brokers </br>
Utilize "Chisel" tools: which is a fast TCP/UDP tunnel, transported over HTTP, secured via SSH </br>
PsExec for Lateral Movement</br>
AnyDesk, LogMeIn, Atera for persistence </br>
Cobalt Strike,Ursnif/Gozi for Data Exfiltration </br>
vssadmin.exe to delete volume Shadow Copy</br>

</br>
Note: Before blocking any IP Address, Please investigate it </br>
</br>
Reference:</br>
1.https://www.cisa.gov/sites/default/files/2023-03/aa23-061a-stopransomware-royal-ransomware_0.pdf
2.https://www.cybereason.com/blog/royal-ransomware-analysis