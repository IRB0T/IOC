## WMI || Windows Management Instrumentation

#### Overview
“Windows Management Instrumentation Event Subscription” is MITRE ATT&CK Technique T1084
WMI is the Microsoft implementation of Web-Based Enterprise Management (WBEM)
</br>

|S.No|What To Look|Event ID|Source|Additional Details|
|:-----:|:----------------|:---------|:--------------------|:--------------------|
|1|(source machine)In security event logs check for event id 4648 "A logon was attempted using explicit creationdentials, check for Process name (wbem\WMIC.exe)|4648|security.evtx|--|
|2|(source machine)if sysmon is utilized by organization then check for event id 1. "process creation" and look for keywords like "wmic, wmic.exe" |1|sysmon/Operational|--|
|2|(Destination machine) check for "wmiprvse.exe" in process creation. |4688|security.evtx|--|
|3|In WMI-activity Operational logs check for event id 5861 for permanent event consumer creation event.|5861|Microsoft-Windows-WMI-Activity/Operational.evtx|--|
|4|If trace logs are enable then check for event id 11 that will help you to identify username, command and remote box from where someone made connection to this system.|11|Tracelogs|--|




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
|7|Installed Patches| Get-WmiObject -query \'select \* from win32_quickfixengineering\'|--|--|

Reference:</br>
1. https://medium.com/threatpunter/detecting-removing-wmi-persistence-60ccbb7dff96

