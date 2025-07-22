# 🧠 Networking Basics – TryHackMe Notes  
*From Pre-Security & Network Fundamentals rooms up to "Network Essentials"*

---

## 🌐 The OSI Model (7 Layers)
- **Application** – Interfaces with the user (e.g., HTTP, DNS)
- **Presentation** – Data formatting & encryption (e.g., SSL/TLS)
- **Session** – Manages connections/sessions
- **Transport** – Ensures data delivery (TCP/UDP)
- **Network** – IP addressing and routing (IP)
- **Data Link** – MAC addresses, switches
- **Physical** – Hardware like cables, NICs

---

## 🛰️ TCP vs UDP
- **TCP**:
  - Connection-oriented
  - Reliable (data delivery, error checking)
  - Slower but secure (used in HTTPS, SSH)
- **UDP**:
  - Connectionless
  - Fast but no guarantee of delivery (used in DNS, streaming)

---

## 🏷️ IP Addressing
- **IPv4**: 32-bit addresses (e.g., 192.168.0.1)
- **IPv6**: 128-bit, newer protocol (e.g., `fe80::1`)
- **Public vs Private IPs**:
  - Private: Used internally (e.g., 192.168.x.x, 10.x.x.x)
  - Public: Routable over the internet

---

## 🧭 DNS (Domain Name System)
- Converts domain names to IP addresses
- Works over **port 53**
- Example: `www.google.com` ➜ `142.250.64.78`

---

## 🌍 HTTP vs HTTPS
- **HTTP**:
  - Port 80
  - Plaintext communication
- **HTTPS**:
  - Port 443
  - Encrypted using SSL/TLS

---

## 🔐 Common Protocols and Their Ports
| Protocol | Port | Use |
|---------|------|-----|
| HTTP | 80 | Web (unencrypted) |
| HTTPS | 443 | Web (encrypted) |
| FTP | 21 | File Transfer |
| SSH | 22 | Secure Remote Access |
| DNS | 53 | Domain Resolution |
| SMTP | 25 | Sending Email |
| POP3 | 110 | Receiving Email |
| IMAP | 143 | Receiving Email |

---

## 🧩 MAC Address vs IP Address
- **MAC Address**:
  - Hardware-based, unique to device (e.g., `00:1A:2B:3C:4D:5E`)
  - Works at Data Link layer
- **IP Address**:
  - Logical address used for routing
  - Can change dynamically

---

## 📡 DHCP (Dynamic Host Configuration Protocol)
- Automatically assigns IP addresses to devices on a network
- Reduces manual IP configuration
- Works with:
  - **IP address**
  - **Subnet mask**
  - **Gateway**
  - **DNS servers**

---

## 🧱 Firewalls & NAT
- **Firewall**:
  - Controls incoming/outgoing traffic using rules
  - Can block specific IPs, ports, or protocols
- **NAT (Network Address Translation)**:
  - Converts private IPs to public IPs (and vice versa)
  - Helps conserve public IPv4 addresses

---

## 🧮 Subnetting Basics (Very High-Level)
- Divides networks into smaller parts
- Helps improve routing and security
- Example: `192.168.1.0/24` → 256 IPs total

---

📌 *These are my consolidated notes based on all TryHackMe rooms I completed up to the “Network Essentials” room. All summaries are handwritten in detail and available in the [`Notes/Handwritten`](./Handwritten) folder.*
