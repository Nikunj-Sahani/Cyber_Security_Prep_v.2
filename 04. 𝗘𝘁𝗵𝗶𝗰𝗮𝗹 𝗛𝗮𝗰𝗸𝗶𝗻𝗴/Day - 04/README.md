<h1 align="center">📜 Day 04 📜</h1>
<h2 align="center">🪬 Nmap Practical Scanning & Tools 🪬</h2>

---
### 🎯 What is Nmap ?
Nmap (Network Mapper) → Scanning tool

- **Nmap is an open-source network scanning tool used to:**

   > - Discover live hosts
   > - Scan open ports
   > - Identify services & versions
   > - Detect operating systems
   > - Find vulnerabilities

- [X] **👉 Commonly used in ethical hacking, penetration testing, and CEH.**

## 🔍 Types of Scans – Commands & Details (Nmap)

**🔹 1️⃣ Host Discovery Scans**
- Ping Scan
  > - **`nmap -sn 192.168.1.0/24`**

   > - Finds live hosts
   > - No port scanning

- ARP Scan (LAN only)
  > - **`nmap -sn -PR 192.168.1.0/24`**

   > - Very accurate in local networks
   > - Works even if ICMP is blocked

**🔹 2️⃣ TCP Port Scans**

- TCP Connect Scan
  > - **`nmap -sT 192.168.1.10`**

   > - Completes full 3-way handshake
   > - Easy to detect
   > - Used without root

- SYN Scan (Stealth Scan)
  > - **`nmap -sS 192.168.1.10`**

   > - Half-open scan
   > - Fast & stealthy
   > - Most common in CEH

- FIN Scan
  > - **`nmap -sF 192.168.1.10`**

   > - Sends FIN flag
   > - Bypasses some firewalls

- NULL Scan
  > - **`nmap -sN 192.168.1.10`**

   > - No TCP flags set
   > - Firewall evasion technique

- XMAS Scan
  > - **`nmap -sX 192.168.1.10`**

   > - FIN + PSH + URG flags
   > - Used to detect closed ports

🔹 **3️⃣ UDP Scan**

- UDP Scan
  > - **`nmap -sU 192.168.1.10`**

   > - Scans UDP services (DNS, SNMP)
   > - Slow but important

🔹 **4️⃣ Service & Version Scanning**

- Service Version Detection
  > - **`nmap -sV 192.168.1.10`**

   > - Finds application name & version

- OS Detection
  > - **`nmap -O 192.168.1.10`**

   > - Detects operating system

- Aggressive Scan
  > - **`nmap -A 192.168.1.10`**
  > - **Includes:**

   > - OS detection
   > - Version scan
   > - Script scan
   > - Traceroute

**🔹 5️⃣ Vulnerability Scanning**

- Nmap Vulnerability Scripts
  > - **`nmap --script vuln 192.168.1.10`**

   > - Checks known vulnerabilities

**🔹 6️⃣ Firewall / IDS Evasion Scans**

- Fragmented Packets
  > - **`nmap -f 192.168.1.10`**

- Decoy Scan
  > - **`nmap -D RND:10 192.168.1.10`**

   > - Hides real attacker IP

- Idle (Zombie) Scan
  > - **`nmap -sI zombie_ip target_ip`**

   > - Extremely stealthy

**🔹 7️⃣ Port Range & Speed Control**

- Specific Ports
  > - **`nmap -p 21,22,80,443 192.168.1.10`**

- All Ports
  > - **`nmap -p- 192.168.1.10`**

- Fast Scan
  > - **`nmap -F 192.168.1.10`**

## 📊 Quick Revision Table
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
# 🪬Practical Scanning with Nmap
I'm starting the kali linux for scanning and i show you **screenshots below.**

- **Kali Linux** ::- (Attacker Machine) for Testing
- **Metasploitable** ::-- ( Vulnerable - Scanning perform on it)

### Important & Common Scans for you

