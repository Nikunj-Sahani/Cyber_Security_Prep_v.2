<h1 align="center">📜 Day 02 📜</h1>
<h2 align="center">🛤️ FootPrinting & Reconnaissance 🛤️</h2>

---
### What is Footprinting?
Footprinting is the first phase of hacking, where an attacker or ethical hacker collects information about a target system or organization.
- To get this information, a hacker might use various methods with variant tools.

## 🎯 Objectives of Footprinting

- Identify IP addresses
- Discover domains & subdomains
- Find network topology
- Collect employee & technology details

## 🧱 Types of Footprinting

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

---
## 🚷 Footprinting Threats
Footprinting threats are risks that arise when attackers collect information about a target during target analysis.

- **1️⃣ Social Engineering :-**

  > - An attacker sends a malicious link or email to the target. If the **user is clicked** & unaware of hacker tactics, the **system can be compromised and information stolen.**

- **2️⃣ System and Network Attacks :-**

  > - The attacker collects details like **network configuration and operating system.** After finding vulnerabilities, the attacker exploits them and may **gain full control of the network.**

- **3️⃣ Information Leakage :-**

  > - Sensitive information available on search engines or **public platforms helps attackers plan** and launch attacks.

- **4️⃣ Privacy Loss :-**

  > - After gaining access through footprinting and privilege escalation, the **attacker can steal or delete sensitive files, causing loss of privacy.**

- **5️⃣ Corporate Espionage :-**

  > - Attackers **steal confidential business data** such as new ideas, strategies, or pricing to harm competitors and **affect market position and share value.**

---
### 🎯 Different Kinds of Information Gathered in Footprinting
These information are most common & Important.

- [ ] Domain name
- [ ] IP addresses
- [ ] User information
- [ ] Phone Number
- [ ] Email address

## 📝 Information obtained in footprinting

- [ ] **✒️ Organization Information**
   > - Includes employee details, phone numbers, office locations, organizational background, and web technologies used by the company.

- [ ] **✒️ Network Information**
   > - Includes IP addresses, open ports, WHOIS records, DNS details, which help attackers understand the network structure.

- [ ] **✒️ System Information**
   > - Includes operating system details, web server location, usernames, and passwords, which help attackers target specific systems.

---
## ✍️ Footprinting Methodology
Footprinting Methodology is the **step-by-step approach used to gather** organizational, network, and system information about a target.

### 🧱 Steps in Footprinting Methodology

- [X] **🖌️ Collect Organization Information**
   > - Company name & background
   > - Employee details
   > - Email IDs & phone numbers
   > - Website technologies
   > - Physical locations

- [X] **🖌️ Collect Network Information**
   > - Domain names
   > - IP addresses
   > - DNS records
   > - WHOIS information
   > - Network range

- [X] **🖌️ Collect System Information**
   > - Operating system details
   > - Web server type & location
   > - Hostnames
   > - Usernames (if exposed)

- [X] **🖌️ Gather Open-Source Intelligence (OSINT)**
   > - Search engines
   > - Social media
   > - Public documents
   > - Job portals

- [X] **🖌️ Perform Active Footprinting (If Authorized)**
   > - Ping
   > - Traceroute
   > - DNS queries
   > - Email enumeration

- [X] **🖌️ Document & Analyze Information**
   > - Identify weak points
   > - Prepare for scanning phase
   > - Reduce detection risk

---
## 💻 Practical of Information Gathering

**1.** **Find on Search Engines**
  > - Search engines are the **first & main source** of key information about the target Organization.
  > - Example :- Yahoo, **Google**, Bing, Duck Duck Go.

- You can see Below, I want to know Information about cyberyaan.
 > - **Go on Search engines and search it - Cyberyaan.**

- Image link

- [ ] Attackers use search engines to gather information about a target :— such as technologies used, **employee details, and login portals** — to *support social engineering and advanced attacks.*

- [ ] Attackers can use advanced search operators available with these search engines and **create complex queries to find, filter, and sort** specific information about the target. Example - Googel Dorking.

- **📵 Google Dorking :-**
Google Dorking is a technique that uses **advanced Google search operators** to find sensitive or hidden information about a target.

> - **Target Name -** Cyberyaan.com
> - Search it on google to see something unique.

   > - **site:cyberyaan.com**
   > - site:cyberyaan.com filetype:pdf
   > - site:cyberyaan.com email
   > - site:cyberyaan.com "confidential"

- image link

**2.** **Find on Social Networking Platforms**
> - It is the way of collecting publicly available **information from social media sites** like instagram, facebook.
> - People unaware & they post every moment of his life without knowing that they are **leaking information himself on internet.**
> - These collected information are **helpful for attacker.**

