# VAPT Project – Simulated Lab (DVWA, Windows & Linux Targets)

This repository contains a complete Vulnerability Assessment & Penetration Testing (VAPT) project performed in a **virtualized lab environment** using Kali Linux, DVWA, Windows Server, and Ubuntu machines.

> Covers Reconnaissance to Reporting  
> Includes exploitation examples like Stored XSS  
> Tools Used: Nmap, Nessus, Metasploit, Burp Suite, Nikto, OWASP ZAP

---

# Lab Setup

- **Attacker Machine**: Kali Linux
- **Target Machines**: Windows Server 2016 & Ubuntu (with DVWA installed)
- **Virtualization Platform**: VirtualBox
- **Networking**: NAT + Host-Only Adapter

---

# Project Phases & Methodology

## Reconnaissance
- Passive & active info gathering
- Tools: `whois`, `netdiscover`, `nslookup`, `Shodan`

## Scanning & Enumeration
- Network scanning using `Nmap`
- Vulnerability scanning with `Nessus` & `Nikto`
- Enumerated services: FTP, SSH, SMB, HTTP

## Exploitation
- Exploited known CVEs via `Metasploit`
- Manual SQL Injection in web app
- Captured flag files as proof

## Post-Exploitation
- Gained shell access & privilege escalation
- Extracted sensitive files (lab)
- Created persistence (for learning only)

## Reporting
- Professional VAPT report created
- Included CVSS severity, screenshots, and mitigation steps

---

# Step 6 Highlight – Stored XSS in DVWA

One key vulnerability demonstrated:

- **Vulnerability**: Stored Cross-Site Scripting (XSS)
- **Tested On**: `http://localhost/DVWA/vulnerabilities/xss_s/`
- **Payload Used**:
  ```html
  <script>alert('Hacked by Sameer')</script>
