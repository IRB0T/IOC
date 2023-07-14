PsExec Execution
</br>
Execute a command-line process on a remote machine.
</br>

|S.No|What To Look|Event ID|Source|Additional Details|
|:-----:|:----------------|:---------|:--------------------|:--------------------|
|1  | Check for Event Id 7045 in system Event log and check for the Service Name "PSEXESVC"  |  7045 | system.evtx  | -- |
|2  | Parse UsnJrnl ($J) file and Check for Keyword "PsExec". You will find entry with extension ".KEY" and in same entry you will able to see "HOSTNAME" of the target system from where it was initiated. (Co-relate timestamp of UsnJrnl entry and System event id 7045.)   |  - | UsnJrnl  | -- |
|3  | Parse prefetch files and Check for Keyword "PsExec". You will able to see "HOSTNAME" of the target system from where it was initiated   |  - | prefetch | -- |

</br>
Knowledge Base:</br>
PsExec is a portable tool from Microsoft that lets you run processes remotely using any user's credentials.</br>
Every time you run PsExec against target system a new service will be installed by default that service name is PSEXESVC. </br>
Whenever you run PsExec against target system you will have traces of services and creation of "psexesvc.exe" </br>
Check UsnJrnl & prefetch files </br>




Reference:</br>

