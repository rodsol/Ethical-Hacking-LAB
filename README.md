# Ethical-Hacking-LAB
#  Nmap & Scapy Ethical Hacking Lab
> Controlled environment practice results focusing on network reconnaissance and packet manipulation.

### Overview
This repository documents ethical practice using Nmap for network enumeration and Scapy for packet crafting/analysis in isolated lab environments.

### Lab Environment
```
Network: 10.6.6.0/24 (Isolated)
Tools: Nmap 7.94, Scapy 2.5.0
```
## Nmap Practice Results
Critical Findings:
- NULL session allowed (`account_used: <blank>`)
- IPC$ share: Anonymous READ/WRITE to IPC service
- print$ share: Printer drivers accessible without auth
- workfiles share: "Confidential" data with anonymous RW access

### Critical Issues Discovered
1. Anonymous SMB Access: Shares accessible without credentials
2. No Authentication: NULL sessions permitted
3. Confidential Data Exposure: "workfiles" share with RW for everyone
4. Protocol Misconfiguration: Samba allowing guest access

### Learning Objectives Achieved
- [x] Nmap script engine usage for service enumeration
- [x] SMB protocol security assessment
- [x] Packet crafting with Scapy
- [x] Protocol field analysis and manipulation
- [x] Security misconfiguration identification

 ### Legal Disclaimer
All activities conducted in controlled, isolated lab environments only.
- No real systems were compromised
- All IPs are lab addresses (10.6.6.0/24)
- For educational purposes only

### Repository Structure
nmap-scapy-lab/
├── nmap and scapy lab /          # Nmap and scapy scan results
└── README.md            # This file
```


