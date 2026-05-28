# TryHackMe Writeups

---

# DNS in Detail
**Platform:** TryHackMe | **Difficulty:** Easy

## Summary
Deep dive into how DNS works and how it resolves domain names to IP addresses.

## What I Did
- Learned DNS record types: A, AAAA, CNAME, MX, TXT
- Understood the DNS resolution process from recursive to authoritative
- Practiced DNS lookups using nslookup and dig

## Tools Used
nslookup, dig

## Key Takeaways
DNS is a critical attack surface — misconfigured records and zone transfers can leak sensitive information.

---

# Pentesting Fundamentals
**Platform:** TryHackMe | **Difficulty:** Easy

## Summary
Covered the ethics, methodology, and legal framework behind penetration testing.

## What I Did
- Learned the penetration testing methodology
- Studied rules of engagement and scoping
- Covered the five phases: recon, scanning, exploitation, post-exploitation, reporting

## Key Takeaways
Pentesting without written authorization is illegal. Methodology and documentation matter as much as technical skills.

---

# Cyber Kill Chain
**Platform:** TryHackMe | **Difficulty:** Easy

## Summary
Covered the Cyber Kill Chain framework used to identify and prevent network intrusions.

## What I Did
- Studied all 7 phases: Reconnaissance, Weaponization, Delivery, Exploitation, Installation, C2, Actions on Objectives
- Mapped real attack scenarios to each phase
- Learned how defenders use the framework to detect and interrupt attacks

## Key Takeaways
Understanding the kill chain from both offensive and defensive perspectives helps you think like an attacker and defend like a professional.

---

# Intro to Digital Forensics
**Platform:** TryHackMe | **Difficulty:** Easy

## Summary
Introduction to digital forensics concepts and practical investigation techniques.

## What I Did
- Learned the forensics investigation process
- Practiced file metadata analysis
- Used tools to examine images and documents for hidden information
- Covered chain of custody and evidence handling

## Tools Used
ExifTool, pdfinfo

## Key Takeaways
Evidence integrity is everything in forensics — how you collect and handle evidence is as important as what you find.

---

# Operating System Security
**Platform:** TryHackMe | **Difficulty:** Easy

## Summary
Introduction to OS security concepts covering authentication, access control, and SSH hardening.

## What I Did
- Studied common OS vulnerabilities
- Practiced SSH authentication with key pairs
- Covered user permissions and access control
- Learned about common attack vectors targeting OS level

## Tools Used
SSH, Linux CLI

## Key Takeaways
Most OS compromises come from misconfiguration, not zero days. Hardening basics like disabling root SSH and enforcing key auth go a long way.

---

# Offensive Security Intro
**Platform:** TryHackMe | **Difficulty:** Easy

## Summary
First hands-on room hacking a website legally in a safe environment.

## What I Did
- Used Gobuster to find hidden directories
- Discovered admin panel through directory enumeration
- Accessed application and demonstrated unauthorized access

## Tools Used
Gobuster

## Key Takeaways
Web applications often expose sensitive endpoints that aren't linked anywhere — always enumerate directories.

---

# Network Security
**Platform:** TryHackMe | **Difficulty:** Easy

## Summary
Covered network security concepts, attack methodology, and practiced hacking into a target server.

## What I Did
- Performed passive and active reconnaissance
- Used Nmap for port scanning and service enumeration
- Identified vulnerabilities on target
- Exploited target machine

## Tools Used
Nmap, Telnet

## Key Takeaways
Recon is the most important phase — the more you know about a target before attacking the more targeted your approach.

---

# Web Application Security
**Platform:** TryHackMe | **Difficulty:** Easy

## Summary
Covered common web application vulnerabilities and how to identify and exploit them.

## What I Did
- Practiced identifying and exploiting IDOR vulnerabilities
- Tested for SQL injection
- Explored XSS attack vectors
- Used Burp Suite to intercept and manipulate requests

## Tools Used
Burp Suite, browser dev tools

## Key Takeaways
OWASP Top 10 vulnerabilities appear constantly in real environments. Understanding how they work is essential for both offense and defense.

---

# Defensive Security Intro
**Platform:** TryHackMe | **Difficulty:** Easy

## Summary
Introduction to defensive security covering SOC operations, threat intelligence, DFIR, and SIEM.

