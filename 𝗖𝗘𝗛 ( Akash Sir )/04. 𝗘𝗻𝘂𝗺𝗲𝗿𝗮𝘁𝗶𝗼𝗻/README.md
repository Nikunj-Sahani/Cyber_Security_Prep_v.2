<h1 align="center">🖥️ Day 04 🖥️</h1>
<h2 align="center">📊 Enumeration 📊</h2>

---
## What is Enumeration ?
Enumeration is the process of gathering detailed information about a target system, network, or application.

> - It happens during the early phase of ethical hacking or penetration testing, which is called **"reconnaissance."**
> - The goal is to **find weaknesses or potential security flaws** in the target.

- [ ] Actively extracting **detailed information from a target** system after scanning. _Such as_
 
  > - Usernames
  > - Computer names
  > - Shared files or resources
  > - Running services

## Common Enumeration Techniques:

- 1️⃣ **NetBIOS Enumeration →** The process of gathering system information.
  - [ ] It is a protocol used for communication between Windows systems in a local network.
  - [ ] **During NetBIOS enumeration,** attackers gather information about:

     > - Computer names
     > - Usernames
     > - Shared folders or files
     > - Workgroup or domain names

     - [X] **Tools used :** NBTscan, Net view, nbtstat

- 2️⃣ **SNMP Enumeration →** Used for managing devices like routers, switches, and printers in a network.
   - [ ] By performing SNMP enumeration, **attackers can collect:**

      > - Network device information
      > - Device configurations
      > - Usernames, passwords, and other sensitive data

      - [X] **Tools used :** snmpwalk, snmpget, snmpenum

- 3️⃣ **LDAP Enumeration →** Commonly used for managing directories like Active Directory (AD).
   - [ ] Through LDAP enumeration, **attackers can gather:**

      > - Usernames
      > - Email addresses
      > - Group memberships
      > - Organizational units

      - [X] **Tools used :** ldapsearch, Nmap, Ldapenum 

- 4️⃣ **NTP Enumeration →** Gathering time server and network information from systems using the NTP protocol.
   - [ ] It is used to synchronize clocks on networked devices.
   - [X] NTP enumeration involves **querying NTP servers to discover:**

      > - Server information
      > - Connected devices
      > - Potential vulnerabilities in timesync configurations

      - [X] **Tools used :** ntpdc, ntpq, Nmap

- 5️⃣ **SMTP Enumeration →** 



 > - **User Account Enumeration –** Finding valid usernames on a system.

 > - **Network Resource Enumeration –** Discovering shared folders and drives.

 > - **Service Enumeration –** Identifying running services and their versions.

 > - **SNMP Enumeration –** Collecting device and network configuration details.

 > - **DNS Enumeration –** Gathering DNS records to find hostnames and IP addresses.



