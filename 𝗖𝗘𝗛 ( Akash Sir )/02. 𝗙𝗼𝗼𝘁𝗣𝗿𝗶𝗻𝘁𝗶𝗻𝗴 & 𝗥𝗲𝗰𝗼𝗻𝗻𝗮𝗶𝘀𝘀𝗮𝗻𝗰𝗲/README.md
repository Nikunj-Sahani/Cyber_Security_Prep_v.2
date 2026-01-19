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

<div style="text-align: center;"><img src="https://github.com/Nikunj-Sahani/Cyber_Security_Prep_v.2/blob/main/Images/Dork1.png" alt="Sample Image"></div>
<div style="text-align: center;"><img src="https://github.com/Nikunj-Sahani/Cyber_Security_Prep_v.2/blob/main/Images/Dork2.png" alt="Sample Image"></div>
<div style="text-align: center;"><img src="https://github.com/Nikunj-Sahani/Cyber_Security_Prep_v.2/blob/main/Images/Dork3.png" alt="Sample Image"></div>
<div style="text-align: center;"><img src="https://github.com/Nikunj-Sahani/Cyber_Security_Prep_v.2/blob/main/Images/Dork4.png" alt="Sample Image"></div>

### 🔍 Another Use of inurl (Google Dorking)
The inurl search operator can be used to **identify publicly accessible web pages** based on specific keywords in the URL.

  > - Some misconfigured or publicly **exposed webcam pages may appear in search results** due to poor security settings, not hacking.

- **Examples (for awareness only):**

  > - **inurl:view/index.shtml –** May show publicly indexed camera pages

  > - **intitle:"webcamXP" inurl:8080 –** Finds pages using WebcamXP software on port 8080

- [X] There are also legitimate live camera websites that stream with permission, such as:

  > - Public webcam platforms
  > - Tourism and traffic monitoring sites

    > - http://www.insecam.org/en/bynew/
    > - http://109.233.191.130:8080/
    > - https://www.skylinewebcams.com/en/webcam/italia/lazio/roma/piazza-di-spagna.html

---
## 🔍 Footprinting Through Search Engines
Search engines are the main source of **key information about the target Organization.**
- [X] Search engines are like yahoo, google , Bing , Duck duckgo, Dogphile, Shodan, Censys.

### 🧐 1. Shodan - Search Engine :::- 
Shodan is a search engine for **Internet-connected devices used to find servers, routers, webcams, IoT devices,** and services exposed online by IP, port, service, or location.

👉 Used in footprinting and reconnaissance **to identify open ports, services, and misconfigurations.**

- **Basic search filters you can use:**

  > - **city :** find devices in a particular city
  > - **country :** find devices in a particular country
  > - **geo :** you can pass it coordinates
  > - **hostname :** find values that match the hostname
  > - **net :** search based on an IP or /x CIDR
  > - **os :** search based on an operating system
  > - **port :** find particular ports that are open
  > - **before/after :** find results within a timeframe

