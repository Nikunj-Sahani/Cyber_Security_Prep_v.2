<h1 align="center">📜 Day 03 📜</h1>
<h2 align="center">🛜 Network Scanning 🛜</h2>

---
### What is Network Scanning ?
Scanning is a method in which we can **get information about a network**, port or vulnerability in a system.

## 🌐 Types of Network Scanning

- **1️⃣ Port Scanning :-** Port scanning is the process of **identifying open ports and services running on a target system** by sending packets to check how it responds.

  > - **Find open, closed, and filtered ports.**
  > - *Examples :* TCP scan , UDP scan
  > - **nmap 192.168.1.10**

- **2️⃣ Network Scanning :-** Network scanning is the process of **discovering active (live) hosts** within a network.

  > - **Find which systems are alive.**
  > - *Examples :* ICMP scan, ARP scan
  > - **nmap -sn 192.168.1.0/24**

- **3️⃣ Vulnerability Scanning :-**

  Vulnerability scanning is the process of **identifying security weaknesses in a system** to determine whether it is exploitable.

## 🎯 Objectives of Network Scanning

 > - Identify live hosts
 > - Discover open or closed ports
 > - Detect running services & versions
 > - Identify operating systems
 > - Find security weaknesses

---
### 🔌 What is Port ?
A port is a logical communication endpoint used by a computer to **identify which service or application should receive data.**

- 📌 **Think of an IP address as a house address and a port as a room number inside the house.**
Examples:

80 → HTTP (Web)

443 → HTTPS (Secure Web)


22 → SSH

21 → FTP

Port Range:

0–1023 → Well-known ports

1024–49151 → Registered ports

49152–65535 → Dynamic/Private ports

📌 Used in TCP and UDP
