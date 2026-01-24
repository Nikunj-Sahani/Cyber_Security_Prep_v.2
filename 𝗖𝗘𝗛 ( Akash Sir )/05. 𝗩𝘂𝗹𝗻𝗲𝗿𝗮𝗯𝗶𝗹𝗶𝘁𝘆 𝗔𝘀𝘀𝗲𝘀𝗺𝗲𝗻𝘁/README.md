<h1 align="center">🖥️ Day 05 🖥️</h1>
<h2 align="center">🎚️ Vulnerability Assessment 🎚️</h2>

---
## What is Vulnerability Assessment?
Vulnerability analysis is a part of the scanning phase.
  
  > - The process of identifying, evaluating, and prioritizing **security weaknesses in systems or networks.**

- **Vulnerability Assessment** is a fundamental task for a penetration tester to **identify security weaknesses** in an environment.
- It involves finding system flaws, design issues, and security gaps that could be exploited in an operating system, application, or website.
- The assessment mainly focuses on **vulnerability impact and vulnerability ranking.**

### 🔍 Types of Vulnerabilities

 > - **Misconfiguration –** Incorrect or insecure system settings

 > - **Default Configuration –** Using default usernames, passwords, or settings

 > - **Design Flaws –** Weaknesses in system or application design

 > - **Buffer Overflow –** Excess data overwrites memory causing crashes or code execution

 > - **Operating System Flaws –** Vulnerabilities in the OS

 > - **SQL Injection –** Injecting malicious SQL queries into applications

 > - **XSS (Cross-Site Scripting) –** Injecting malicious scripts into web pages

👉 These vulnerabilities are commonly identified during a Vulnerability Assessment.

- **Vulnerability Divides in Four Categories**

   > - **Low**    :::: _L1_
   > - **Medium** :::: _L2_
   > - **High**   :::: _L3_
   > - **Critical** :::: _L4_

## 🔍 Types of Vulnerability Assessment

 > - **Active Assessment –** Direct interaction with systems

 > - **Passive Assessment –** Indirect monitoring without interaction

 > - **External Assessment –** Testing from outside the organization

 > - **Internal Assessment –** Testing from inside the organization

 > - **Host-Based Assessment –** Assessing a single system or PC

 > - **Network Assessment –** Assessing network devices and services

 > - **Application Assessment –** Assessing web or mobile applications

 > - **Wireless Network Assessment –** Assessing Wi-Fi security

### 🔁 Vulnerability Management Life Cycle

 - [X] **Identify –** Discover vulnerabilities
 - [X] **Assess –** Analyze risk and severity
 - [X] **Prioritize –** Rank vulnerabilities
 - [X] **Remediate –** Fix or mitigate issues
 - [X] **Verify –** Re-test to confirm fixes
 - [X] **Monitor –** Continuously track new vulnerabilities

---
## 📊 Vulnerability Scoring System

- **1. CVSS (Common Vulnerability Scoring System) -** It assigns a score from 0.0 to 10.0 to indicate vulnerability severity:

| Severity | CVSS Score Range |
| -------- | ---------------- |
| None     | 0.0              |
| Low      | 0.1 – 3.9        |
| Medium   | 4.0 – 6.9        |
| High     | 7.0 – 8.9        |
| Critical | 9.0 – 10.0       |

   > - 👉 _Higher score = more severe vulnerability._


- **2. CVE (Common Vulnerabilities and Exposures) –** Provides a unique ID for publicly known vulnerabilities.
  - [X] CVE-2023-12345

  - [X] Easy to track, reference, and share across security tools and databases.
 
    > - MITRE CVE ::: [Link to Go](http://cve.mitre.org)
    > - Exploit DataBase  ::: [Link to Go](https://www.exploit-db.com/)

- **3. National Vulnerability Database (NVD) -**
  - [X] A government-maintained database that gives detailed **vulnerability information linked to CVE and CVSS.**

     > - Vulnerability Database ::: [Link to Go](https://nvd.nist.gov)

---
## Vulnerability Assessment Tools
👉 Used to identify, analyze, and prioritize vulnerabilities in systems and applications.

 > - **Nmap :-** Network scanning tool used to discover live hosts, open ports.
 > - **Nikto :-** Web server vulnerability scanner.
 > - **OWASP ZAP :-** Security testing tool used to find vulnerabilities like SQL Injection and XSS in web applications.
 > - **Burp Suite :–** Web application vulnerability testing.
 > - **Nessus :-** Popular vulnerability scanner.
 > - **Accunetix :-** Automated web application vulnerability scanner used to detect issues such as SQL, XSS, CSRF.
 > - **Nexpose (InsightVM) :-** Risk-based vulnerability management.
 > - **OpenVAS (GVM) :–** Open-source vulnerability assessment tool.
 > - **Legion :-** Performs scanning, enumeration, and service discovery using multiple integrated tools.   
 > - **Qualys :-** Cloud-based vulnerability scanning.

### Link to Go the Websites::-

- [X] **Use in Linux :-** Nikto | Legion | Nmap | OpenVAS |
  
[Nmap](https://nmap.org/download.html#windows) || [OwaspZAP](https://www.zaproxy.org/download) || [Burp Suite Community](https://portswigger.net/burp/communitydownload) || [Nessus](https://www.tenable.com/downloads?loginAttempted=true) || [Accunetix](https://www.acunetix.com/support/docs/wvs/installing-acunetix-wvs/) || [Nexpose](https://www.rapid7.com/products/nexpose/) || [OpenVAS](https://github.com/greenbone/openvas-scanner) || [Legion](https://github.com/Abacus-Group-RTO/legion) || [Qualys](https://www.qualys.com/community-edition)



---
## 🕹️ Example 1 🕹️ Vulnerability Assessment of a Web Application

- **Scope Definition ::**

    > - **System:-** E-commerce web application
    > - **Components:-** Web server, application server, database server
    > - **Assessment Tools:-** Nmap, OpenVAS, OWASP ZAP, Nessus

- **Data Colllection ::**

    > - **Network Scanning :–** Using Nmap to identify live hosts, open ports, and running services.
    > - **Vulnerability Scanning :–** Using OpenVAS and Nessus to detect known security vulnerabilities.
    > - **Web Application Scanning :–** Using OWASP ZAP to identify web application vulnerabilities such as XSS and SQL Injection.

- **Perform Assessement ::**

    > - 



                                                                                                                                                                                                                                                                                                                                                                                                        
