<h1 align="center">📕 Day 02 ✏️</h1>

---
### Types of Address
- Logical - IP Address
- Physical - MAC Address
  
## IP Address : Logical Address - Assigned online 
IP address is a unique numerical label assigned to every device connected to a network.

- **Why called Logical ::** Because IP is format of Bits and made with Binary Number.
 - Addresses can be assigned dynamically via DHCP.
 - **If DHCP Failed ♻️ APIPA** assigned IP automatically in range of **169.254.0.1 to 169.254.255.254.**


## MAC Address : Physical Address - Assigned to Device
A MAC address is a unique hardware identifier assigned to a device’s network interface card (NIC).

---
# IP Address :: Detailed ::
 - Two types of IP
  > - IPv4
  > - IPv6

## 🗳️ **IPv4 :** IPv4 is the 4th version of the Internet Protocol
 - [ ] It is used to identify devices on a network.
 - [ ] It using a **32-bit address**
 - [ ] Written as **four decimal numbers** (0–255) separated by dots.
  > - **Example :** 192.168.1.1
 - [ ] Each address has two parts:
  > - **Network ID →** identifies the network.
  > - **Host ID →** identifies the device within that network.

### Octate in IP Address
- [ ] 4 octate in Ipv4 address - **192.168.1.0**

   > - 192 : **1st Octate**
   > - 168 : **2nd Octate**
   > - 1 : **3rd Octate**
   > - 0 : **4th Octate**

### Bit in IP Address
- [ ] Ipv4 address made by 32 bit - **192.168.1.0**
- [ ] One Octate takes 8 bit.

   > - 192 : **8-bit**
   > - 168 : **8-bit**
   > - 1 : **8-bit**
   > - 0 : **8-bit**

  - **192.168.1.0 :: 32-bit**

### Classes of IP
- [ ] 4 classes in IPv4.
- [ ] Class - A : B : C : D

   > - Class A :: **1 - 127**
   > - Class B :: **128 - 191**
   > - Class C :: **192 - 223**
   > - Class D :: **224 - 239**
 
  - *Mainly Used* :: **Class-C IP : 192.168.1.0**

### Parts of IP Address
Every IPv4 address has two Parts
> - Network Part
> - Host Part

- **IP of Class A** - 10.10.1.1

  > - 10 : Network
  > - 10 : Host
  > - 1 : Host
  > - 1 : Host

- **IP of Class B** - 128.10.1.0

  > - 128 : Network
  > - 10 : Network
  > - 1 : Host
  > - 0 : Host

- **IP of Class C** - 192.50.1.1

  > - 192 : Network
  > - 50 : Network
  > - 1 : Network
  > - 1 : Host

- **Table For Understand**

|         Class         | 1st | 2nd | 3rd | 4th |
|-----------------------|-----|-----|-----|-----|
| Class A - 10.10.1.1   |  N  |  H  |  H  |  H  |
| Class B - 128.10.1.0  |  N  |  N  |  H  |  H  |
| Class C - 192.50.1.1  |  N  |  N  |  N  |  H  |

---
### Binary to Decimal - IP Bit
Each octet (8 bits) is converted from binary → decimal to form a IP address.

- Formula : **Binary Number * 2ⁿ⁽ᵇⁱⁿᵃʳʸ ᵖᵒˢⁱᵗⁱᵒⁿ ᵛᵃˡᵘᵉ⁾**
> - **n * 2ⁿ**
> - **IP 192.168.1.0 - Describe in Bit**
<div style="text-align: center;"><img src="https://github.com/Nikunj-Sahani/Cyber_Security_Prep_v.2/blob/main/Images/B-D-1.png" alt="Sample Image"></div>

---
### 🥎 8 - Bit
 - **We can create 256 numbers using 8 - bits**
 - **Example -** 1  0  1  0  0  0  0  1 

| S.No. | Binary | Position | Binary to Number |
|-------|--------|----------|------------------|
|   1   |   0    |     0    |    0 * 2⁰ = 0    |
|   2   |   0    |     1    |    0 * 2¹ = 0    |     
|   3   |   0    |     2    |    0 * 2² = 0    |     
|   4   |   0    |     3    |    0 * 2³ = 0    |     
|   5   |   0    |     4    |    0 * 2⁴ = 0    |     
|   6   |   0    |     5    |    0 * 2⁵ = 0    |     
|   7   |   0    |     6    |    0 * 2⁶ = 0    |     
|   8   |   0    |     7    |    0 * 2⁷ = 0    |     

### How can we define with Different Bit ?
For better mindset, we differentiate the bit,

 > - If someone ask for : 8 - bit
 > - If someone ask for : 4 - bit
 > - If someone ask for : 3 - bit
 > - If someone ask for : 2 - bit

### 🥎 4 - Bit
  We define using 4 - bit
  - How many Numbers can create using 4 - bit ?
  - **We can create 16 numbers using 4 - bits**

| Binary | Binary | Binary | Binary |  
|--------|--------|--------|--------|
|  0000  |  0100  |  1000  |  1100  | 
|  0001  |  0101  |  1001  |  1101  |
|  0010  |  0110  |  1010  |  1110  |
|  0011  |  0111  |  1011  |  1111  |

### 🥎 3 - Bit
  We define using 2 - bit
  - How many Numbers can create using 3 - bit ?
  - **We can create 8 numbers using 3 - bits**

| Binary | Binary |  
|--------|--------|
|   000  |   100  |
|   001  |   101  | 
|   010  |   110  |
|   011  |   111  |  

### 🥎 2 - Bit
  We define using 2 - bit
  - How many Numbers can create using 2 - bit ?
  - **We can create 4 numbers using 2 - bits**

| Binary |
|--------|
|   00   |
|   01   |
|   10   |
|   11   |

### For Recall IP - Bit
- Using **8 - Bit = 256 Numbers**
- Using **7 - Bit = 128 Numbers**
- Using **6 - Bit = 64 Numbers**
- Using **5 - Bit = 32 Numbers**
- Using **4 - Bit = 16 Numbers**
- Using **3 - Bit = 8 Numbers**
- Using **2 - Bit = 4 Numbers**

---
## 🗳️ IPv6
IPv6 is the newer version of IP created to **overcome the IPv4 address shortage.**
 - **IPv6 uses 128 bits**, offering *340 undecillion (3.4×10³⁸) addresses.*

### IPv6 Address Format

- [ ] It uses **128-bits IPv6 Address**
- [ ] Written in 8 groups of 4 **hexadecimal digits**
- [ ] 1 Group of Ip - **16 bits**
- [ ] Separated by colons **:**

> - Example :- **2001:0db8:0000:0000:0000:ff00:0042:8329**

### Auto Configuration of IPv6
No need for DHCP in many cases.
- **It auto configure the IPv6 using SLAAC.**

- The device automatically forms its IP:
  > - Takes prefix from router
  > - Uses MAC address or random value
  > - Generates full 128-bit IPv6 address

---
---
