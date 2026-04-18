# FUTURE_CS_01
Task 1 - Vulnerability Assessment Report for a Live Website
## Task 1 – Nmap Reconnaissance

**Objective:** Perform network reconnaissance and identify exposed services.

**Tool Used:** Nmap

**Command Executed:** nmap -sS -sV -Pn -T4 testphp.vulnweb.com


**Target:** testphp.vulnweb.com

**Key Findings:**
- Host is reachable and active
- All 1000 scanned TCP ports are filtered (no response)
- Reverse DNS indicates hosting on AWS infrastructure

**Analysis:**
- The target is protected by firewall/security group filtering
- Direct service enumeration is restricted
- Network-level attack surface is minimized

**Conclusion:**
- No publicly exposed services detected
- Indicates strong perimeter security configuration

**Evidence:**
- Scan Output → `scan-results/nmap-scan.txt`
- Screenshot → `screenshots/nmap-final-scan.png`