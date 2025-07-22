# 🧠 Cybersecurity & Networking Foundations – TryHackMe Notes
_This repository contains my detailed learning notes from TryHackMe rooms up to "Network Essentials", including Pre-Security, Network Fundamentals, and hands-on experience with Linux, Windows CMD, and PowerShell._

---

## 🌐 OSI Model – The 7 Layers of Networking

| Layer Number | Layer Name     | Description |
|--------------|----------------|-------------|
| 7️⃣           | Application     | Closest to the user – handles protocols like HTTP, HTTPS, FTP, DNS |
| 6️⃣           | Presentation    | Translates, encrypts, or compresses data (e.g., SSL/TLS) |
| 5️⃣           | Session         | Manages sessions and connections between applications |
| 4️⃣           | Transport       | Provides reliable (TCP) or unreliable (UDP) delivery of data |
| 3️⃣           | Network         | Handles logical addressing and routing (IP addresses) |
| 2️⃣           | Data Link       | Responsible for MAC addressing and switching |
| 1️⃣           | Physical        | Physical medium: cables, NICs, switches |

---

## 🛰️ TCP vs UDP

### TCP (Transmission Control Protocol)
- Connection-oriented
- Guarantees delivery with acknowledgments (ACKs)
- Supports flow control and error checking
- Slower but reliable
- Used in HTTPS, SSH, FTP

### UDP (User Datagram Protocol)
- Connectionless
- No guarantee of delivery, order, or integrity
- Much faster due to low overhead
- Used in DNS, VoIP, video streaming, games

---

## 🏷️ IP Addressing

### IPv4
- 32-bit address: `e.g. 192.168.1.1`
- Four octets separated by dots
- Common private ranges:
  - 10.0.0.0 – 10.255.255.255
  - 172.16.0.0 – 172.31.255.255
  - 192.168.0.0 – 192.168.255.255

### IPv6
- 128-bit address: `e.g. fe80::1ff:fe23:4567:890a`
- Designed to replace IPv4 due to exhaustion

### Public vs Private IP
- **Private IPs** are not routable on the internet
- **Public IPs** are globally unique and internet routable

---

## 🧭 DNS – Domain Name System

- Resolves domain names to IP addresses
- Works primarily over **UDP port 53** (TCP for large responses)
- Hierarchical system:
  - Root → TLD → Domain → Subdomain
- Example:
  - `www.google.com` ➜ `142.250.64.78`
- Common record types:
  - A, AAAA, MX, CNAME, NS, TXT

---

## 🌍 HTTP vs HTTPS

| Protocol | Port | Description |
|----------|------|-------------|
| HTTP     | 80   | Unencrypted web communication |
| HTTPS    | 443  | Encrypted with SSL/TLS |

---

## 🔐 Common Protocols and Their Default Ports

| Protocol | Port | Use |
|----------|------|-----|
| HTTP     | 80   | Unencrypted web |
| HTTPS    | 443  | Secure web |
| FTP      | 21   | File transfers |
| SSH      | 22   | Secure remote access |
| DNS      | 53   | Domain resolution |
| SMTP     | 25   | Sending email |
| POP3     | 110  | Receiving email (older) |
| IMAP     | 143  | Receiving email (modern) |

---

## 🧩 MAC Address vs IP Address

### MAC Address
- Hardware address unique to each device
- Format: `00:1A:2B:3C:4D:5E`
- Assigned by NIC manufacturers
- Works on Layer 2 (Data Link)

### IP Address
- Logical, changeable address used for routing
- Works on Layer 3 (Network)
- Can be dynamically assigned (DHCP) or static

---

## 📡 DHCP – Dynamic Host Configuration Protocol

- Automatically assigns:
  - IP Address
  - Subnet Mask
  - Default Gateway
  - DNS Server
- Operates over **UDP ports 67 (server) and 68 (client)**

---

## 🧱 Firewalls & NAT

### Firewalls
- Enforce rules to block/allow traffic
- Can filter by:
  - IP Address
  - Port
  - Protocol (TCP/UDP/ICMP)

### NAT (Network Address Translation)
- Allows multiple private IPs to share a public IP
- Used in routers to translate between internal and external networks

---

## 🧮 Subnetting Basics

- Used to divide larger networks into smaller, manageable sub-networks
- CIDR notation: `192.168.1.0/24`
  - /24 = 255.255.255.0 → 256 IPs total (254 usable)
- Helps in better IP management, isolation, and security

---

## 💻 Linux Terminal Experience

- Navigated Linux filesystems using:
  - `ls`, `cd`, `pwd`, `cat`, `less`, `touch`, `nano`, `vim`
- Managed permissions with:
  - `chmod`, `chown`, `sudo`
- Network Commands:
  - `ifconfig`, `ip a`, `ping`, `netstat`, `ss`, `traceroute`
- Process Monitoring:
  - `ps`, `top`, `htop`, `kill`, `killall`
- File Management:
  - `mv`, `cp`, `rm`, `mkdir`, `rmdir`, `find`, `grep`
- Package Management:
  - `apt`, `apt-get`, `dpkg` (Debian/Ubuntu based systems)

---

## 🪟 Windows CMD & PowerShell Basics

### Windows Command Prompt
- Basic networking commands:
  - `ipconfig`, `ping`, `netstat`, `tracert`, `nslookup`
- File navigation:
  - `cd`, `dir`, `copy`, `del`, `type`, `mkdir`, `rmdir`

### Windows PowerShell
- PowerShell is object-oriented and far more powerful:
  - Get IP: `Get-NetIPAddress`
  - Firewall rules: `Get-NetFirewallRule`
  - Services: `Get-Service`, `Start-Service`, `Stop-Service`
  - Process mgmt: `Get-Process`, `Stop-Process`

---

## 🧪 TryHackMe Rooms Completed

| Room Name           | Status    | Key Topics Covered |
|---------------------|-----------|--------------------|
| Pre-Security        | ✅ Done   | Basic networking, CLI, security concepts |
| Network Fundamentals| ✅ Done   | OSI model, protocols, DNS, DHCP, Firewalls |
| Network Essentials  | ✅ Done   | IP, Subnetting, Ports, TCP/UDP, NAT |
| Linux Basics        | ✅ Done   | CLI usage, user mgmt, permissions |
| Windows Fundamentals| ✅ Done   | CMD, PowerShell, Win internals |
| _Nmap_              | 🚧 To Do | Port scanning and enumeration |

---

📌 _These notes will continue to expand as I complete more TryHackMe modules like Nmap, Metasploit, Burp Suite, and Web Hacking Fundamentals._

