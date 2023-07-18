## WMI || Windows Management Instrumentation

#### Overview
“Windows Management Instrumentation Event Subscription” is MITRE ATT&CK Technique T1084
WMI is the Microsoft implementation of Web-Based Enterprise Management (WBEM)
</br>

|S.No|What To Look|Event ID|Source|Additional Details|
|:-----:|:----------------|:---------|:--------------------|:--------------------|
|1|--|--|--|--|




#### KB
Sysmon can be configured to log WmiEventFilter, WmiEventConsumer, and WmiEventConsumerToFilter activity and enable the detection of WMI abuse. ( Event ID : 19,20,21) </br>
Registered a WMI event filter</br>
Registered a WMI event consumer</br>
Bound the event consumer to the event filter</br>
WmiPrvse.exe,

#### Basic Commands To Do Different activity utilizing WMI.
|#|Event|Command-1|Command-2|Additional Details|
|:-----:|:----------------|:---------|:--------------------|:--------------------|
|1|Check For Installed Antivirus on local Machine|Get-WmiObject -Namespace root\SecurityCenter2 -Class AntiVirusProduct|Get-WmiObject -Namespace root\SecurityCenter2 -computername localhost -Query \"Select \* from AntiVirusProduct\"|--|
|2|File Listing|Get-WmiObject -Query \"Select \* From Win32_Directory where Path = \'\\Users\\UserName\\Downloads\\\'"|--|--|

Reference:</br>
1. https://medium.com/threatpunter/detecting-removing-wmi-persistence-60ccbb7dff96

