Home SOC Lab – Network Scanning & Service Enumeration

## Overview
This project demonstrates internal network reconnaissance using Nmap to identify exposed services and analyze port states within a Kali Linux virtual environment.



## Objective
To simulate basic reconnaissance activity and understand how different scanning techniques reveal service exposure.



## Tools Used
- Kali Linux
- Nmap
- OpenSSH
- systemctl



## Methodology

### 1.Identified Local IP Address
Used: ip a

### 2.Verified SSH Service Status
Used: sudo systemctl status ssh

### 3.Performed SYN Scan (Stealth Scan)
Used: sudo nmap -sS 192.168.64.2

### 4.Performed TCP Connect Scan
Used: nmap -sT 192.168.64.2



## Key Findings
- Identified open SSH service on port 22
- Observed differences between stealth scan and full TCP connect scan
- Understood how service state impacts port visibility



## Security Insight
Exposed SSH services increase attack surface and may become targets for brute-force attacks. Proper monitoring, firewall configuration, and authentication hardening are critical defensive measures.



## Resume Description
Built a home cybersecurity lab to simulate internal reconnaissance using Nmap. Identified exposed SSH services and analyzed differences between SYN and TCP connect scans.
