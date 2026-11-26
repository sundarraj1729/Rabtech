# RabTech Internship – Task 3
## Network Scanning and Enumeration

### 1. Objective
To identify open ports, running services, service versions,
UDP ports and the operating system of an authorized lab target.

### 2. Lab Environment
- Attacker: Kali Linux
- Target: Metasploitable 2
- Target IP: 192.168.56.102
- Network: VirtualBox Host-only Network
- Tool: Nmap 7.95

### 3. Scanning Activities
1. TCP port scanning
2. Service and version detection
3. UDP port scanning
4. Operating system detection

### 4. Key Findings
- 23 open TCP ports were identified.
- FTP, SSH, Telnet, SMTP and HTTP services were detected.
- Database services included MySQL and PostgreSQL.
- UDP DNS and NetBIOS name service ports were identified as open.
- OS fingerprinting indicated Linux 2.6.X.

### 5. Evidence
- task3_tcp_scan.txt
- task3_service_version.txt
- task3_udp_scan.txt
- task3_os_detection.txt
- Task3_Combined_Report.txt

### 6. Conclusion
Nmap was used to identify network services and gather
information about the authorized Metasploitable 2 lab target.
The results provide a baseline for further security assessment.
