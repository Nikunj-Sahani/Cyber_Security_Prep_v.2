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

- [ ] **Examples:**

  > - 80 → HTTP (Web)
  > - 443 → HTTPS (Secure Web)
  > - 22 → SSH
  > - 21 → FTP

- [ ] **Total Ports : - 65535**
- [ ] **Port Range:**

  > - 0 – 1023 → Well-known ports
  > - 1024 – 49151 → Registered ports
  > - 49152 – 65535 → Dynamic/Private ports
  > - 📌 Used in TCP and UDP

### 🔹 What is a Packet?
A packet is a small unit of data that is transmitted over a network.

- 📌 **Large data is broken into packets,** sent across the network, and **reassembled at the destination.**

- [ ] **Packet Contains :-**

   > - Source IP
   > - Destination IP
   > - Port numbers
   > - Data (payload)
   > - Control information

- [X] ➡ **A packet carries data.**
- [X] ➡ **A port tells where the packet should go (which application).**

---
## 📊  Common Network Ports & Their Uses 🌐

- **20, 21 –** FTP (File Transfer Protocol)
  > - Used to transfer files between computers over TCP.
  > - **20 -** Data Connection **:-** handles the actual data transfer in active mode
  > - **21 -** Data Control **:-** handles control commands (like login, requests)

- **22 –** SSH (Secure Shell)
  > - Used for secure remote login and communication between computers.

- **23 –** Telnet
  > - Used for remote text-based communication (not secure).

- **25 –** SMTP (Simple Mail Transfer Protocol)
  > - Used to send emails.

- **53 –** DNS (Domain Name System)
  > - Translates domain names into IP addresses.

- **67 / 68 –** DHCP (Dynamic Host Configuration Protocol)
  > - Used to automatically assign IP addresses to network devices.

- **80 –** HTTP (Hypertext Transfer Protocol)
  > - Used to access websites (not secure).

- **109 –** POP2 (Post Office Protocol v2)
  > - Used to receive emails (obsolete).

- **110 –** POP3 (Post Office Protocol v3)
  > - Used to download emails from a mail server.

- **123 –** NTP (Network Time Protocol)
  > - Used to synchronize time across network devices (uses UDP).

- **143 –** IMAP4 (Internet Message Access Protocol)
  > - Used to access and manage emails directly on the server.

- **161 –** SNMP (Simple Network Management Protocol)
  > - Used to monitor and manage network devices.

- **443 –** HTTPS (HTTP Secure)
  > - Secure web communication using SSL/TLS encryption.

- **3389 –** RDP (Remote Desktop Protocol)
  > - Used to remotely access Windows systems with a GUI.

- **8080 –** HTTP Alternate / Apache Server
  > - Used as an alternative web port for web applications.

---
## 🖥️ TCP & UDP

### 🎮 TCP - Transmission Control Protocol
TCP is connection-oriented and reliable.

- **Key Features :**

  > - Connection-oriented (3-way handshake)
  > - Reliable (acknowledgements & retransmission)
  > - Ordered data delivery
  > - Error checking & flow control
  > - Slower but accurate

- **Common TCP Services :**

  > - HTTP (80)
  > - HTTPS (443)
  > - FTP (21)
  > - SSH (22)
  > - SMTP (25)

### 🎮 UDP (User Datagram Protocol)
UDP is connectionless and fast.

- **Key Features :**

  > - Connectionless (no handshake)
  > - No guarantee of delivery
  > - No order or error correction
  > - Faster than TCP
  > - Low overhead

- **Common UDP Services :**

  > - DNS (53)
  > - DHCP (67/68)
  > - NTP (123)
  > - SNMP (161)
  > - TFTP (69)

## 📌 3 - Way Handshake
The 3-Way Handshake is the process used by **TCP to establish a reliable connection between a client and a server** before data transfer.

- **Simple :-** TCP 3-Way Handshake is a **three-step process used to establish a TCP connection** between two systems.

### 🧱 Steps of 3-Way Handshake (SYN → SYN-ACK → ACK)

- **1️⃣ SYN (Synchronize)**

  > - Client → Server
  > - **Client sends a SYN packet to request a connection.**
  > - 📦 SYN

- **2️⃣ SYN-ACK (Synchronize + Acknowledge)**

  > - Server → Client
  > - **Server responds with SYN-ACK, agreeing to the connection.**
  > - 📦 SYN + ACK

- **3️⃣ ACK (Acknowledge)**

  > - Client → Server
  > - **Client sends ACK, confirming the connection.**
  > - 📦 ACK

---
### 🚩 Common TCP Flags

- **SYN (Synchronize)**
   > - Used to start a TCP connection
   > - First step of 3-way handshake

- **ACK (Acknowledgment)**
   > - Confirms receipt of data
   > - Used in almost every TCP packet

- **FIN (Finish)**
   > - Used to gracefully close a TCP connection

- **RST (Reset)**
   > - Immediately terminates a connection
   > - Sent when an error occurs or port is closed

- **PSH (Push)**
   > - Tells receiver to deliver data immediately to application

- **URG (Urgent)**
   > - Indicates urgent data in the packet
   > - Rarely used today

### 📊 TCP Flags Summary Table

| Flag | Full Form      | Purpose               |
| ---- | -------------- | --------------------- |
| SYN  | Synchronize    | Start connection      |
| ACK  | Acknowledgment | Confirm data          |
| FIN  | Finish         | Close connection      |
| RST  | Reset          | Abort connection      |
| PSH  | Push           | Send data immediately |
| URG  | Urgent         | Priority data         |

### 🔐 Attack Mapping (Important)

- **SYN Flood → SYN flag abuse**
 > - Abuse of SYN flag to create many half-open connections and cause DoS

- **RST Injection → RST flag abuse**
 > - Abuse of RST flag to forcefully terminate an active TCP connection

---
## Types of Scan

- **-sT =** TCP scan
- **-sS =** Stealth scan
- **-sX =** Xmas scan
- **-sF =** Fin scan
- **-sN =** Null scan
- **-sA =** ARP scan

### 📊 Quick Revision Table

| Scan Type  | Command       | Purpose          |
| ---------- | ------------- | ---------------- |
| Ping       | -sn           | Live hosts       |
| SYN        | -sS           | Stealth scan     |
| TCP        | -sT           | Full connection  |
| UDP        | -sU           | UDP ports        |
| FIN        | -sF           | Firewall evasion |
| NULL       | -sN           | Stealth          |
| XMAS       | -sX           | Port state       |
| OS         | -O            | OS detection     |
| Version    | -sV           | Service info     |
| Aggressive | -A            | Full scan        |
| Vuln       | --script vuln | Vulnerabilities  |

---
# Question Reminder

- What is network scanning?
- Why is network scanning used in ethical hacking?
- What is the main purpose of a ping scan?
- Which scan is called a half-open scan?
- What does port scanning identify?
- Which protocol is mainly scanned in UDP scanning?
- What is ARP scanning used for?
- Which scan uses FIN, PSH, and URG flags?
- What information is gathered from open ports?
- What is OS fingerprinting?
- Which scan is best for detecting live hosts in a LAN?
- Why is UDP scanning slow?
- What is vulnerability scanning?
- Which scan technique helps in firewall evasion?
- What is aggressive scanning?

---



