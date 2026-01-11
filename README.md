# SIEM Detection Rules Lab

## 📌 Project Overview
This project demonstrates how Security Information and Event Management (SIEM) systems detect suspicious activity using Windows Security Event Logs. The lab focuses on identifying successful logon behavior and simulating detection logic commonly used by SOC analysts.

## 🛠 Tools & Technologies
- Azure Virtual Machine (Windows 10)
- Windows Event Viewer
- Security Event Logs
- Event ID 4624 (Successful Logon)
- GitHub for documentation

## 🧪 Lab Setup
- Deployed a Windows 10 VM in Azure
- Enabled Security Auditing
- Generated multiple successful login events
- Collected logs from Event Viewer

## 🔍 Detection Logic
**Rule Name:** Multiple Successful Logons  
**Event ID:** 4624  
**Condition:** 3 or more successful logons within a short time window  
**Purpose:** Identify abnormal authentication behavior

## 📊 Observed Events
The following logs were generated and analyzed:
- SYSTEM account logons
- Service-based authentication events
- Elevated token logons

## 🚨 Alert Simulation
An alert would be triggered when:
- Multiple successful logons occur rapidly
- Authentication behavior deviates from baseline

## 📄 Documentation
Detailed analysis and screenshots are included in the PDF below:

➡ **SIEM_Detection_Rules_Lab.pdf**

## 🎯 Skills Demonstrated
- SIEM fundamentals
- Log analysis
- Detection rule creation
- Security event investigation
- Technical documentation

## 🚀 Next Steps
- Integrate logs with Azure Sentinel
- Create KQL-based detection rules
- Add failed login correlation
- Expand to brute-force detection

---
**Author:** Marcus Ashmond  
