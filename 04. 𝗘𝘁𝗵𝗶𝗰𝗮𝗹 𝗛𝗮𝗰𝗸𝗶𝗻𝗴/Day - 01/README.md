<h1 align="center">📜 Day 01 📜</h1>
<h2 align="center">🧑‍💻 ETHICAL HACKING INTRODUCTION 🧑‍💻</h2>

---
## 🖋️ What is Hacking ?
Hacking is a process of **gaining unauthorized access of a system** with the help of exploiting systems vulnerabilities.

### What is Ethical Hacking ?
Ethical Hacking is a process in which a **hacker hacks a system in a legal way and his aim is to identify vulnerabilities** in an application, in systems or in organisation by bypassing system security.

### Who is Hacker ?
Hacker is a person who find weakness in computer and **gain unauthorized access of a system.**

### 🎭 Types of Hackers - White & Black & Grey

   - **White Hat Hacker -** Hackers whos’ aim is to scan for vulnerabilities and gain access of the system with the permission of the owner.

   - **Black Hat Hacker -** Hackers who has aim is to gain unauthorised access of the system with the help of malicious and threat activity, they are also known as crackers.

   - **Grey Hat Hacker -** Hackers who attack depending upon the situation they do both work offensively and defensively at various times.

   > - **Script Kiddies -** An unskilled hacker who compromises a system by running scripts, tools and software which was developed by real hackers.
  
   > - **Cyber Terrorists -** These are individuals with a wide range of skills, motivation by religious or potential beliefs.
  
   > - **Suicide Hackers -** Suicide hackers aim to bring down critical infrastructure and not worried about facing jail or any kind of punishment.
  
   > - **Hacktivists –** The group of hackers that work together to archive a certain objective and they work for government or any other agencies.
  
   > - **State Sponsored Hackers -** These types of hackers are employed by any single community, group, organisations and any individual person and the purpose depends on commands of the persons who sponsored the hackers.

---
## ✏️ Classification of Attacks

- **Passive Attacks -** Passive attacks involve an attacker passively monitoring or collecting data without altering or destroying it.
   > - *Example -* Footprinting, sniffing and eavesdropping and Network traffic analysis.

- **Active attacks -** The attacker taking direct action against the target system or network, and can be more dangerous than passive attacks.
   > - *Example -* DOS & DDOS attack, Firewall and IDS attack, Spoofing & Man in middle attack.

- **Close-in Attack -** A Close-In Attack is an attack in which the attacker must be physically close to the target system, network, or user to carry out the attack.
   > - This type of attack focuses on physical access rather than remote exploitation. **Example - Social Engineering.**
   
- **Insider Attacks -** It carried out by people who are familiar with the computer network system and hold authorised access to all the information.
   > - *Example -* Employee Data theft and spoliation.

- **Distributions attacks -** It occur when attackers tamper with hardware and software prior to installation.
   > - *Example -* Modification of Software and Hardware during production and Modification of Software and Hardware during distribution.

---
### 1️⃣ Classification Based on Activity

- **🔹 Passive Attacks :-** Attacker only observes data, does not modify it.
  > - **Example -** Eavesdropping  ,,  Traffic analysis  ,,  Sniffing (Wireshark)
  > - 🛑 Hard to detect

- **🔹 Active Attacks :-** Attacker alters or disrupts data or services.
   > - **Example -** DoS / DDoS  ,,  Man-in-the-Middle  ,,  Spoofing  ,,  Malware attacks

### 2️⃣ Classification Based on Target

- **🔹 Network Attacks :-** 
   > - DoS / DDoS
   > - ARP Spoofing
   > - DNS Poisoning
   > - Packet Sniffing

- **🔹 Host-Based Attacks :-**
   > - Password cracking
   > - Privilege escalation
   > - Malware infection

- **🔹 Web Application Attacks :-**
   > - OWASP Top 10
   > - SQL Injection
   > - XSS (Cross-Site Scripting)
   > - CSRF
   > - File Inclusion (LFI/RFI)

- **🔹 Wireless Attacks :-**
   > - Evil Twin
   > - Deauthentication attack
   > - WPA/WPA2 cracking

### 3️⃣ Classification Based on Security Goals (CIA Triad)

- **🔹 Confidentiality Attacks :-**
  > - Sniffing
  > - Keylogging
  > - Data theft

- **🔹 Integrity Attacks :-**
  > - Data modification
  > - Website defacement
  > - MITM attacks

- **🔹 Availability Attacks :-**
  > - DoS / DDoS
  > - Ransomware


### 4️⃣ Classification Based on Technique 

- **🔹 Social Engineering Attacks :-**
  > - Phishing
  > - Vishing
  > - Pretexting
  > - Baiting

- **🔹 Malware-Based Attacks :-**
  > - Virus
  > - Worm
  > - Trojan
  > - Ransomware
  > - Spyware

- **🔹 Password Attacks :-**
  > - Brute force
  > - Dictionary attack
  > - Credential stuffing