- The Link to GO... **[ SHODAN ](https://www.shodan.io/)**

<div style="text-align: center;"><img src="https://github.com/Nikunj-Sahani/Cyber_Security_Prep_v.2/blob/main/Images/Shodan1.png" alt="Sample Image"></div>
<div style="text-align: center;"><img src="https://github.com/Nikunj-Sahani/Cyber_Security_Prep_v.2/blob/main/Images/Shodan2.png" alt="Sample Image"></div>
<div style="text-align: center;"><img src="https://github.com/Nikunj-Sahani/Cyber_Security_Prep_v.2/blob/main/Images/Shodan3.png" alt="Sample Image"></div>

---
### 🧐 2. Censys - Search Engine :::-
Censys is an Internet scanning and search platform **used to discover and analyze Internet-exposed devices,** services, websites, and digital certificates.

👉 Commonly used in footprinting and reconnaissance to **identify open ports, services, TLS/SSL certificates,** and security misconfigurations.

   > - **Alternative of Shodan**

- The Link to GO... **[ Censys ](https://search.censys.io/)**

<div style="text-align: center;"><img src="https://github.com/Nikunj-Sahani/Cyber_Security_Prep_v.2/blob/main/Images/Censys.png" alt="Sample Image"></div>

---
#### 🧐 3. Netcraft - Domain Search Engine :::-
Netcraft is an online information-gathering tool **used to identify web technologies, hosting details**, server OS, DNS information, and security posture of a website.

👉 Used in footprinting and reconnaissance to **collect publicly available website** and **infrastructure information.**

- The Link to GO... **[ Netcraft ](https://sitereport.netcraft.com/)**
 
<div style="text-align: center;"><img src="https://github.com/Nikunj-Sahani/Cyber_Security_Prep_v.2/blob/main/Images/Netcraft1.png" alt="Sample Image"></div>
<div style="text-align: center;"><img src="https://github.com/Nikunj-Sahani/Cyber_Security_Prep_v.2/blob/main/Images/Netcraft2.png" alt="Sample Image"></div>

---
#### 🧐 4. WhoisLookup - Domain Search Engine :::-
WHOIS Lookup is an information-gathering technique **used to obtain domain registration details such as domain owner, registrar**, registration dates, name servers, and **contact information.**

👉 Used in footprinting to **identify ownership and infrastructure details** of a target domain.

- The Link to GO... **[ Whoislookup ](https://whois.domaintools.com/)**
 
<div style="text-align: center;"><img src="https://github.com/Nikunj-Sahani/Cyber_Security_Prep_v.2/blob/main/Images/Mxtool.png" alt="Sample Image"></div>
<div style="text-align: center;"><img src="https://github.com/Nikunj-Sahani/Cyber_Security_Prep_v.2/blob/main/Images/Domaintools.png" alt="Sample Image"></div>

---
#### 🧐 5. Buzzsumo - Track internet Activity (PAID)
Basically it track all the activity over the internet. **BuzzSumo is an online content analysis and research tool** used to identify popular content, trending topics, and influential authors across social media platforms.

👉 In footprinting, **it helps gather public information about an organization’s online presence**, content strategy, and key influencers.

- The Link to GO... **[ Buzzsumo ](https://buzzsumo.com/)**
 
<div style="text-align: center;"><img src="https://github.com/Nikunj-Sahani/Cyber_Security_Prep_v.2/blob/main/Images/Buzzsumo.png" alt="Sample Image"></div>

---
#### 🧐 6. Nslookup - Domain Records
DNS turn domain name into Ip address for the browser .

👉 DNS or Domain Name System footprinting reveal the DNS zone data like : **DNS server name , DNS records, IP address , domain mail server** , etc.

- The Link to GO... **[ Nslookup ](https://www.nslookup.io/)**
 
<div style="text-align: center;"><img src="https://github.com/Nikunj-Sahani/Cyber_Security_Prep_v.2/blob/main/Images/Nslookup.png" alt="Sample Image"></div>

---
## 🔍 Reverse DNS Lookup
This task is performed to check the shared server of target "Means **Target is hosted in whatever server there may be other domains are also hosted.**"

- If we able to compromise the any domain of that server we got server access and we can target the our victim .
  > - Lets see how Reverse DNS footprinting is done :
  > - Tool name is **You Get Signal**

- **Websites and tools to perform a Reverse DNS Lookup:**

  > - **MXToolbox –** Reverse DNS lookup tool , [Reverse Lookup](https://mxtoolbox.com/ReverseLookup.aspx)
  > - **ViewDNS –** Reverse IP / PTR record lookup , [DNS view](https://viewdns.info/)
  > - **DNSChecker –** Reverse DNS checker , [Domain check](https://dnschecker.org/)
  > - **IPinfo –** Shows hostname for an IP ,  [IP Lookup](https://ipinfo.io/)

---
### 🔍 Gather information Through Video search Engines
TubePilot is an **OSINT tool used to analyze YouTube data** such as channels, videos, keywords, trends, and engagement metrics.

👉 In footprinting, it helps gather public information about an organization’s or individual’s video content, reach, and online presence.

- The Link to GO... **[ Tubepilot ](https://tubepilot.ai/tools/youtube-data-viewer/)**
 
<div style="text-align: center;"><img src="https://github.com/Nikunj-Sahani/Cyber_Security_Prep_v.2/blob/main/Images/Tubepilot.png" alt="Sample Image"></div>

---
## 🔍 Linux Tools to Recon

> - Nmap
> - Whois
> - Nslookup
> - Nikto
> - DNSrecon
> - Traceroute
> - Dig

---
<div style="text-align: center;"><img src="https://github.com/Nikunj-Sahani/Cyber_Security_Prep_v.2/blob/main/Images/Nmap10.png" alt="Sample Image"></div>

---
<div style="text-align: center;"><img src="https://github.com/Nikunj-Sahani/Cyber_Security_Prep_v.2/blob/main/Images/Whois10.png" alt="Sample Image"></div>

---
<div style="text-align: center;"><img src="https://github.com/Nikunj-Sahani/Cyber_Security_Prep_v.2/blob/main/Images/Nslookup10.png" alt="Sample Image"></div>

---
<div style="text-align: center;"><img src="https://github.com/Nikunj-Sahani/Cyber_Security_Prep_v.2/blob/main/Images/Nikto10.png" alt="Sample Image"></div>

---
<div style="text-align: center;"><img src="https://github.com/Nikunj-Sahani/Cyber_Security_Prep_v.2/blob/main/Images/Dnsrecon10.png" alt="Sample Image"></div>

---
<div style="text-align: center;"><img src="https://github.com/Nikunj-Sahani/Cyber_Security_Prep_v.2/blob/main/Images/Traceroute10.png" alt="Sample Image"></div>

---
<div style="text-align: center;"><img src="https://github.com/Nikunj-Sahani/Cyber_Security_Prep_v.2/blob/main/Images/Dig10.png" alt="Sample Image"></div>

---
---
## Best Practices for Reconnaissance:

- **Avoid Direct Contact Early :** Use indirect methods like WHOIS lookups and DNS analysis to reduce detection risks.
- **Document Findings :** Keep track of all information gathered for planning and reporting.
- **Prioritize Privacy :** Use anonymization tools or virtual private networks (VPNs) if necessary to mask your activity.
- **Follow Ethical Boundaries :** Ensure you’re gathering information legally and ethically, especially when working with sensitive data.
