# 🔐 Web Reconnaissance & Network Scanning

**Performing information gathering, web technology fingerprinting, DNS enumeration, and network scanning using Kali Linux.**

<p align="center">
  <img src="https://img.shields.io/badge/Skill-Cybersecurity-404040?style=flat-square&labelColor=C00000" />
  <img src="https://img.shields.io/badge/OS-Kali%20Linux-E87500?style=flat-square&logo=kalilinux&logoColor=white" />
  <img src="https://img.shields.io/badge/Tools-Nmap%20%7C%20Zenmap-0070C0?style=flat-square" />
  <img src="https://img.shields.io/badge/Tools-Dig%20%7C%20Nslookup-238F89?style=flat-square" />
  <img src="https://img.shields.io/badge/Network-Reconnaissance-C00000?style=flat-square" />
  <img src="https://img.shields.io/badge/NetworkWalks-404040?style=flat-square&labelColor=C00000" />
  <img src="https://img.shields.io/badge/Ethical%20Hacking-E87500?style=flat-square" />
</p>

---

## 📌 Project Overview

This project focuses on practicing **Information Gathering (Reconnaissance)** and **Network Scanning** using various tools available in Kali Linux.

The practical activities were divided into two main modules:
W2-PM1: Information Gathering & Web Reconnaissance using Kali Linux Tools
W2-PM3: Information Gathering using Maltego
W2-PM4: Information Gathering & Web Reconnaissance using theHarvester
W2-PM5: Network Scanning using Zenmap

The first module involved gathering information about a target domain, identifying web technologies, inspecting HTTP response headers, and querying DNS records.

The second module focused on scanning the local area network (LAN) to discover active devices and identify open ports.

These exercises provided practical experience in understanding how reconnaissance techniques support the initial stages of a penetration testing assessment.

---

## 🎯 Objectives

The main objectives of this project are to:

- Perform DNS lookups and identify domain IP addresses.
- Identify web technologies using WhatWeb.
- Inspect HTTP response headers using cURL.
- Enumerate DNS information using Dig.
- Understand the information exposed by web infrastructure.
- Discover active devices within a local network.
- Identify open ports using Zenmap.
- Practice network reconnaissance using Kali Linux tools.

---

## 🛡️ Purpose of the Project

Reconnaissance is an important initial phase of penetration testing. It helps security professionals understand the target environment before conducting further security assessments.

This project focuses on developing practical skills in:

- DNS Enumeration
- Web Technology Fingerprinting
- HTTP Header Analysis
- Information Gathering
- Network Host Discovery
- Port Scanning
- Network Mapping

⚠️ **Important:** All scanning and testing activities must be performed only against systems and networks that you own or have explicit authorization to assess.

---

## ⚙️ Tools & Technologies

| 🧩 Tool | 🎯 Purpose |
|---|---|
| Kali Linux | Security testing environment |
| Nslookup | DNS lookup and IP resolution |
| WhatWeb | Web technology fingerprinting |
| cURL | HTTP header inspection |
| Dig | DNS information enumeration |
| Zenmap | Network scanning and visualization |
| Nmap | Host discovery and port scanning |

---

# 🪜 Practical Implementation

## Module W2-PM4: Information Gathering & Web Reconnaissance

This module focused on collecting information about the target domain `networkwalks.com` using different reconnaissance utilities available in Kali Linux.

### 1. DNS Lookup (Nslookup)

**Tool:** Nslookup

The `nslookup` command was used to query DNS information and identify the IP address associated with the target domain.

**Command:**

```bash
nslookup networkwalks.com
```

**Result:**

Successfully resolved the domain name to its corresponding IP address.

**Screenshot:**

<p align="center">
  <img src="nslookup.png" width="850" alt="Nslookup DNS lookup results">
</p>

**Key Concept:**

DNS resolution translates human-readable domain names into IP addresses that computers use to communicate over networks.

---

### 2. Web Technology Fingerprinting (WhatWeb)

**Tool:** WhatWeb

WhatWeb was used to identify technologies and software components associated with the target website.

**Command:**

```bash
whatweb networkwalks.com
```

**Result:**

Identified information about the web server technologies and Content Management System (CMS) used by the website.

**Screenshot:**

<p align="center">
  <img src="wwebss.png" width="850" alt="WhatWeb technology fingerprinting results">
</p>

**Key Concept:**

Technology fingerprinting helps security professionals understand the technologies running behind a website and identify potential areas for further security assessment.

