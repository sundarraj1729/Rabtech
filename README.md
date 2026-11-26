# RabTech Internship – Task 3
## Network Scanning and Enumeration Using Nmap

### 📌 Project Overview
This task focuses on network scanning and enumeration using Nmap in an authorized cybersecurity lab environment. The objective is to identify open ports, detect running services and versions, scan UDP ports, and perform operating system detection.

### 🎯 Objectives
- Perform TCP port scanning.
- Identify open ports and associated services.
- Detect service and software versions.
- Perform UDP port scanning.
- Identify the target operating system.
- Save and document scan results.

### 🖥️ Lab Environment

| Component | Details |
|---|---|
| Attacker Machine | Kali Linux |
| Target Machine | Metasploitable 2 |
| Target IP | `192.168.56.102` |
| Network Configuration | VirtualBox Host-only |
| Scanning Tool | Nmap 7.95 |

### 🔍 Tasks Performed

**1. TCP Port Scanning**
```bash
nmap 192.168.56.102 -oN task3_tcp_scan.txt
```
Identified open TCP ports and their associated services.

**2. Service and Version Detection**
```bash
nmap -sV 192.168.56.102 -oN task3_service_version.txt
```
Detected running services and their software versions.

**3. UDP Port Scanning**
```bash
sudo nmap -sU --top-ports 20 192.168.56.102 -oN task3_udp_scan.txt
```
Identified commonly used UDP ports and their states.

**4. Operating System Detection**
```bash
sudo nmap -O 192.168.56.102 -oN task3_os_detection.txt
```
Performed operating system fingerprinting to estimate the target OS.

### 📊 Key Findings

- 23 open TCP ports were identified.
- FTP, SSH, Telnet, SMTP, HTTP and SMB services were detected.
- MySQL and PostgreSQL database services were identified.
- DNS and NetBIOS UDP services were detected.
- OS fingerprinting indicated a Linux 2.6.X kernel family.

### 📁 Repository Structure

```text
RabTech-Internship-Task-3/
│
├── README.md
├── Task3_Report.md
├── Task3_Combined_Report.txt
│
├── task3_tcp_scan.txt
├── task3_service_version.txt
├── task3_udp_scan.txt
└── task3_os_detection.txt
```

### 📝 Conclusion

This task provided practical experience in network reconnaissance and enumeration using Nmap. The scans helped identify open ports, running services, software versions, UDP services and operating system information within an authorized lab environment.

### ⚠️ Disclaimer

All scanning activities were conducted against the approved, intentionally vulnerable Metasploitable 2 virtual machine in an isolated VirtualBox Host-only lab environment. These techniques must only be used on systems for which explicit authorization has been obtained.

---

**Internship:** RabTech Academy  
**Task:** Task 3 – Network Scanning and Enumeration  
**Tool:** Nmap
