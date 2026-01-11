## Lab Screenshots

### Windows VM Running
![Windows VM](screenshots/windows_vm_running.png.jpg)

### Successful Logon Event (Event ID 4624)
![Event 4624](screenshots/event_4624_successful_logon.png.jpg)
# SIEM Detection Rules Lab

## Project Overview
This project demonstrates hands-on experience with SIEM threat detection using Windows Security Event Logs.  
The lab simulates successful authentication activity and documents how a SOC analyst would detect and investigate it.

## Tools Used
- Microsoft Azure (Windows VM)
- Windows Event Viewer
- Windows Security Logs
- GitHub for documentation

## Objective
To detect and document multiple successful logon events (Event ID 4624) and demonstrate basic SIEM-style detection logic.
## Sample Detection Rule

**Rule Name:** Multiple Successful Logons  
**Event ID:** 4624  
**Log Source:** Windows Security Logs  

### Detection Logic
Trigger an alert when:
- 3 or more successful logon events
- Occur within a short time window
- On the same system or account

### Why This Matters
Multiple successful logons in a short time frame may indicate:
- Credential misuse
- Automated login activity
- Potential lateral movement

### Analyst Response
- Review logon timestamps
- Identify the account used
- Verify if activity is expected or suspicious
