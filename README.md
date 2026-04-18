# 🔥 Linux Firewall Lab (Attack vs Defense)

## Overview

This project demonstrates the implementation of a Linux firewall using iptables and simulates real-world attack scenarios to analyze defensive behavior.

The lab was built to practice **network security, intrusion detection, and system hardening** in a controlled environment.

---

## Technologies Used

* Linux (Ubuntu/Kali)
* iptables
* Nmap
* Hydra
* VirtualBox

---

## Lab Architecture

```
Attacker Machine (Kali Linux)
        │
        │  (Scan / Brute Force)
        ▼
Target Machine (Firewall Enabled)
```

* Isolated network using VirtualBox (Host-Only / Internal Network)
* One machine simulates the attacker
* One machine acts as the secured target

---

## Firewall Configuration

Key rules implemented:

* Default policy: DROP all incoming traffic
* Allow established and related connections
* SSH protection with brute-force mitigation
* Anti port-scan rules
* Rate limiting to prevent flooding
* Logging of suspicious activities

## Results

* Unauthorized scans are detected and logged
* Brute-force attempts are limited and blocked
* Only allowed services remain accessible
* System exposure significantly reduced

---

## Future Improvements

* Integration with Fail2Ban for automated banning
* Deploy Suricata for real-time intrusion detection
* Traffic inspection with Wireshark
* Migration to nftables

---

## Skills Demonstrated

* Network Security Fundamentals
* Firewall Configuration (iptables)
* Attack Simulation & Analysis
* Linux System Hardening
* Defensive Security Mindset

---

## Disclaimer

This project is for **educational purposes only**.
All tests were performed in a controlled lab environment.

---

## 👨‍💻 Author

Gustavo Henrique
Cybersecurity Student
