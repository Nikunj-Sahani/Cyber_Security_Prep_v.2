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

- **3. National Vulnerability Database (NVD) -** A government-maintained database that gives detailed **vulnerability information linked to CVE and CVSS.**

   > - https://nvd.nist.gov ::: [Link to Go](https://nvd.nist.gov)





