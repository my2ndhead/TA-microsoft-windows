Author: my2ndhead 
Source type(s):  wineventlog:security, wineventlog:application, wineventlog:system
                 xmlwineventlog:security, xmlwineventlog:application, xmlwineventlog:system
                 Perfmon:CPU, Perfmon:CPUTime, Perfmon:System, Perfmon:FreeDiskSpace, Perfmon:LogicalDisk, Perfmon:LocalNetwork, Perfmon:Process, Perfmon:Memory, Perfmon:Network
                 WinHostMon
                 DhcpSrvLog
                 WinRegistry
                 Script:InstalledApps,Script:ListeningPorts,Script:TimesyncConfiguration,Script:TimesyncStatus

Supported product(s): 
* Windows event logs
* Windows XML event logs
* Windows Perfmon
* Windows WinHostMon
* Windows WinRegistry
* Windows DhcpSrvLog
* Windows Script:InstalledApps
* Windows Script:ListeningPorts
* Windows Script:TimeSyncConfiguration
* Windwos Script:TimeSyncStatus

Supported CIM Version: >=4.4.0
Supported CIM Data Models: Authentication, Change Analysis, Inventory, Performance

Eventgen Samples included: Yes

Add-on contains: Search and Parsing-Time configuration


Microsoft KB Documents used for lookups
 * Description of security events in Windows 7 and in Windows Server 2008 R2: https://support.microsoft.com/en-us/kb/977519
 * Where can I find the full list of Failure Reasons for event 4625? http://answers.microsoft.com/en-us/windows/forum/windows_vista-security/where-can-i-find-the-full-list-of-failure-reasons/d0269426-2183-4d99-8af0-cc009dee6658
 * LogLevel Enumeration: https://msdn.microsoft.com/en-us/library/microsoft.windowsazure.diagnostics.loglevel.aspx


Note 1: App is not compatible with Splunk App for Windows Infrastructure due to different eventtype naming

Note 2: App does not include following bin scripts, due to copyright reasons. Run Splunk_TA_windows on Forwarders instead.
  * bin/win_installed_apps.bat
  * bin/win_listening_ports.bat
  * bin/win_timesync_status.bat
  * bin/win_timesync_configuration.bat

Todo: Improve CIM Datamodel compatibility
