**Outdated: I didn't find enough time to update this repo - sorry**

# Sysmon-Version-History

An Inofficial Sysmon Changelog

This changelog was composed with the help of the technet blog articles, the Internet wayback machine and Google.

## v11.10

Release date: 24.06.2020

Config schema version: 4.32

Reference: 
- https://www.youtube.com/embed/HCZlJDKUqn0?autoplay=0

New Features: 
- File Delete

Fixed Bugs:
- fixes bugs ???

Known Issues:
- None

## Missed Version 

... some missed versions

## v10.4

Release date: 06.09.2019

Config schema version: 4.22

Reference: 
- https://techcommunity.microsoft.com/t5/Sysinternals-Blog/Sysmon-10-4-Rule-Enhancements/ba-p/840631

New Features: 
- None

Fixed Bugs:
- fixes bugs ???

Known Issues:
- None

## v10.2

Release date: ?

Config schema version: 4.21

Reference: 
- None

New Features: 
- None

Fixed Bugs:
- fixes bugs ???

Known Issues:
- None

## v10.1

Release date: 14.06.2019

Config schema version: 4.21

Reference: 
- None

New Features: 
- None

Fixed Bugs:
- fixes bugs ???

Known Issues:
- None

## v10.0

Release date: 12.06.2019

Config schema version: 4.21

Reference: 
- https://blogs.technet.microsoft.com/sysinternals/2019/06/12/sysmon-v10-0-autoruns-v13-95-vmmap-v3-26/
- https://twitter.com/holisticinfosec/status/1138676889227186176

New Features: 
- DNS Query logging (Event ID 22)
- reports OriginalFileName in process create and load image events
- adds ImageName to named pipe events
- logs pico process creates and terminates

Fixed Bugs:
- fixes several bugs

Known Issues:
- None

## v10.0

Release date: 11.06.2019

Config schema version: 4.21

Reference: 
- https://twitter.com/holisticinfosec/status/1138676889227186176

New Features: 
- DNS Query logging (Event ID 22)
- reports OriginalFileName in process create and load image events
- adds ImageName to named pipe events
- logs pico process creates and terminates

Fixed Bugs:
- fixes several bugs

Known Issues:
- None

## v9.01

Release date: 18.03.2019

Config schema version: 4.2

Reference: 
- https://twitter.com/olafhartong/status/1110979769586327552
- https://twitter.com/analyze_v/status/1112809459213107200

New Features: 
- None

Fixed Bugs:
- Regression fix for exclusions due to the introduction of rule groups

Known Issues:
- None

## v9.0

Release date: 18.02.2019

Config schema version: 4.2

Reference: 
- None

New Features: 
- new "rule groups" that support AND or OR matching across rules

Fixed Bugs:
- None

Known Issues:
- None

## v8.04

Release date: 18.12.2018

Config schema version: 4.1

Reference: 
- https://twitter.com/olafhartong/status/1070581799439474689
- https://twitter.com/analyze_v/status/1072923678873022464 

New Features: 
- None

Fixed Bugs:
- fixes an error with some configurations that caused severe blind spots

Known Issues:
- None

## v8.02

Release date: 11.12.2018

Config schema version: 4.1

Reference: https://blogs.technet.microsoft.com/sysinternals/2018/12/09/autoruns-v13-93-handle-v4-21-process-explorer-v16-22-sdelete-v2-02-sigcheck-v2-71-sysmon-v8-02-and-vmmap-v3-25/

New Features: 
- None

Fixed Bugs:
- fixes several filtering bugs
- resolves a handle leak and high CPU usage for certain filters when on Windows 7 and Windows Server 2008
- fixes a bug that could cause the service process to crash

Known Issues:
- issue with some configurations that caused severe blind spots https://twitter.com/analyze_v/status/1072923678873022464

## v8.0

Release date: 06.07.2018

Config schema version: 4.1

Reference: https://twitter.com/markrussinovich/status/1015017015768113152

New Features: 
- Rule tagging

Fixed Bugs:
- command-line truncation report

Known Issues:
- None

## v7.03

Release date: 14.05.2018

Config schema version: 4.0

Reference: https://blogs.technet.microsoft.com/sysinternals/2018/05/14/sysmon-v7-03/

New Features: 
- does not hash files larger than 2GB to avoid causing performance issues with SQL Server's large alternate data streams it places on database files

Fixed Bugs: 
- fixes a service executable crash that could result from long file names
- Process tracking callbacks

Known Issues:
- performance issues with SQL Server's large alternate data streams 

## v7.02

Release date: 30.04.2018

Config schema version: 4.0

Reference: https://blogs.technet.microsoft.com/sysinternals/2018/04/30/sysmon-v7-02/

New Features: 
- None

