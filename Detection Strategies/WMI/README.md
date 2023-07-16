## WMI || Windows Management Instrumentation
</br>
### Knowledge Base
“Windows Management Instrumentation Event Subscription” is MITRE ATT&CK Technique T1084
WMI is the Microsoft implementation of Web-Based Enterprise Management (WBEM)
</br>

|S.No|What To Look|Event ID|Source|Additional Details|
|:-----:|:----------------|:---------|:--------------------|:--------------------|
|1|--|--|--|--|




#### Suggestions
Sysmon can be configured to log WmiEventFilter, WmiEventConsumer, and WmiEventConsumerToFilter activity and enable the detection of WMI abuse. ( Event ID : 19,20,21) </br>
Registered a WMI event filter</br>
Registered a WMI event consumer</br>
Bound the event consumer to the event filter</br>
WmiPrvse.exe,


Reference:</br>
1. https://medium.com/threatpunter/detecting-removing-wmi-persistence-60ccbb7dff96

