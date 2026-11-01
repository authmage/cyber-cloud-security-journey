
# 🔄 High Availability (HA)

High Availability means connecting two firewalls so that if one firewall fails, the other can take over and maintain network connectivity.

## 🔁 Failover

If the active firewall fails, the passive firewall takes over. This process is called **Failover**.

---

## 🔗 HA Links

### 1️⃣ HA1 – Control Link (Communication & Control)

- Used for communication and coordination between the two firewalls.
- Handles configuration synchronization and control messages.

### 2️⃣ HA2 – Data Link (Session & Data Synchronization)

- Used to synchronize session information and other runtime data between firewalls.

### 3️⃣ HA3 – Packet Forwarding Link

- Used to forward network packets between two firewalls in an Active-Active HA deployment.
- Helps when traffic received by one firewall needs to be processed by its peer.
- Supports packet forwarding in supported deployments and configurations.

---

## 📌 Important Notes

- **HA3 is not required in Active-Passive mode.**
- It is not necessary to have all three physical HA1, HA2, and HA3 ports on a Palo Alto firewall.
- The availability and requirements of these links depend on the HA mode, firewall model, and deployment configuration.
- Virtual HA1, HA2, and HA3 connections can also be configured using virtual interfaces in a Palo Alto VM-Series deployment.
