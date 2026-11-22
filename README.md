# Networkwalks Cybersecurity Internship

This repository documents my hands-on learning, practical activities, technical progress, and evidence collected during my Cybersecurity Internship at Networkwalks.

## 1. Laptop Specifications

- **OS:** Windows 11 Home
- **RAM:** 8 GB
- **Processor:** Intel Core i3-N305 (1.80 GHz)
- **Storage:** 238 GB
- **Virtualization:** Oracle VirtualBox 7.2.8
- **Kali Linux:** Kali Linux 2026.3 VirtualBox amd64

## 2. Internship Overview

This repository contains weekly task documentation, practical exercises, screenshots, reports, and technical observations completed during the internship.

The activities cover Linux setup, networking, footprinting, network scanning, and password security.

## 3. Tools and Technologies

### Operating Systems and Virtualization
- Kali Linux
- Windows 11
- Oracle VirtualBox

### Networking and Reconnaissance
- Nmap
- Wireshark
- Tcpdump
- WHOIS
- WhatWeb
- NSLookup
- cURL
- Wafw00f
- DNSRecon

### Password Security
- John the Ripper
- Johnny
- Strawberry Perl
- pdf2john.pl
- Networkwalks Hash Calculator
- Networkwalks Password Cracker

*Tools are listed based on the activities documented in this repository.*

## 4. Weekly Progress

### Week 01 – Kali Linux Setup and Networking

- Kali Linux environment setup
- System information inspection
- IP configuration
- Network route inspection
- Connectivity testing
- DNS resolution testing
- VirtualBox network configuration

### Week 02 – Footprinting and Network Scanning

**PM1 – Footprinting**
- WHOIS lookup
- Website technology identification
- DNS information gathering
- HTTP response inspection
- Web application firewall detection
- DNS reconnaissance

**PM5 – Network Scanning**
- IP configuration analysis
- Connectivity testing
- Network scanning
- ARP inspection
- Network adapter information collection
- Network topology documentation

### Week 03 – Password Cracking

**PM1 – Password Cracking with John the Ripper**
- Configured John the Ripper and Johnny.
- Installed and verified Strawberry Perl.
- Used `pdf2john.pl` to extract the PDF password hash.
- Loaded the extracted hash into Johnny.
- Performed password recovery.
- Verified the recovered password by opening the protected PDF.

**PM2 – Password Cracking with Networkwalks Tools**
- Used the Networkwalks Hash Calculator.
- Extracted the PDF password hash using the PDF option.
- Used the Networkwalks Password Cracker.
- Performed password recovery.
- Verified the result by unlocking the provided PDF.

## 5. Repository Structure

```text
networkwalks-cybersecurity-lab/
│
├── Week-01/
│   ├── Evidence/
│   │   └── Kali-Linux-Lab/
│   └── README.md
│
├── Week-02/
│   ├── Evidence/
│   │   ├── PM1-Footprinting/
│   │   └── PM5-Network-Scanning/
│   ├── Reports/
│   └── README.md
│
├── Week-03/
│   ├── PM1-JTR/
│   │   ├── README.md
│   │   ├── W3-PM1-PDF1-UNLOCKED.png
│   │   └── W3-PM1-hash.txt
│   │
│   ├── PM2-Networkwalks-Tools/
│   │   ├── README.md
│   │   └── W3-PM2-PDF1-UNLOCKED.png
│   │
│   └── README.md
│
└── README.md
```

## 6. Learning Outcomes

- Gained practical exposure to Linux and networking.
- Practised basic reconnaissance techniques.
- Explored network scanning and information gathering.
- Learned PDF password hash extraction.
- Gained hands-on experience with John the Ripper and Johnny.
- Practised password recovery using Networkwalks tools.
- Improved technical documentation and reporting skills.

## 7. Evidence and Documentation

Screenshots, practical reports, hash files, and supporting documentation are organised by week and task.

Each weekly folder contains relevant documentation and evidence of the activities performed.

## 8. Disclaimer

All practical activities are performed for educational purposes in authorised lab environments and within the scope of the internship.
