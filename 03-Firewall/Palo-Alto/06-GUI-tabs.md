
# 🖥️ Palo Alto Firewall GUI Tabs

## 📌 Important – Default Management and Data Interface Services

**By default, which services are enabled on the management interface of the firewall?**

- Ping
- HTTPS
- SSH

**By default, which services are disabled on the management interface?**

- Telnet
- HTTP
- SNMP

**By default, which services are enabled on the data interface?**

- None

---

## 1️⃣ Dashboard – Overall Firewall Status

The Dashboard is the first page where we check the overall health and status of our firewall.

**It displays:**

- Firewall health
- CPU and memory usage
- Interface status
- System information

**Example:**

You want to check whether your firewall is working properly.

---

## 2️⃣ ACC – Application Command Center

ACC provides a graphical view of what is happening inside our network.

**It displays:**

- Applications used by network users.
- Traffic patterns and bandwidth usage.
- Threat activity and suspicious traffic.

**In simple words:**

It helps identify which user is consuming bandwidth or whether suspicious applications are being used.

**Example:**

You want to know how many users are using YouTube.

---

## 3️⃣ Monitor – Logs and Troubleshooting

Used to monitor and view firewall logs, such as:

- Traffic logs
- Threat logs
- URL filtering logs
- System logs
- Configuration logs

Monitor is where we investigate what has already happened in the firewall.

**In simple words:**

If a user cannot access a website, check the traffic logs to find the source IP, destination IP, application, action, and session details.

**Example:**

A user cannot access a website. You can check the traffic logs to find out why.

---

## 4️⃣ Policies – Control Network Traffic

Used to create rules that control network traffic.

Policies define what traffic the firewall should allow, deny, or inspect.

**Types of Policies:**

- **Security Policies** – Allow or deny traffic.
- **NAT Policies** – Translate IP addresses.
- **Decryption Policies** – Control encrypted traffic.
- **QoS Policies** – Manage bandwidth.
- **DoS Protection** – Protect against Denial-of-Service attacks.
- **Application Override** – Define application identification exceptions.

**Example:**

Allow users in the LAN to access the internet using a security policy and source NAT configuration.

You can also create a policy to allow employees to access Google but block Facebook.

---

## 5️⃣ Objects – Reusable Configuration Components

Instead of entering the same IP addresses and settings repeatedly, we create objects and reuse them in policies.

**Types of Objects:**

- **Addresses** – IP addresses.
- **Address Groups** – Collections of IP addresses.
- **Applications** – Application definitions.
- **Services** – Port numbers and protocols.
- **Security Profiles** – Antivirus, anti-spyware, vulnerability protection, etc.

**Example:**

Create an address object for your office network:

`192.168.1.0/24`

---

## 6️⃣ Network – Interfaces and Routing

Used to configure network-related settings.

The Network tab connects the firewall to the network and determines how traffic moves through it.

**It includes:**

- Ethernet interfaces and interface types.
- Security zones.
- Virtual routers and routing tables.
- VLANs.
- Routing.
- DHCP.
- VPN.

**Example:**

Configure Ethernet interfaces and assign them to LAN and WAN zones.

---

## 7️⃣ Device – Firewall-Wide Settings

Used to configure and manage the firewall itself.

The Device tab contains settings that control the firewall itself, rather than individual traffic flows.

**It includes:**

- Management and general setup.
- Administrator accounts and authentication.
- High Availability (HA).
- Licenses.
- Software updates.
- Certificates.
- Dynamic updates.

**Example:**

Create an administrator account or configure HA1 and HA2.

