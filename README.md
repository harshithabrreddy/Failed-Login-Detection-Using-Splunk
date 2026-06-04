# Failed Login Detection Using Splunk

## Project Overview
This project demonstrates how to detect failed Windows login attempts using Splunk Enterprise and Windows Event Logs.

The objective of this project is to simulate basic SOC analyst monitoring and log analysis activities.

---

## Tools Used
- Splunk Enterprise
- Windows Event Logs
- Windows OS

---

## Features
- Collected Windows Security logs
- Detected failed login attempts using Event ID 4625
- Performed log analysis using SPL queries
- Investigated authentication-related events

---

## SPL Queries Used

### Failed Login Detection
```spl
EventCode=4625
```

### Count Failed Logins by Username
```spl
EventCode=4625 | stats count by Account_Name
```

### Successful Login Detection
```spl
EventCode=4624
```

---

## Project Workflow

Windows Failed Login Attempt
        ↓
Windows Security Event Logs
        ↓
Splunk Enterprise
        ↓
EventCode 4625 Detection
        ↓
SOC Investigation

---

## Screenshots

### Failed Login Detection
(Add screenshot here)

### EventCode 4625 Results
(Add screenshot here)

---

## Skills Learned
- SIEM Basics
- Log Analysis
- Windows Event Logs
- Threat Detection
- SOC Monitoring
- SPL Queries

---

## Author
B R Harshitha