- **Nowadays almost all people are highly active in social media networks, jobs sites, etc.**

   > - Social networking services, such as Facebook, Twitter, and LinkedIn, provide useful information about the individual **that helps the attacker in performing social engineering** and other attacks.

    > - The people search can provide critical information about a person or an organization, **including location, emails, websites, blogs, contacts,** important dates, etc.

    > - People search online services, that  provide people's **names, addresses, contact details, date of birth**, photographs, videos, profession, and so much.

- **➿ U.S based Websites to Search :-**
    > -  **Spokeo, Intelius, pipl, BeenVerified, Whitepages, and PeekYou,**

- **➿ India based Websites to Search :-**
India has strict privacy laws, so options are limited:

   > - **Truecaller –** Best for phone number identity
   > - **Google Dorking –** Search name + email + username
   > - **LinkedIn –** Professional identity verification
   > - **Facebook / Instagram / X –** Profile cross-verification
   > - **Voter list / Company MCA site –** Legal public records only

- [ ] **➿ Used by cybersecurity & investigators (ethical use only):**

   > - **WhatsMyName –** Username lookup across platforms **::--** [Click to Open Website](https://whatsmyname.me/)
   > - **Social Searcher –** Social media mentions  **::--** [1st Website](https://www.social-searcher.com/) [2nd Website](https://socialsearcher.net/)
   > - **Hunter.io –** Email domain verification  **::--** [Click to Open Website](https://hunter.io/)
   > - **Maltego –** Advanced relationship mapping (professional) **::--** **[Best in Kali Linux]**

**3.** **Find on Web Service**
 > - Hacker tries to gain information from web services like **job site, groups, social networks, forums** etc to gain sensitive information.

**4.** **Find thorugh DNS (Domain Name System)**
DNS turn domain name into Ip address for the browser.

   > - DNS or Domain Name System footprinting reveal the DNS zone data like **DNS server name , DNS records, IP address , domain mail server** , etc .
   > - We use some tools for **DNS footprinting**

- **📧 Nslookup :-** [Click to Open Website](https://www.nslookup.io/)
   > - Search - cyberyaan.com

link photo

- **📧 Whoislookup :-** [Click to Open Website](https://whois.domaintools.com/)
   > - Search - cyberyaan.com

link photo

- **📧 MxtoolBox :-** [Click to Open Website](https://mxtoolbox.com/whois.aspx)
   > - Search - cyberyaan.com

link photo


- **📧 Netcraft :-** [Click to Open Website](https://sitereport.netcraft.com/)
   > - Search - cyberyaan.com

link photo

---
## ➿ Footprinting through social engineering
Footprinting through social engineering is the process of collecting information about a target (person or organization) by interacting with people.
  > - **Attackers exploit human psychology—trust, fear, curiosity, or authority—to extract sensitive details.**

- **To Gather Info:**

  > - Employee names & roles
  > - Email IDs & phone numbers
  > - Internal processes
  > - Technologies used
  > - Security policies (often unintentionally revealed)

- **Shoulder surfing :-** Observing a victim to steal sensitive information.

- **Dumpster diving :-** Collecting confidential data from discarded materials.

- **Impersonation :-** Pretending to be a trusted identity to deceive victims.

---
## 🧩 Types of Social Engineering Used in Footprinting
- **1️⃣ Pretexting :-** Attacker creates a fake scenario to gain trust.

  Example : “Hi, I’m from the IT support team. We’re updating the email server—can you confirm your username?”

- [X] **Information collected:**
  
  > - Usernames
  > - Department structure
  > - IT procedures

- 2️⃣ **Phishing (Email-Based) :-** Malicious emails designed to trick users into revealing data.

   Example : Fake HR email asking employees to “verify details”

- [X] **Collected info:**

  > - Login credentials
  > - Email format (firstname.lastname@company.com)
  > - Employee responses

- 3️⃣ **Vishing (Voice Phishing) :-** Phone calls impersonating authority.

   Example : “This is the bank security team. We detected suspicious activity.”

- [X] **Collected info:**

  > - DOB
  > - Account hints
  > - Verification process

- 4️⃣ **Smishing (SMS Phishing) :-** Malicious text messages.

   Example : “Your courier is delayed. Track here: [link]”

- [X] **Collected info:**

  > - Phone numbers
  > - Device type
  > - Location indicators

- 5️⃣ **Impersonation :-** Pretending to be: New employee , Vendor , Auditor , Delivery staff.

- [X] **Collected info:**

  > - Office layout
  > - Badge policies
  > - Employee schedules

- 6️⃣ **Baiting :-** Offering something attractive.

  Example : Free USB drive labeled “Salary Details”

- [X] **Collected info:**

  > - System behavior
  > - Auto-run settings
  > - Antivirus presence

- 7️⃣ **Tailgating :-** Following an employee into restricted areas.

- [X] **Collected info:**

  > - Physical security controls
  > - Badge enforcement

---
## 🐉 Kali Linux Footprinting Tools

- **theHarvester :-** Collects emails, subdomains, hosts from public sources
- **Maltego :-** Graph-based OSINT and relationship mapping
- **Recon-ng :-** Modular web reconnaissance framework
- **dnsrecon :-**	DNS zone and record discovery
- **dig :-**	DNS record lookup
- **nslookup :-**	DNS queries
- **whois :-** Domain registration info

---
---
# 🫸🏻 Lab & Practical Questions

- [X] Perform search engine footprinting to find publicly available documents related to a target organization.
- [ ] Collect employee details of an organization using social networking sites.
- [ ] Identify the web technologies used by a target website.
- [ ] Perform DNS footprinting to obtain A, MX, and NS records of a domain.
- [ ] Conduct a WHOIS lookup to gather domain registration information.
- [ ] Trace the network path to a target system using a network footprinting technique.
- [ ] Analyze an email header to identify the sender’s IP address and mail server.
- [ ] Extract metadata from a publicly available document to identify usernames and software details.

---
---

## 📌 Well-structured table based on the Footprinting Methodology diagram

| **Category**                | **Footprinting Technique**                   | **Description / What is Collected**                                      |
| --------------------------- | -------------------------------------------- | ------------------------------------------------------------------------ |
| **Search Engines**          | Advanced Google Hacking                      | Uses Google dorks to find sensitive files, directories, and exposed data |
|                             | Google Hacking Database & Advanced Search    | Predefined dorks and filters to locate misconfigurations                 |
|                             | Video, Meta, FTP, IoT Search Engines         | Finds cameras, FTP servers, metadata, and IoT devices                    |
|                             |                                              |                                                                          |
| **Web Services**            | People Search Services                       | Finds personal details like name, email, phone number                    |
|                             | Financial Services & Job Sites               | Job roles, salary patterns, technologies used                            |
|                             | Deep & Dark Web Footprinting                 | Leaked credentials, hidden services, underground data                    |
|                             | Competitive Intelligence & Business Profiles | Company size, partners, revenue, market position                         |
|                             | Monitor Alerts & Online Reputation           | Brand mentions, leaks, reputation tracking                               |
|                             |                                              |                                                                          |
| **Social Networking Sites** | Social Engineering                           | Extracts info by interacting with people                                 |
|                             | Social Media Sites                           | Employee details, locations, habits, technologies                        |
|                             | Analyzing Social Network Graphs              | Relationship mapping between employees                                   |
|                             | Groups, Forums, Blogs, NNTP                  | Discussions revealing internal or technical info                         |
|                             | Public Source Code Repositories              | API keys, credentials, internal logic (GitHub, GitLab)                   |
|                             |                                              |                                                                          |
| **Website Footprinting**    | Web Spiders & Website Mirroring              | Copies entire website structure                                          |
|                             | Internet Archive                             | Accesses old versions of websites                                        |
|                             | Extract Links, Wordlists, Metadata           | Hidden directories, usernames, file info                                 |
|                             | Monitor Web Page Updates & Traffic           | Change detection and usage patterns                                      |
|                             |                                              |                                                                          |
| **Email Footprinting**      | Track Email Communication                    | Identifies email patterns and flows                                      |
|                             | Analyze Email Header                         | Finds sender IP, mail server, routing path                               |
|                             |                                              |                                                                          |
| **Whois Footprinting**      | Whois Lookup                                 | Domain owner, registrar, creation date                                   |
|                             | IP Geolocation Lookup                        | Physical location of IP address                                          |
|                             |                                              |                                                                          |
| **DNS Footprinting**        | DNS Interrogation                            | DNS records (A, MX, NS, TXT, SOA)                                        |
|                             | Reverse DNS Lookup                           | Maps IP addresses to domain names                                        |
|                             |                                              |                                                                          |
| **Network Footprinting**    | Locate Network Range                         | Identifies IP ranges used by organization                                |
|                             | Traceroute                                   | Discovers network path and devices                                       |
|                             |                                              |                                                                          |
| **Social Engineering**      | Eavesdropping                                | Listening to conversations                                               |
|                             | Shoulder Surfing                             | Observing passwords or sensitive data                                    |
|                             | Dumpster Diving                              | Collecting info from discarded material                                  |
|                             | Impersonation                                | Pretending to be a trusted person                                        |
|                             |                                              |                                                                          |


---
---
