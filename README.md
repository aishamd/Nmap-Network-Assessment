# Nmap Network Assessment

## Overview

This project demonstrates a basic network security assessment using Nmap. The objective was to identify open TCP ports, detect running services, and document the findings in a professional security report.

## Tools Used

- Kali Linux
- Nmap
- Git
- GitHub

## Commands Used

### Basic Port Scan

```bash
nmap scanme.nmap.org
```

### Service Detection Scan

```bash
nmap -sV scanme.nmap.org -oN reports/service-scan.txt
```

## Project Structure

```
Nmap-Network-Assessment/
├── README.md
├── reports/
│   ├── nmap-assessment.md
│   └── service-scan.txt
└── screenshots/
```

## Skills Demonstrated

- Network Scanning
- Service Enumeration
- Security Documentation
- Linux Command Line
- Git & GitHub

## Disclaimer

This scan was performed against the authorized practice target **scanme.nmap.org** provided by the Nmap Project for educational purposes only.
