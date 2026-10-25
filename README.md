# Windows Event Log Forensics

## Project Overview
This project documents my exploration of Windows Event Logs and their role in digital forensics, threat detection, and incident response. Completed as part of Hack The Box coursework, it covers Windows Event Viewer, Event ID 4624, Event Tracing for Windows (ETW), and PowerShell-based log discovery.

## Tools and Technologies
- Windows Event Viewer
- Windows PowerShell
- Get-WinEvent cmdlet
- Event Tracing for Windows (ETW)
- Hack The Box learning modules

## Topics Covered
### Windows Event Logs
Explored standard Windows log categories, including Application, Security, Setup, System, and Forwarded Events. Studied Event ID 4624, which records successful logons.

### Event Tracing for Windows
Learned how ETW providers offer additional visibility into system and application activity, including process, file, network, and .NET runtime events.

### PowerShell Log Discovery
Used Get-WinEvent to enumerate available Windows event logs and inspect properties such as log names, record counts, and enabled status.

```powershell
Get-WinEvent -ListLog * | Select-Object LogName, RecordCount, IsClassicLog, IsEnabled, LogMode, LogType | Format-Table -AutoSize
```

## Skills Demonstrated
- Navigating and interpreting Windows Event Logs
- Understanding authentication event records
- Exploring ETW for threat-detection visibility
- Enumerating logs with PowerShell
- Documenting technical findings and learning outcomes

## Project Documentation
[View the Windows Event Log Forensics Portfolio (PDF)](Windows_Event_Logs_Forensics_Portfolio_Polished.pdf)

## Project Scope
This is an educational project based on Hack The Box coursework. It demonstrates foundational Windows logging and forensic analysis concepts rather than a live incident investigation.  
