Zerologon || CVE-2020-1472
</br>
A critical vulnerability that allows an attacker without credentials to elevate to the highest possible privileges in the domain.
</br>

|S.No|What To Look|Event ID|Source|Additional Details|
|:-----:|:----------------|:---------|:--------------------|:--------------------|
|1  | In Security Event Logs Check for event id 4624 and look specifically for "Account Name". If you can find Account Name as the DC computer account or anonymous logon then it's our first indication AND "Source Network Address Field" will have a different IP address then DC IP. This will help us to find the source from which Zerologon exploit exploitation is attempted AND we should see captured Authentication Package as "NTLM"  |  4624 | Security.evtx  | -- |
|2  | Check for all the recent Password Reset Events. Check for events with event id "4742". When you check for these events also remember that AD will reset password for computer account every 30days. Try to co-relate 4624 & 4742 timings. In 4742 you will see "Account Name" as the DC computer account or anonymous logon AND check for "Password Last Set" field AND "Authentication Package" will be NTLM |  4742 | Security.evtx  | -- |


</br>
Knowledge Base:</br>
We will see how to detect "Zerologon" exploitation utilizing Windows event logs & Password history.
</br>



Reference:</br>
1.https://www.kroll.com/en/insights/publications/cyber/cve-2020-1472-zerologon-exploit-detection-cheat-sheet