Fixed Bugs: 
- Memory leaks
- Process tracking callbacks

Known Issues:
- performance issues with SQL Server's large alternate data streams 

## v7.01

Release date: 30.04.2018

Config schema version: 4.0

Reference: https://blogs.technet.microsoft.com/sysinternals/2018/04/30/sysmon-v7-02/

New Features: 
- None

Fixed Bugs: 
- bug in v7.01 that could cause the sysmon config change event to be corrupt
- bug that prevented registry keys from being reported with abbreviated root key names (e.g. HKLM)

Known Issues:
- performance issues with SQL Server's large alternate data streams 

## v7.0

Release date: 02.01.2018

Config schema version: 4.0

Reference: https://twitter.com/markrussinovich/status/948294964378660864

New Features: 
- File version information
- Dump old configuration schema versions

Fixed Bugs: 
- None

Known Issues:
- Some BSOD on Windows 7 x64 upgrades https://twitter.com/Tecko921/status/948588631144452097
- performance issues with SQL Server's large alternate data streams 

## v6.2

Release date: 22.11.2017

Config schema version: 3.4

Reference: https://www.darkoperator.com/blog/2017/11/24/operational-look-at-sysinternals-sysmon-620-update

New Features: 
- Enhancements in WMI Logging
- Ability to change driver name
- Ability to change service name and service executable name

Fixed Bugs:
- ?

Known Issues:
- None

## v6.1

Release date: 11.09.2017

Config schema version: 3.4

Reference: https://blogs.technet.microsoft.com/sysinternals/2017/09/12/sysinternals-update-sysmon-v6-1-process-monitor-v3-4-autoruns-v13-8-accesschk-v6-11/

New Features: 
- monitoring of WMI filters and consumers (ID 19, ID 20, ID 21)

Fixed Bugs:
- fixes a bug in image load filtering

Known Issues:
- Issue with Windows Server 2008 (affects all newer versions of Sysmon) https://social.technet.microsoft.com/Forums/en-US/28325d60-5647-48ec-977b-73608ff2a62a/sysmon-61?forum=windowsinternals

## v6.03

Release date: 17.06.2017

Config schema version: 3.3

Reference: https://blogs.technet.microsoft.com/sysinternals/2017/06/17/sysinternals-update-sysmon-v6-03/

New Features: 
- None

Fixed Bugs:
- bug that prevented imageload include filters from working in some configurations

Known Issues:
- ?

## v6.02

Release date: 22.05.2017

Config schema version: 3.3

Reference: https://web.archive.org/web/20170817004219/https://docs.microsoft.com/en-us/sysinternals/downloads/sysmon

New Features: 
- ?

Fixed Bugs:
- ?

Known Issues:
- ?

## v6.01

Release date: ?

Config schema version: 3.3

Reference: https://www.reddit.com/r/AskNetsec/comments/7u3koo/sysmon_blue_screen_of_death/

New Features: 
- ?

Fixed Bugs:
- ?

Known Issues:
- https://www.reddit.com/r/AskNetsec/comments/7u3koo/sysmon_blue_screen_of_death/
- Issue with Windows Server 2008 (affects all newer versions of Sysmon) https://social.technet.microsoft.com/Forums/en-US/28325d60-5647-48ec-977b-73608ff2a62a/sysmon-61?forum=windowsinternals
- https://social.technet.microsoft.com/Forums/en-US/36adab01-b1dd-41ff-866f-b3e3b611d842/sysmon-v60-bugcheck?forum=miscutils

## v6.0

Release date: 17.02.2017

Config schema version: 3.3

Reference: https://blogs.technet.microsoft.com/sysinternals/2017/02/17/update-sysmon-v6-autoruns-v13-7-accesschk-v6-1-process-monitor-v3-32-process-explorer-v16-2-livekd-v5-61-and-bginfo-v4-21/

New Features: 
- Named pipe events (ID 17 "Pipe Created" and ID 18 "Pipe Connected")
- Configuration changes logged as separate event
- Dump Sysmons configuration scheme (-s)
- interprets and displays registry paths in their common format

Fixed Bugs:
- ?

Known Issues:
- https://www.reddit.com/r/AskNetsec/comments/7u3koo/sysmon_blue_screen_of_death/
- Issue with Windows Server 2008 (affects all newer versions of Sysmon) https://social.technet.microsoft.com/Forums/en-US/28325d60-5647-48ec-977b-73608ff2a62a/sysmon-61?forum=windowsinternals
- https://social.technet.microsoft.com/Forums/en-US/36adab01-b1dd-41ff-866f-b3e3b611d842/sysmon-v60-bugcheck?forum=miscutils

## v5.0

Release date: 18.11.2016 (?)

Config schema version: 3.2

