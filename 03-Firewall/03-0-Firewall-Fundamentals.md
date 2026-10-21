
# 🔥 What is a Firewall?

A **🛡️ Firewall** is a network/security device that monitors incoming and outgoing network traffic and permits or blocks data packets based on a set of security policies.

In other words, it monitors, inspects, filters, and controls traffic based on security policies.

---

## 🎯 Goals of a Firewall (Why Do We Need a Firewall?)

1. 🛡️ **Stop Hackers (Threat Protection):** Prevents hackers, viruses, malware, and denial-of-service (DoS) attacks from reaching private computers or networks.

2. 🔍 **Inspect the Traffic (Traffic Filtering):** Inspects incoming and outgoing data packets and either allows, rejects, or drops them based on security policies.

3. 🔐 **Block Unauthorized Users (Access Control):** Enforces boundaries on who or what can access specific network resources, applications, or ports.

4. 🚫 **Data Exfiltration Prevention:** Monitors outgoing traffic to stop sensitive internal data from leaking or being sent to unauthorized external destinations.

---

## ⚖️ If a Firewall Can Inspect and Forward Data Packets, Why Do We Need a Separate Router? Why Can't We Use Only a Firewall?

- 🛣️ **Router:** *Where should the packet go? (Traffic Director)* — It forwards packets.
- 🛡️ **Firewall:** *Should the traffic be allowed? (Security Guard)* — It analyzes traffic before allowing communication.

A firewall can perform routing functions; however, the primary responsibilities are different. A router mainly forwards data packets between networks and determines the best path to reach the destination. A firewall mainly monitors and filters network traffic based on security rules to allow legitimate traffic and block unauthorized traffic.

In small networks, a single firewall can perform both functions. In large enterprise networks, routers and firewalls are often used separately for better performance, scalability, and security.

So, we use a router for efficient routing and a firewall for security, although one device can perform both roles.

---

## ❓ Follow-Up Questions

### 🔹 Can a Firewall Replace a Router?

Yes, many modern firewalls support routing, but whether they can replace a router depends on the network's requirements and the firewall's capabilities.

### 🔹 Can a Router Provide Security?

Yes. Routers can provide basic security features such as ACLs, packet filtering, and other protections. However, dedicated firewalls generally offer more advanced security inspection features.

### 🔹 Why Do Enterprises Use Both?

They may need high-performance routing, advanced security inspection, network segmentation, scalability, and redundancy.

---

## 📍 Where Do We Place a Firewall?

A firewall is generally placed between two networks to monitor and control traffic based on security policies.

In a typical enterprise network, it is placed between the internet-facing router and the internal LAN.

Firewalls can also be placed between internal network segments, around a DMZ, or installed on individual computers as host-based firewalls.

The placement depends on the organization's security requirements and network design.

> 📝 **Note:** A **DMZ (Demilitarized Zone)** is a specialized subnetwork that sits between an organization's trusted internal network (LAN) and an untrusted external network, such as the internet. It isolates public-facing services (web, email, DNS, FTP servers, etc.) from sensitive internal resources. Firewalls enforce strict rules to monitor and filter traffic moving between the internet, the DMZ, and the internal network. If a hacker compromises a server inside the DMZ, the server remains in the isolated zone, and the hacker cannot easily reach internal databases or employee directories.

---

## 🔍 Why Are ACLs Not Enough?

A basic ACL operates mainly at **Layer 3 and Layer 4** of the OSI model. It filters traffic based on source and destination IP addresses, protocols, and port numbers. It cannot understand or inspect application-level requests at **Layer 7**.

For example, an ACL can allow HTTPS traffic on TCP port 443, but it cannot normally identify the specific website or inspect the HTTP request content. A Layer 7-aware firewall can provide application-level inspection and control, depending on its capabilities and configuration.

- 🔹 **Allow or block HTTPS traffic on port 443** → ACL
- 🔹 **Control which applications can or cannot be accessed** (Facebook, Instagram, YouTube, etc.) → Firewall

---

## 🏭 Different Firewall Vendors

- 🔹 Cisco
- 🔹 Palo Alto Networks
- 🔹 Check Point
- 🔹 Fortinet