## What I Did
- Learned SOC analyst responsibilities
- Studied threat intelligence feeds and IOCs
- Covered DFIR fundamentals
- Practiced using a SIEM to investigate alerts

## Key Takeaways
Defense requires understanding the attacker's perspective. Knowing how attacks work makes you a better defender.

---

# Security Operations
**Platform:** TryHackMe | **Difficulty:** Easy

## Summary
Deep dive into Security Operations Center responsibilities, processes, and tools.

## What I Did
- Studied SOC tiers and analyst roles
- Learned alert triage and escalation processes
- Covered log analysis and SIEM usage
- Practiced investigating security incidents

## Key Takeaways
A SOC analyst's job is pattern recognition at scale — knowing what normal looks like is how you spot what isn't.

---

# Nmap
**Platform:** TryHackMe | **Difficulty:** Easy

## Summary
Covered Nmap in depth — scan types, service detection, OS fingerprinting, and output formats.

## What I Did
- Used -sV for service version detection
- Used -sC for default scripts
- Ran -A for aggressive scan combining OS detection, version, scripts
- Practiced -sS SYN scans, -sU UDP scans
- Used --top-ports and -p- for port range scanning

## Tools Used
Nmap

## Key Takeaways
Understanding scan types and when to use each one is fundamental to recon.

---

# HTTP in Detail
**Platform:** TryHackMe | **Difficulty:** Easy

## Summary
Covered how HTTP works including requests, responses, methods, and status codes.

## What I Did
- Studied HTTP methods: GET, POST, PUT, DELETE
- Learned request and response structure
- Covered cookies and how they maintain session state
- Understood HTTPS and how TLS encrypts traffic

## Key Takeaways
HTTP is the foundation of web application attacks. Understanding the protocol deeply is essential for web pentesting.

---

# Nmap Live Host Discovery
**Platform:** TryHackMe | **Difficulty:** Medium

## Summary
Focused on using Nmap to discover live hosts on a network using various scan techniques.

## What I Did
- Used ARP scans for local network discovery
- Practiced ICMP echo, timestamp, and address mask scans
- Used TCP SYN and ACK ping scans
- Combined techniques for comprehensive host discovery

## Tools Used
Nmap

## Key Takeaways
Host discovery is the first step of any engagement. Different environments require different techniques — ARP works locally, ICMP and TCP work across subnets.

---

# Metasploit: Introduction
**Platform:** TryHackMe | **Difficulty:** Easy

## Summary
Introduction to the Metasploit Framework covering its core components and basic usage.

## What I Did
- Navigated msfconsole
- Searched for and selected modules
- Set RHOSTS, LHOST, payload options
- Used auxiliary and exploit modules
- Practiced post-exploitation basics

## Tools Used
Metasploit Framework

## Key Takeaways
Metasploit streamlines exploitation but understanding what each module does matters more than just running it.

---

# Introduction to Cryptography
**Platform:** TryHackMe | **Difficulty:** Medium

## Summary
Covered core cryptography concepts including symmetric, asymmetric encryption, hashing, and PKI.

## What I Did
- Studied AES and DES symmetric encryption
- Learned RSA and Diffie-Hellman key exchange
- Covered hashing algorithms: MD5, SHA-1, SHA-256
- Understood PKI and how TLS certificates work

## Key Takeaways
Cryptography underpins almost every security control. Weak implementations are a massive attack surface.

---

# Burp Suite: Repeater
**Platform:** TryHackMe | **Difficulty:** Easy

## Summary
Hands-on practice with Burp Suite's Repeater tool for manipulating and replaying HTTP requests.

## What I Did
- Intercepted HTTP requests with Burp Proxy
- Used Repeater to modify and resend requests
- Tested for vulnerabilities by manipulating parameters
- Practiced identifying server responses to malicious input

## Tools Used
Burp Suite

## Key Takeaways
Repeater is essential for manual web testing — being able to precisely control and replay requests is how you confirm and exploit vulnerabilities.

---

# Packets & Frames
**Platform:** TryHackMe | **Difficulty:** Easy

## Summary
Covered how data is divided into packets and frames and transmitted across a network.

## What I Did
- Learned the difference between packets and frames
- Studied how data is encapsulated at each layer
- Covered TCP three-way handshake
- Practiced analyzing packets

## Tools Used
Wireshark

## Key Takeaways
Understanding how data moves across a network at a low level is essential for both attack and defense — packet analysis is a core skill for any security role.
