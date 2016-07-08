Author: my2ndhead 

Source type(s):  

 * wineventlog:security
 * wineventlog:application 
 * wineventlog:system
 * xmlwineventlog:security 
 * xmlwineventlog:application
 * xmlwineventlog:system
 * Perfmon:CPU
 * Perfmon:CPUTime
 * Perfmon:System
 * Perfmon:FreeDiskSpace
 * Perfmon:LogicalDisk, 
 * Perfmon:LocalNetwork
 * Perfmon:Process
 * Perfmon:Memory
 * Perfmon:Network
 * WinHostMon
 * DhcpSrvLog
 * WinRegistry
 * Script:InstalledApps
 * Script:ListeningPorts
 * Script:TimesyncConfiguration
 * Script:TimesyncStatus

Supported product(s): 

 * Windows 2008 R2 and 7
 * Windows 2012 R2 and 8.1
 * Windows 2016 and 10

App Version: 1.0
 
Supported CIM Version: >=4.4.0

Supported CIM Data Models: 

 * Application State
 * Authentication
 * Change Analysis
 * Inventory
 * Performance
 * Update

Eventgen Samples included: Yes

Add-on contains: Search and Parsing-Time configuration

===

Add-on is a partial replacement for Splunk_TA_windows. Focus is on CIM compliancy and performance.

Note 1: Test this add-on first on a separate Search Head before running in production.

Note 2: App is not compatible with Splunk App for Windows Infrastructure due to different eventtype naming

Note 3: App does not include following bin scripts, due to copyright reasons. Run Splunk_TA_windows on Forwarders instead.

 * bin/win_installed_apps.bat
 * bin/win_listening_ports.bat
 * bin/win_timesync_status.bat
 * bin/win_timesync_configuration.bat

Note 4: You can collaborate on the TA at https://github.com/my2ndhead/TA-microsoft-windows

Microsoft KB Documents used for lookups:

 * Description of security events in Windows 7 and in Windows Server 2008 R2: https://support.microsoft.com/en-us/kb/977519
 * Where can I find the full list of Failure Reasons for event 4625? o
   http://answers.microsoft.com/en-us/windows/forum/windows_vista-security/where-can-i-find-the-full-list-of-failure-reasons/d0269426-2183-4d99-8af0-cc009dee6658
 * LogLevel Enumeration: https://msdn.microsoft.com/en-us/library/microsoft.windowsazure.diagnostics.loglevel.aspx

Todo: Improve CIM Datamodel compatibility (ongoing)

License: Create Commons Attribution 4.0 International 
         https://creativecommons.org/licenses/by/4.0/
