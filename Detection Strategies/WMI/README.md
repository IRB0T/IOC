## WMI || Windows Management Instrumentation

#### Overview
“Windows Management Instrumentation Event Subscription” is MITRE ATT&CK Technique T1084
WMI is the Microsoft implementation of Web-Based Enterprise Management (WBEM)
</br>

|S.No|What To Look|Event ID|Source|Additional Details|
|:-----:|:----------------|:---------|:--------------------|:--------------------|
|1|--|--|--|--|




#### KB
When we see Event with Event ID 5858 that indicates that someone was utilizing WMI to do queries but when Query result in error at that time it will be noted under event id 5858 </br>
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
|3|List all Running services| Get-WmiObject -Query \"SELECT \* FROM Win32_Service where State = \'Running\'\"|--|--|
|4|Processor Architecture| Get-WmiObject -Query \"Select OSArchitecture FROM win32_OperatingSystem\"|--|--|
|5|Get Make,Model of machine| Get-WmiObject -Query \"Select \* FROM Win32_ComputerSystem\"|--|--|
|6|Logged-on accounts| Get-WmiObject -Class Win32_ComputerSystem \\| Select-Object UserName| Get-WmiObject -Query "Select UserName FROM Win32_ComputerSystem"|--|

Reference:</br>
1. https://medium.com/threatpunter/detecting-removing-wmi-persistence-60ccbb7dff96