Reference: https://twitter.com/danielhbohannon/status/799604709137010688

New Features: 
- File creation events (ID 11)
- Registry add/delete/rename/value set events (ID 12)

Fixed Bugs:
- ?

Known Issues:
- https://twitter.com/felixw3000/status/800030486189871104
- https://twitter.com/PhantomofMobile/status/801132296409448448

## v4.12

Release date: 29.08.2016

Config schema version: 3.1

Reference: https://blogs.technet.microsoft.com/sysinternals/2016/08/29/update-sysmon-v4-12-autologon-v3-1-sigcheck-v2-54-process-monitor-v3-31/

New Features: 
- reports the status of CRL checking
- fixes a bug where certain configuration files could cause the driver to blue screen

Fixed Bugs:
- ?

Known Issues:
- ?

## v4.0

Release date: 28.04.2016

Config schema version: 3.0

Reference: https://web.archive.org/web/20160315070513/https://technet.microsoft.com/en-us/sysinternals/dn798348

New Features: 
- more powerful filtering capabilities, allowing for both include and exclude rules to be specified for specific events types
- complex matching on different event fields

Fixed Bugs:
- None

Known Issues:
- ?

## v3.21

Release date: 04.02.2015

Config schema version: 2.0

Reference: https://web.archive.org/web/20160315070513/https://technet.microsoft.com/en-us/sysinternals/dn798348

New Features: 
- None

Fixed Bugs:
- fixes a paged pool leak of token objects when image logging is enabled

Known Issues:
- ?

Support:
- Last version with support of Windows 2008 or Windows Server 2003

## v3.2

Release date: 04.01.2016

Config schema version: 2.0

Reference: https://blogs.technet.microsoft.com/sysinternals/2016/01/05/update-sigcheck-v2-4-sysmon-v3-2-process-explorer-v16-1-autoruns-v13-51-accesschk-v6-01/

New Features: 
- option of logging raw disk and volume accesses

Fixed Bugs:
- ?

Known Issues:
- ?

Support:
- Last version to officially support Windows 2008 R2 or Windows Server 2003

## v3.11

Release date: 26.10.2015

Config schema version: 2.0

Reference: https://blogs.technet.microsoft.com/sysinternals/2015/10/26/update-autoruns-v13-5-sigcheck-v2-3-rammap-v1-4-bginfo-v4-21-sysmon-v3-11-adinsight-v1-2/

New Features: 
- None

Fixed Bugs:
- fixes a memory leak for DLL image load event monitoring
- removes a misleading warning when processing configuration files

Known Issues:
- ?

## v3.1

Release date: 20.06.2015

Config schema version: 2.0

Reference: https://blogs.technet.microsoft.com/sysinternals/2015/07/22/update-sysmon-v3-1-logonsessions-v1-3-vmmap-v3-21/

New Features: 
- adds information about the thread initialization function for CreateRemoteThread events, including the DLL and function name and address
- changes the format of timestamps to allow for simple string sorting

Fixed Bugs:
- fixes several bugs

Known Issues:
- ?

## v3.0

Release date: 20.04.2015

Config schema version: 2.0

Reference: https://blogs.technet.microsoft.com/sysinternals/2015/04/20/update-sysmon-v3-0-autornus-v13-3-regjump-v1-1-process-monitor-v3-11/

New Features: 
- adds the process name to process terminate events
- reports remote thread creation events (ID 8)
- improves the simplicity and flexibility of filter settings

Fixed Bugs:
- None

Known Issues:
- ?

## v2.0

Release date: 19.01.2015

Reference: https://blogs.technet.microsoft.com/sysinternals/2015/01/19/updates-sysmon-v2-0-accesschk-v5-21-ru-v1-1/

New Features: 
- includes driver load and image load events with signature information
- adds imphash calculation https://www.fireeye.com/blog/threat-research/2014/01/tracking-malware-import-hashing.html
- configurable hashing algorithm reporting
- flexible filters for including and excluding events
- support for supplying configuration via a configuration file (XML) instead of the command line

Fixed Bugs:
- None

Known Issues:
- ?

## v1.01

Release date: 18.08.2014

Reference: https://blogs.technet.microsoft.com/sysinternals/2014/08/19/updates-autoruns-v12-02-coreinfo-v3-31-sysmon-v1-01-whois-v1-12/

New Features: 
- includes unique UDP connections within 15-minute intervals

Fixed Bugs:
- fixes the manifest registration so that Sysmon event logs can be interpreted without installing Sysmon

Known Issues:
- ?

## v1

Release date: 08.08.2014

Reference: https://blogs.technet.microsoft.com/sysinternals/2014/08/08/new-sysmon-v1-0-updates-autoruns-v12-01-coreinfo-v3-3-procexp-v16-03/

