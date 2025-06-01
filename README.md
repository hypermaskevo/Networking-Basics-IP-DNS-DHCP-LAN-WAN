# Lesson 1: Networking Basics – IP, DNS, DHCP, LAN, WAN

## 🎯 Goal
Understand the core networking concepts: IP addressing, DHCP, DNS, LAN, WAN.  
Build a simple local network in Cisco Packet Tracer using dynamic IP addressing.

---

## 📘 Theory

### 🔌 IP (Internet Protocol)
An IP address is a unique identifier for a device in a network.  
IPv4 example: `192.168.10.1`  
Types of IP:
- **Static** – Manually assigned.
- **Dynamic** – Automatically assigned via DHCP.

### 🌐 DNS (Domain Name System)
DNS translates domain names (e.g., `google.com`) into IP addresses.

### 🧠 DHCP (Dynamic Host Configuration Protocol)
A protocol that automatically distributes IP addresses, gateways, and DNS to devices.

### 🏠 LAN (Local Area Network)
A high-speed local network with limited coverage, like a home or office.

### 🌍 WAN (Wide Area Network)
A global network connecting broad geographic areas — the Internet.

---

## 🧪 Lab Exercise (see `lab01.pkt`)

### ⚙️ Topology
- 1x Router
- 1x Switch
- 1x DHCP Server
- 2x PCs

### 🛠️ Configuration
#### DHCP Server:
- IP Address: `192.168.10.2`
- DHCP Pool: `192.168.10.100 – 192.168.10.150`
- Subnet Mask: `255.255.255.0`
- Gateway: `192.168.10.1`
- DNS Server: `8.8.8.8`

#### Router:
- FastEthernet0/0: `192.168.10.1 /24`

#### PCs:
- Set to receive IP automatically (DHCP)

---

## ✅ Test Your Setup
1. Run the simulation.
2. On each PC, open the terminal → run `ipconfig` → verify IP address.
3. Ping between PC1 and PC2 → `ping 192.168.10.X`

---

## 📂 Folder Structure
