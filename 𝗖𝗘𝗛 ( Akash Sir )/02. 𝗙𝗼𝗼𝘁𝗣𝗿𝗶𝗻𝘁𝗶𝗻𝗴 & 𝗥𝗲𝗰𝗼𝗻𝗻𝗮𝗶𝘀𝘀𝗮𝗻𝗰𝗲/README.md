<h1 align="center">🖥️ Day 02 🖥️</h1>
<h2 align="center">🛃 FootPrinting & Reconnaissance 🛃</h2>

---
### What is FootPrinting ?
Hackers gather as much information as possible about a target system or organization.

## 🤾‍♂️ Techniques and Tools for Footprinting
Footprinting is the first step in ethical hacking, It **helps them to understand** the "attack surface," or **all possible entry points,** of a network.

### Key Techniques :

 > - **DNS Lookup :** Finding details about a domain name's IP address and its associated servers.
 > - **WHOIS Lookup :** A WHOIS search provides information about who owns a domain and their contact details.
 > - **IP Address Scanning :** Helps locate open IP addresses associated with a target network.
 > - **Social Media Analysis :** Gathering information from social media platforms to understand structure and security practices.
 > - **Website Analysis :** Looking at the target’s website to find technology in use, linked resources, and more.

### Common Tools:

 > - **Nmap :** Used to find open ports, running services, and details about the target’s network.
 > - **Maltego :** A tool used for mapping connections between people, companies, domains, and more.
 > - **Google Dorking :** Using search engines to find information by search operators like `site:`, `filetype:`, etc.
 > - **Nikto :** Network scanning Tool

## 🕵️ PreAttack Phase Overview
Footprinting and reconnaissance form part of the preattack phase. 

  > - This phase helps ethical **hackers plan and prepare** before actively trying to enter the network.
  > - In this phase, hackers **don’t interact directly** with the systems they want to test,
  > - Instead, they gather information from public and open sources, **which keeps them undetected.**

- **Purpose of PreAttack Phase :**

   > - 1. Risk Minimization 
   > - 2. Target Understanding
   > - 3. Resource Planning

#### Best Practices of Reconnaissance
Reconnaissance is a broader term that includes footprinting but also extends into active probing (later stages).

   > - **Active**
   > - **Passive**

---
## 🕵️ Why Footprinting is Important
It helps attackers (or ethical hackers) to **understand their target, find weaknesses,** and plan their next moves.

### 🧱 Types of Footprinting

- **1️⃣ Passive Footprinting**
> - 🔹 No direct interaction with target, only monitoring
> - 🔹 Hard to detect

- *Examples:*
   > - Google hacking
   > - WHOIS lookup
   > - Social media
   > - Public records

- **2️⃣ Active Footprinting**
> - 🔹 Direct interaction with target
> - 🔹 Easier to detect

- *Examples:*

   > - Ping
   > - Traceroute
   > - DNS queries
   > - Network scanning

### 🎯 Different Kinds of Information Gathered in Footprinting
These information are most common & Important.

- [ ] Domain name
- [ ] IP addresses
- [ ] User information
- [ ] Phone Number
- [ ] Email address

### 🚷 Footprinting Threats
Footprinting threats are risks that arise when attackers collect information about a target during target analysis.

  > - **Social Engineering –** Tricking people to reveal sensitive information.

  > - **System & Network Attacks –** Using gathered details to exploit systems or networks.

  > - **Information Leakage –** Exposure of sensitive data on public platforms.

  > - **Privacy Loss –** Unauthorized access, theft, or deletion of personal or confidential data.

  > - **Corporate Espionage –** Stealing business secrets to gain competitive advantage.

## 📝 Information obtained in footprinting

- [ ] **✒️ Organization Information**
   > - Includes employee details, phone numbers, office locations, organizational background, and web technologies used by the company.

- [ ] **✒️ Network Information**
   > - Includes IP addresses, open ports, WHOIS records, DNS details, which help attackers understand the network structure.

- [ ] **✒️ System Information**
   > - Includes operating system details, web server location, usernames, and passwords, which help attackers target specific systems.

### 🕵️ Tools Used in Footprinting:

- **Nslookup :** Finds DNS records.
- **Traceroute :** Tracks the route data takes.
- **Whois :** Gets domain owner information.
- **Nmap :** Scans for open ports and services.
- **Nikto :** Checks for website vulnerabilities

---
## 🔍 Google Dorks Used by Ethical Hackers (For Information Gathering)
Ethical hackers use Google search operators to find publicly available information during the footprinting phase.

- **filetype:** Used to find specific file types such as PDF, DOC, or XLS.
   > - _Example:_ filetype:pdf report – **Finds PDF reports**.

- **index of:** Displays open directories and file listings on a website.
   > - _Example:_ index of password – May **show directories containing password files.**

- **info:** Shows basic information Google has about a webpage.
   > - _Example:_ info:example.com – **Displays website details.**

- **intitle:** Searches for specific words in the webpage title.
   > - _Example:_ intitle:login – **Finds login pages.**

- **title:** Searches for an exact phrase in the page title.
   > - _Example:_ title:"admin panel" – **Finds pages with that exact title.**

- **inurl:** Searches for specific keywords in the URL.
   > - _Example:_ inurl:admin – **Finds admin-related URLs.**

- **link:** Finds webpages that link to a specific site.
   > - _Example:_ link:example.com – **Shows sites linking to example.com.**

- **related:** Displays websites similar to a given website.
   > - _Example:_ related:amazon.com – **Shows similar e-commerce sites.**

- **site:** Restricts search results to a specific domain or website.
   > - _Example:_ site:example.com – **Searches only within example.com.**

---
## 🔍 Footprinting Through Search Engines