### 5️⃣ Classification Based on Access Level

- **🔹 Insider Attacks :-** Performed by employees or trusted users

- **🔹 Outsider Attacks :-** Performed by external hackers

### 6️⃣ Classification Based on Automation

- **🔹 Manual Attacks :-**
  > - Human-driven testing
  > - Advanced exploitation

- **🔹 Automated Attacks :-**
  > - Botnets
  > - Automated scanners

### 7️⃣ Classification Based on Layer (OSI Model)

| OSI Layer    | Attack Examples   |
| ------------ | ----------------- |
| Physical     | Cable tapping     |
| Data Link    | ARP Spoofing      |
| Network      | IP Spoofing       |
| Transport    | SYN Flood         |
| Session      | Session Hijacking |
| Presentation | SSL Stripping     |
| Application  | SQL Injection     |

---
## 🔐 CIA Traid
The CIA Triad is a core security model used in ethical hacking, CEH, and cybersecurity to protect information systems.

- **CIA Triad is a security model designed to ensure Confidentiality, Integrity, and Availability of information.**
  
- [ ] **1. Confidentiality -** Only authorized individuals/systems can view sensitive data or classified information.
  
   > - **In simple word-** 🔒 Protects data from unauthorized access
  
   > - **Examples :-** Passwords , Encryption , Access control , Firewalls

   > - **Attacks on Confidentiality :-** Sniffing , Phishing , Shoulder surfing , Keylogging

- [ ] **2. Integrity -** This make sure that data has not been modified. Corruption of data is a failure to maintain data integrity.

   > - **In simple word-** 🛡️ Ensures data is accurate and not altered
   
   > - **Examples :-** Hashing (MD5, SHA) , Digital signatures , File permissions , Checksums

   > - **Attacks on Confidentiality :-** Man-in-the-Middle (MITM) , SQL Injection , Website defacement

- [ ] **3. Availability -** This means that the network should be readily available to its users. This applies to systems and to data.

   > - **In simple word-** ⚡ Ensures systems and data are accessible when needed
   
   > - **Examples :-** Redundant servers , Load balancing , Backups , UPS
  
   > - **Attacks on Confidentiality :-** DoS / DDoS , Ransomware , Hardware failure

 - [ ] Extra to Remember Only :- NOT part of CIA, but it supports security.

- **Authenticity –** This refers to communication document or any Data that ensures the quality of data being genuine.

- **Non-Repudiation –** Non-repudiation provides proof of origin and delivery so that neither sender nor receiver can deny their involvement.

---
## 🧠 Hacking Methodology / Phases of Hacking

- [ ] **1️⃣ Reconnaissance (Footprinting) :-** It is the first stage of hacking where we first gather information about the target of his computer system.

  - **Goal :** Collect information about the target
  > - IP address, domain, DNS
  > - Employees, emails, technologies

  - **Types:**
   > - Passive (Google, WHOIS)
   > - Active (Ping, traceroute)

- [ ] 2️⃣ **Scanning & Enumeration :-** Scanning is a method in which we can get information about a network, port or vulnerability in a system

  - **Goal :** Discover live systems, open ports, and services
   > - Port scanning
   > - OS detection
   > - User & service identification

  - **Tools :**
   > - nmap, netstat, ss
 
- [ ] 3️⃣ **Gaining Access :-** Enumeration is technique to extracting user name information networks resource and machines shares services in systems.

  - **Goal :** Exploit vulnerabilities to enter the system
   > - Password attacks
   > - Exploits
   > - Web attacks (SQLi, XSS)

  - **Tools :**
   > - Metasploit, Hydra, Burp Suite

- [ ] 4️⃣ **Maintaining Access :-** Hackers try to hold on to the initial access or foothold they have gained on the network.

  - **Goal :** Keep access for future use (testing purpose)
   > - Backdoors
   > - Rootkits
   > - Trojans

- [ ] 5️⃣ **Covering Tracks :-** Hide activity and erase evidence

   > - Clearing logs
   > - Hiding files
   > - Using steganography

> - *Related Topics*

- **Vulnerability Analysis -** The process of analysing protocol services and configuration to discover vulnerabilities and design flaws that will expose operating system.

- **System Hacking -** When an attacker finds and collects information by using different ways like footprinting, scanning, enumeration and vulnerability analysis are used in these phases and entered in target system is known as system hacking.

   > - It includes: - : Gaining Access : Escalating Privileges : Maintain access : Clearing Logs

---
## 🧱 Cyber Kill Chain
Cyber Kill Chain is a model that identifies the steps followed by attackers to carry out a cyber attack.

### 📌🧱 7 Stages of Cyber Kill Chain

- **1️⃣ Reconnaissance**
   > - Attacker collects information about the target
   > - Emails, IPs, domains, employees

- **2️⃣ Weaponization**
   > - Creates malicious payload
   > - Malware + exploit combined

- **3️⃣ Delivery**
   > - Sends malware to victim
   > - Email attachment, USB, website

