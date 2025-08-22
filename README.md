# Post-Attack Network Session Analysis of PCAP Files using Wireshark 

## 📁 Project Overview
This project focuses on performing **network forensic analysis** on a captured `.pcap` file using **Wireshark**. It simulates a post-attack investigation in a Windows Active Directory environment to uncover attacker behavior and extract key Indicators of Compromise (IoCs).

## 🎯 Objective
To analyze malicious network traffic after a simulated cyber attack using NeSA and Wireshark, identify the infected client, and understand attacker activity.

## 🧪 Dataset Details
- **PCAP Source**: [Malware-Traffic-Analysis.net](https://www.malware-traffic-analysis.net/)
- **Exercise Name**: `2025-06-13 - IT'S A TRAP!`
- **LAN Subnet**: `10.6.13.0/24`
- **AD Domain**: `massfriction.com`
- **Capture Duration**: ~34 minutes (21:03:55 to 21:38:23)
- **Total Packets**: 48,877
- **Total Sessions**: 212

## 🛠️ Tools Used
- **NeSA** (Network Session Analyser by CDAC)
- **Wireshark**
- **Threat Intel Portals** (VirusTotal, AbuseIPDB)

## 🔍 What Was Analyzed
- Basic traffic statistics (packets, sessions, top talkers, protocol distribution)
- Identification of infected Windows client:
  - IP address
  - MAC address
  - Hostname
  - User account
- Detection of:
  - Suspicious DNS & HTTP requests
  - Malicious domains & IPs
  - Encrypted Command-and-Control (C2) communication
  - Signs of data exfiltration
- Attack timeline reconstruction

## 📊 Key Findings
| Forensic Element | Value |
|------------------|-------|
| Infected IP      | **10.6.13.133** |
| MAC Address      | **24:77:03:ac:97:df** |
| Hostname         | **DESKTOP-5AVE44C** |
| Username         | **gaines** |
| Malicious Domains| hillcoweb.com, windows-msgas.com, event-datamicrosoft.live, varying-rentals-calgary-predict.trycloudflare.com |
| External IPs     | 67.217.228.199, 83.137.149.15, 205.174.24.80, 104.21.112.1, 104.21.80.1, 104.21.16.1 |
| Protocols Used   | TLS/443 (C2), HTTP/80 (fake Microsoft C2, exfiltration), SMB, Kerberos, DNS |

## ✅ Forensics Checklist Followed
- [x] Basic information extraction
- [x] Session and protocol analysis
- [x] HTTP and DNS traffic inspection
- [x] Malicious session identification
- [x] Timeline building
- [x] IOC extraction and reporting
- [x] Answered specific forensic questions (infected IP, MAC, hostname, user)

## 📁 Report Structure
The complete analysis is documented in the report with:
- Timeline of attack
- Session tables and findings
- Indicators of Compromise (IoCs)
- Screenshots of NeSA and Wireshark output
- Key recommendations

## 👤 Author
**Shankar Sharma**  
Cyber Forensics & Security | CDAC Project | 2025

## 📘 Disclaimer
This project is for **educational and research purposes only**. The PCAP file is sourced from public malware training data and does not represent a real organization's data.
