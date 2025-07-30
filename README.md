# Post-Attack Network Session Analysis of PCAP Files using NeSA

## 📁 Project Overview
This project focuses on performing **network forensic analysis** on a captured `.pcap` file using **CDAC’s NeSA (Network Session Analyser)**. It simulates a post-attack investigation in a Windows Active Directory environment to uncover attacker behavior, reconstruct sessions, and extract key Indicators of Compromise (IoCs).

## 🎯 Objective
To analyze malicious network traffic after a simulated cyber attack using NeSA and Wireshark, identify infected clients, and understand attacker activity based on session-level data.

## 🧪 Dataset Details
- **PCAP Source**: [Malware-Traffic-Analysis.net](https://www.malware-traffic-analysis.net/)
- **Exercise Name**: `2025-06-13 - IT'S A TRAP!`
- **LAN Subnet**: `10.6.13.0/24`
- **AD Domain**: `massfriction.com`

## 🛠️ Tools Used
- **NeSA** (Network Session Analyser by CDAC)
  
## 🔍 What Was Analyzed
- Reconstructed all sessions from the `.pcap`
- Identified the infected Windows client and corresponding:
  - IP address
  - MAC address
  - Hostname
  - User account name
- Detected:
  - Suspicious DNS & HTTP requests
  - Potential malware download
  - Command-and-Control communication
  - Signs of data exfiltration

## 📊 Key Findings
| Forensic Element | Value |
|------------------|-------|
| Infected IP      | (to be filled after analysis) |
| MAC Address      | (to be filled) |
| Hostname         | (to be filled) |
| Username         | (to be filled) |
| Malicious Domain | (to be filled) |
| External IPs     | (to be filled) |

## ✅ Forensics Checklist Followed
- [x] Session reconstruction by IP and protocol
- [x] HTTP and DNS traffic inspection
- [x] Malicious session identification
- [x] Timeline building
- [x] IOC extraction and reporting

## 📁 Report Structure
The complete analysis is documented in the report with:
- Timeline of attack
- Session tables and findings
- Screenshots of NeSA output
- Indicators of Compromise (IoCs)
- Recommendations (optional)
