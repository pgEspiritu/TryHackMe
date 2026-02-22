# 🖧 Local Area Network (LAN) Topologies & Core Networking Concepts

Networking designs have evolved over time. In networking, **topology** refers to the **layout or structure** of how devices are connected. Each topology has strengths and weaknesses that affect **cost, performance, reliability, and security**.

---

## ⭐ Star Topology

::contentReference[oaicite:0]{index=0}


### 📌 Overview
- Each device connects to a **central device** (switch or hub).
- **Most common topology today** due to reliability and scalability.

### ✅ Advantages
- 🔧 **Scalable** – easy to add/remove devices  
- 🧪 **Fault isolation** – one device failure doesn’t affect others  
- 📈 **Good performance** with switches

### ❌ Disadvantages
- 💸 **Higher cost** (more cabling + central hardware)
- 🛠️ **Maintenance increases** as the network grows
- ⚠️ **Single point of failure** – if the central device fails, the network goes down

---

## 🚌 Bus Topology

::contentReference[oaicite:1]{index=1}


### 📌 Overview
- All devices share a **single backbone cable**.
- Devices branch off like **leaves from a tree**.

### ✅ Advantages
- 💰 **Low cost**
- 🧵 **Minimal cabling**
- ⚡ **Simple to set up**

### ❌ Disadvantages
- 🐌 **Performance bottlenecks** under heavy traffic
- 🧩 **Hard to troubleshoot**
- ❌ **No redundancy** – backbone failure breaks the entire network

---

## 🔁 Ring Topology (Token Topology)

::contentReference[oaicite:2]{index=2}


### 📌 Overview
- Devices form a **closed loop**
- Data travels in **one direction** around the ring

### ✅ Advantages
- 🔍 **Easier troubleshooting**
- 🚦 **Less congestion** than bus topology
- 🧵 **Less cabling** than star topology

### ❌ Disadvantages
- 🐢 **Inefficient routing** (data may pass many devices)
- 💥 **Single failure** (device or cable) breaks the entire network

---

## 🔀 What Is a Switch?

::contentReference[oaicite:3]{index=3}


### 📌 Overview
- A **switch** connects multiple devices using Ethernet
- Common in **schools, offices, and enterprises**
- Available in **4, 8, 16, 24, 32, 64 ports**

### 🔥 Why Switches Are Efficient
- 🧠 Knows which device is on which port
- 📤 Sends data **only to the intended device**
- 🚫 Reduces unnecessary network traffic (unlike hubs)

---

## 🌐 What Is a Router?

::contentReference[oaicite:4]{index=4}


### 📌 Overview
- A **router connects networks** together
- Moves data using a process called **routing**

### 🔁 Routing Explained
- Determines the **best path** for data across networks
- Increases **redundancy and reliability**
- 📉 Slight performance cost, but 🟢 **no downtime**

---

## 🧪 Practical: Breaking LAN Topologies
- Interactive labs demonstrate how **different topologies fail**
- Goal: **exploit weaknesses** to retrieve a flag
- Reinforces real-world **availability and resilience risks**

---

## 🍰 Subnetting Explained
Subnetting is the process of **splitting a large network into smaller networks**.

📌 Think of it like **slicing a cake** — deciding who gets which piece.

### 🏢 Why Businesses Use Subnetting
Departments like:
- Accounting
- Finance
- Human Resources

…need **separation and control**, just like real-world workflows.

---

## 🧮 IP Addressing & Subnet Masks
- IP addresses and subnet masks both have **4 octets (32 bits)**
- Values range from **0–255**

### Subnets Use IP Addresses to:
1. Identify the **Network Address**
2. Identify the **Host Address**
3. Identify the **Default Gateway**

### 📋 Address Types Summary
| Type | Purpose | Example |
|---|---|---|
| **Network Address** | Identifies the network | `192.168.1.0` |
| **Host Address** | Identifies a device | `192.168.1.100` |
| **Default Gateway** | Sends traffic to other networks | `192.168.1.254` |

🏠 **Home networks** usually need one subnet  
🏢 **Businesses** require multiple subnets

---

## 🔐 Why Subnetting Matters (Security)
Subnetting provides:
- ⚡ **Efficiency**
- 🔐 **Security**
- 🎛️ **Control**

### ☕ Café Example
- 🔒 Staff network (POS, printers)
- 🌍 Public Wi-Fi network

➡️ Subnetting **keeps them separated** while sharing Internet access.

---

## 🔁 ARP (Address Resolution Protocol)

::contentReference[oaicite:5]{index=5}


### 📌 What Is ARP?
ARP maps:
- **IP Address → MAC Address**

Devices must know the **MAC address** to communicate on a local network.

### 🧠 How ARP Works
- Devices keep a table called an **ARP cache**
- Uses two messages:
  - 📢 **ARP Request** – “Who owns this IP?”
  - 📩 **ARP Reply** – “That IP is mine; here’s my MAC”

---

## 📡 DHCP (Dynamic Host Configuration Protocol)

::contentReference[oaicite:6]{index=6}


### 📌 What DHCP Does
Automatically assigns IP addresses to devices.

### 🔄 DHCP Process (DORA)
1. **Discover** – device looks for DHCP server  
2. **Offer** – server offers an IP address  
3. **Request** – device accepts the offer  
4. **ACK** – server confirms assignment  

➡️ Device can now communicate on the network.

---

## ✅ Key Takeaways
- 🖧 LAN topologies affect **performance and reliability**
- 🔀 Switches reduce traffic; 🌐 routers connect networks
- 🍰 Subnetting improves **security and control**
- 🔁 ARP links **IP ↔ MAC**
- 📡 DHCP automates IP assignment

🚀 **Understanding these concepts is foundational for networking and cybersecurity.**
