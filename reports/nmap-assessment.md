# Nmap Network Assessment Report

## Project Overview

This project demonstrates a basic network security assessment using Nmap.

The assessment was performed against the authorised practice target **scanme.nmap.org** to identify open TCP ports and detect running network services.

---

## Target

- Host: scanme.nmap.org
- Purpose: Educational practice
- Tool Used: Nmap

---

## Command 1 - Basic Port Scan

```bash
nmap scanme.nmap.org
```

### Purpose

The purpose of this scan is to identify open TCP ports on the target.

### Observation

### Observation

The Nmap service detection scan identified four open TCP ports on the target host.

| Port | State | Service | Version |
|------|-------|---------|---------|
| 22 | Open | SSH | OpenSSH 6.6.1p1 |
| 80 | Open | HTTP | Apache httpd 2.4.7 |
| 9929 | Open | nping-echo | Nping Echo |
| 31337 | Open | tcpwrapped | Service Protected |

The scan confirmed that the host was reachable and responding to network requests. Service detection successfully identified the software running on the exposed ports, providing useful information for further security assessment.

## Security Analysis

The scan identified several open services that may require further review during a security assessment.

- SSH (Port 22) allows secure remote administration. It should be protected with strong authentication and restricted access.
- HTTP (Port 80) indicates that a web server is running. Web applications should be regularly tested for vulnerabilities such as those listed in the OWASP Top 10.
- The Nping Echo service (Port 9929) is used for network testing and should only be exposed if required.
- The tcpwrapped service (Port 31337) suggests that access to the service is being filtered or controlled by security mechanisms.

## Recommendations

- Close unnecessary open ports.
- Keep all services updated with the latest security patches.
- Restrict SSH access to trusted IP addresses where possible.
- Regularly perform vulnerability assessments and network scans.
- Monitor exposed services for suspicious activity.