- **4️⃣ Exploitation**
   > - Exploit runs on victim system
   > - Vulnerability is triggered

- **5️⃣ Installation**
   > - Malware installed on system
   > - Backdoor or trojan created

- **6️⃣ Command & Control (C2)**
   > - Attacker communicates with infected system
   > - Remote access established

- **7️⃣ Actions on Objectives**
   > - Data theft
   > - Privilege escalation
   > - System damage

### 🔁 Cyber Kill Chain vs Hacking Methodology

| Cyber Kill Chain     | Hacking Methodology   |
| -------------------- | --------------------- |
| Defender focused     | Attacker focused      |
| 7 stages             | 5 stages              |
| Used to stop attacks | Used to test security |

---
## ⚠️ Risk Management
Risk Management is a systematic approach to identify, assess, treat, and monitor risks to minimize their impact on an organization.

- **1️⃣ Risk Identification :-**
  First identify the cause, consequences, sources of Risk.

  > - Identify valuable assets (Data, servers, networks, people)

- **2️⃣ Risk Assessment :-**
 It must be analyse to know the severity and seriousness of the risk.

  > - Determine risk level (📐 Risk = Threat × Vulnerability × Impact)

- **3️⃣ Risk Treatment :-**
  After knowing the seriousness of risk, it must eliminate. And check that it won’t affect again.

  > -🔹 **Risk Mitigation**
    > - Reduce risk using controls (Firewalls, IDS, patching)

  > -🔹 **Risk Acceptance**
    > - Accept risk if low and manageable

  > -🔹 **Risk Transfer**
    > - Transfer risk to third party (Insurance, cloud provider)

  > -🔹 **Risk Avoidance**
    > - Eliminate risk by stopping activity

- **4️⃣ Risk Tracking :-**
After Treatment of Risk, ensure that it should be controlled and identifies the chance of new risk.

   > - Identify possible threats (Hackers, malware, insider threats, natural disasters)

- **5️⃣ Risk Review :-**
Evaluates the performance of the implemented risk management strategies.

   > - Monitoring & Review (Continuous risk evaluation)
   > - Update controls

### 📊 Risk Management Process Flow
 > - **Assets → Threats → Vulnerabilities → Risk → Controls → Monitoring**

- **🔐 Example :--**

  > - **Asset :** Customer database
  > - **Threat :** SQL Injection
  > - **Vulnerability :** No input validation
  > - **Risk :** Data breach
  > - **Control :** Web Application Firewall

---
## 📌 Cyber Laws ⚖️
Cyber laws deal with legal issues related to cybercrime, data protection, electronic transactions, and digital evidence.

- **👉 Primary cyber law of India**

 > - **Information Technology (IT) Act, 2000**

- > *Objectives:*
   > - Legal recognition of electronic records & digital signatures
   > - Define cyber crimes
   > - Provide punishments & penalties

### 🔐 Important Sections of IT Act

| Section | Description                         |
| ------- | ----------------------------------- |
| **43**  | Unauthorized access, data damage    |
| **43A** | Failure to protect sensitive data   |
| **65**  | Tampering with computer source code |
| **66**  | Computer-related offenses           |
| **66C** | Identity theft                      |
| **66D** | Online cheating / fraud             |
| **66E** | Violation of privacy                |
| **66F** | Cyber terrorism                     |
| **67**  | Obscene content online              |
| **72**  | Breach of confidentiality           |


### 🌍 International Cyber Laws (Basics)

- GDPR (EU) – Data protection & privacy
- Computer Fraud and Abuse Act (USA)
- Cybercrime Convention (Budapest Convention)

### HiPPA :- Health Insurance Portability and Accountability Act
HIPAA is a U.S. law that ensures the privacy, security, and confidentiality of healthcare data.

- **🎯 Main Purpose of HIPAA**

  > - Protect medical records
  > - Control access to health data
  > - Prevent data breaches
  > - Ensure patient privacy

- **Protected Health Information includes:**

  > - Patient name
  > - Medical history
  > - Lab reports
  > - Insurance details

- **🧨 HIPAA Violations (Examples)**

  > - Unauthorized access to medical records
  > - Sharing patient data without consent
  > - Lost or stolen unencrypted medical devices
  > - Weak access controls

---
---

# 📊 Easy Memory Trick

- **R W D E I C A**
> - 👉 Recon → Weapon → Delivery → Exploit → Install → C2 → Action

## **🔐 Example (Phishing Attack)**

  - [ ] **Recon :** Collect employee emails
  - [ ] **Weapon :** Create malicious PDF
  - [ ] **Delivery :** Email attachment
  - [ ] **Exploit :** User opens PDF
  - [ ] **Install :** Backdoor installed
  - [ ] **C2 :** Attacker connects remotely
  - [ ] **Action :** Steal credentials

### **🧠 CEH Exam Tips**

 - > **Phishing email** → Delivery
 - > **Malware creation** → Weaponization
 - > **Remote server communication** → C2
 - > **Data exfiltration** → Actions on Objectives



