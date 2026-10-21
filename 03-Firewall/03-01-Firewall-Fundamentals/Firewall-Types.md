
# 🔥 Types of Firewalls

Firewalls can be classified in different ways.

### 📌 Classification of Firewalls

- 🖥️ **Based on Deployment:** Host-Based Firewall, Network-Based Firewall.
- ⚙️ **Based on Implementation:** Hardware Firewall, Software Firewall, Cloud Firewall (FWaaS – Firewall as a Service).
- 🔍 **Based on Traffic Inspection:** Stateless Firewall (Packet Filtering), Stateful Firewall, Circuit-Level Gateway, Proxy Firewall, Next-Generation Firewall (NGFW).
- 🎯 **Based on Purpose:** Web Application Firewall (WAF), Cloud Firewall.

> 📝 **Note:** These firewall types can overlap. For example, an NGFW can be hardware-based or software-based, and a cloud firewall may be delivered as FWaaS.

---

## 🖥️ 1. Host-Based Firewall

- Installed on an individual computer or server.
- **Example:** Windows Defender Firewall protects a laptop by controlling incoming and outgoing connections.

## 🌐 2. Network-Based Firewall

- Protects traffic flowing between networks or network segments.
- **Example:** A company firewall controls traffic between the internet and the office network.

---

## ⚙️ 3. Hardware Firewall

- Runs on a dedicated physical appliance.

## 💻 4. Software Firewall

- Runs as software on general-purpose hardware or a virtual machine.

---

## 🔍 5. Stateless Firewall (Packet-Filtering Firewall)

- Makes a decision on each packet individually and does not maintain a session table.
- Looks only at source and destination IP addresses, protocols, and port numbers.
- Does not know whether a packet belongs to an existing connection.

**Example:** A company allows traffic to its web server on port 443 (HTTPS) and blocks traffic on port 23 (Telnet). It checks each packet against its rules without remembering previous packets.

---

## 🔐 6. Stateful Firewall (Tracks Active Connections)

- Remembers active connections and checks whether packets belong to permitted connections.

**Example:**

1. PC1 sends a SYN packet to the server.
2. The firewall records the connection.
3. The server replies.
4. The firewall checks whether the packet is part of an existing connection.
5. If yes, it allows the packet.
6. If no, it drops the packet.

These firewalls track sessions and drop packets that do not match the expected connection state.

> 📝 **SYN Packet:** A SYN packet (short for *synchronize*) is the first network packet sent by a client to request and start a TCP connection. It acts as a digital "door knock," telling a server that the client wants to open a communication session.

> 📝 **Session Table:** A firewall session table is a database that tracks active network connections in a stateful firewall.

**Example:** We open Google on the laptop. The firewall remembers the connection and allows the website's response traffic because it belongs to our established connection.

---

## 🚀 7. Next-Generation Firewall (NGFW)

**Advanced Traffic and Application Security**

It combines traditional firewall filtering with advanced security capabilities, such as application identification, intrusion prevention, and deeper traffic inspection.

### 🛡️ NGFW Security Features

- 🔹 **SandBlast: Threat Extraction** — Removes potentially dangerous content and provides a safer version.
- 🔹 **SandBlast: Threat Emulation** — Tests a suspicious file to see if it behaves like malware.
- 🔹 **URL Filtering**
- 🔹 **Anti-Bot**
- 🔹 **Antivirus**
- 🔹 **Anti-Spam**
- 🔹 **IPS (Intrusion Prevention System)** — Monitors and detects suspicious or malicious activity and automatically blocks and prevents threats.
- 🔹 **Identity Awareness**
- 🔹 **VPN**
- 🔹 **Firewall**
- 🔹 **App Control**
- 🔹 **DLP (Data Loss Prevention)**

**Example:** A company configures an application-aware firewall to allow YouTube but block Facebook, depending on the firewall's capabilities and configuration.

---

## 🔄 8. Circuit-Level Gateway

- Checks whether a connection is established according to its rules.
- It does not inspect the full application data.

**Example:** It checks the TCP connection before allowing the session to proceed.

---

## 🔁 9. Proxy Firewall

- Acts as an intermediary between a client and a destination server.
- It can inspect application-level traffic and helps control how clients access particular servers.

**Example:** A company uses a proxy to control employee web access and block requests to restricted websites.

---

## 🌍 10. Web Application Firewall (WAF)

- Protects web applications by inspecting HTTP/HTTPS requests and blocking malicious web traffic.

**Example:** An online shopping website uses a WAF to detect and block malicious requests targeting login or payment pages.

---

## ☁️ 11. Firewall as a Service (FWaaS)

- It is a cloud-delivered firewall service.
- Instead of managing all firewall functionality through a physical appliance at each location, an organization can use a provider's cloud-based firewall service.

**Example:** A company uses a cloud firewall service to apply security policies to employees working at different office locations or remotely.

---

## ☁️ 12. Cloud Firewall

- Filters network traffic to protect cloud-based resources, such as virtual machines, networks, and applications.

**Example:** An organization configures firewall rules to allow HTTPS access to a cloud-hosted website while restricting direct access to its internal servers.
