# Vulnerability Assessment and Penetration Testing (VAPT)

## Project Overview

This project demonstrates a Vulnerability Assessment and Penetration Testing (VAPT) exercise performed against a Metasploitable 2 virtual machine using Kali Linux.

The objective was to identify security weaknesses, assess associated risks, and recommend remediation measures using industry-standard open-source security tools.

---

## Lab Environment

### Attacker Machine
- Kali Linux
- Oracle VirtualBox

### Target Machine
- Metasploitable 2

### Network Configuration
- Host-Only Adapter

---

## Tools Used

| Tool | Purpose |
|--------|---------|
| Nmap | Network Scanning & Service Enumeration |
| Nikto | Web Vulnerability Assessment |
| OpenVAS | Vulnerability Scanner (Setup Attempt) |
| VirtualBox | Virtualization Platform |

---

## Methodology

### Phase 1 – Planning
- Define target scope
- Configure lab environment
- Select security tools

### Phase 2 – Discovery
- Host discovery
- Port scanning
- Service enumeration

### Phase 3 – Vulnerability Analysis
- Identify exposed services
- Assess attack surface
- Evaluate risks

### Phase 4 – Reporting
- Document findings
- Assign risk ratings
- Recommend mitigations

---

## Key Findings

### Anonymous FTP Access
- Port: 21
- Severity: Medium
- Anonymous login enabled

### Outdated Apache Server
- Port: 80
- Severity: High
- Running outdated version

### Samba Service Exposure
- Ports: 139/445
- Severity: High
- Network file-sharing exposed

### Multiple Open Services
- Severity: Medium
- Increased attack surface

---

## Risk Assessment

| Vulnerability | CVSS Score | Severity |
|--------------|------------|-----------|
| Anonymous FTP | 5.3 | Medium |
| Outdated Apache | 8.1 | High |
| Samba Exposure | 7.5 | High |
| Multiple Open Services | 6.5 | Medium |

---

## Screenshots

### Kali Linux VM
![Kali Linux](screenshots/01-kali-linux-vm.png)

### Metasploitable Login
![Metasploitable Login](screenshots/02-metasploitable-login.png)

### Target IP Address
![Target IP](screenshots/03-target-ip-address.png)

### Nmap Scan Results
![Nmap](screenshots/04-nmap-basic-scan.png)

### Service Detection
![Service Detection](screenshots/05-nmap-service-detection.png)

### Nikto Scan Results
![Nikto](screenshots/06-nikto-scan-results.png)

---

## Remediation Recommendations

### FTP
- Disable anonymous login
- Restrict access

### Apache
- Upgrade to latest version
- Apply security patches

### Samba
- Restrict network access
- Disable unnecessary shares

### Open Ports
- Close unused ports
- Implement firewall rules

### Authentication
- Use strong passwords
- Enable MFA

---

## Challenges Faced

### OpenVAS Installation Issues
- PostgreSQL conflicts
- Feed synchronization failures
- GVMD startup issues
- Notus Scanner errors

---

## Learning Outcomes

- Vulnerability Assessment
- Risk Analysis
- Service Enumeration
- Security Reporting
- Remediation Planning