---

### 3. HTTP Header Inspection (cURL)

**Tool:** cURL

The `curl` utility was used to inspect the HTTP response headers returned by the target web server.

**Command:**

```bash
curl -I https://networkwalks.com
```

**Result:**

Retrieved the HTTP response headers and checked the server response status and available header information.

**Screenshot:**

<p align="center">
  <img src="curl-i.png" width="850" alt="cURL HTTP response headers">
</p>

**Key Concept:**

HTTP headers can reveal useful information about server behavior, response configuration, and potentially exposed technologies.

---

### 4. DNS Records Enumeration (Dig)

**Tool:** Dig

The `dig` command was used to query DNS information associated with the target domain.

**Command:**

```bash
dig networkwalks.com ANY
```

**Result:**

Queried the DNS server for available DNS record information associated with the domain.

**Screenshot:**

<p align="center">
  <img src="dnsrconss.png" width="850" alt="Dig DNS enumeration results">
</p>

**Key Concept:**

DNS enumeration helps security professionals understand domain configuration and gather information about the target's DNS infrastructure.

---

## Module W2-PM5: Network Scanning with Zenmap

This module focused on discovering active devices and identifying open ports within the local area network (LAN).

**Tool:** Zenmap (Nmap GUI)

### Scan Configuration

| 🧩 Parameter | ⚙️ Configuration |
|---|---|
| Target Scope | Local Area Network (LAN) |
| Scanning Tool | Zenmap |
| Scan Types | Intense Scan / Ping Scan |
| Main Objective | Host Discovery & Port Identification |

### Scanning Procedure

1. Install and opened Zenmap.
2. Specified the local network as the scan target.
3. Selected the appropriate scanning profile.
4. Executed the scan to discover active devices.
5. Reviewed the scan results to identify available hosts and open ports.

### Summary of Findings

The local network was successfully scanned, and active devices connected to the network were identified.

The scan also helped identify open ports on the discovered devices.

**Screenshot:**
<p align="center">
  <img src="nmapss2.png" width="850" alt="Dig DNS enumeration results">
</p>
**Key Concept:**

Network scanning helps security professionals map network environments, discover active hosts, and identify accessible services.

---

## 🔎 Results & Findings

The following table summarizes the activities performed during the practical exercises:

| 🔍 Activity | 🛠️ Tool | ✅ Result |
|---|---|---|
| DNS Lookup | Nslookup | Domain resolved to an IP address |
| Technology Fingerprinting | WhatWeb | Web technologies and CMS identified |
| HTTP Header Inspection | cURL | HTTP response headers retrieved |
| DNS Enumeration | Dig | DNS information queried |
| Host Discovery | Zenmap | Active local network devices identified |
| Port Scanning | Zenmap | Open ports identified |

---

## 💡 What I Learned

Through these practical exercises, I gained a better understanding of reconnaissance techniques and network scanning.

The most important concepts I learned include:

### 1. DNS Enumeration

I learned how DNS lookup utilities such as Nslookup and Dig can be used to retrieve domain-related information and understand DNS resolution.

### 2. Web Technology Fingerprinting

I learned how WhatWeb identifies technologies and software components used by websites, which can help during the initial information-gathering phase.

### 3. HTTP Header Analysis

I learned how to retrieve and inspect HTTP response headers using cURL and understand the information that web servers expose through their responses.

### 4. Network Host Discovery

I gained practical experience using Zenmap to discover active devices within a local network and understand how network scanning identifies connected hosts.

### 5. Port Scanning

I learned how port scanning helps identify open ports on discovered devices, providing useful information about potentially accessible network services.

### 6. Reconnaissance Methodology

I understood how different information-gathering tools complement one another during the reconnaissance phase of a penetration testing assessment.

---

## 🔐 Security & Ethical Use

These activities were conducted for educational purposes as part of the NetworkWalks cybersecurity training program.

All network scanning activities should remain within authorized testing environments and approved network scopes.

The information gathered during reconnaissance should be handled responsibly and used only for legitimate security assessment purposes.

---

## 👤 Author

**Irshad Hussain**

Cybersecurity Student 

---

## 📌 Project Information

- **Program:** Cybersecurity Internship | NetworkWalks
- **Week:** 02
- **Module W2-PM4:** Information Gathering & Web Reconnaissance
- **Module W2-PM5:** Network Scanning with Zenmap
- **Environment:** Kali Linux
- **Focus:** Web Reconnaissance & Network Scanning

