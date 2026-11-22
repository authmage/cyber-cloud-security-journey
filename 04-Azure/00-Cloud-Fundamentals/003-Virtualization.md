
# 💻 Virtualization

Virtualization is a technology that allows us to create multiple virtual computers (Virtual Machines) on a single physical computer using software.

- Increases server resource utilization (usage) and reduces the wastage of RAM and other resources.

In simple words, instead of purchasing multiple physical computers or servers, we can create multiple Virtual Machines (VMs) on one physical machine. Each virtual machine behaves like an independent computer and can run its own operating system and applications.

---

## ❓ Why Do We Need Virtualization?

Before virtualization, organizations faced several problems when managing physical servers.

### 1️⃣ More Physical Hardware

- Organizations needed separate physical computers or servers for different applications.
- Every server required its own hardware.
- Purchasing multiple servers was expensive.

### 2️⃣ High Maintenance Costs

- More electricity consumption.
- More physical space required.
- Hardware maintenance increased costs.

### 3️⃣ Underutilization of Resources

- Some servers used only 10–20% of their CPU and RAM capacity.
- Even though the server had unused resources, organizations couldn't easily use those resources for other applications.

### 4️⃣ Difficult Management

- IT teams had to manage multiple physical servers.
- Installing operating systems, updating software, and troubleshooting hardware took more time.

### 5️⃣ Scalability Issues

- If an organization needed another server, it had to purchase additional hardware.
- Setting up a new physical server took time.

---

## 🖥️ Virtual Machine (VM)

A Virtual Machine is a software-based computer that runs inside a physical computer.

**Each VM has its own:**

- Operating System (Windows/Linux).
- Virtual CPU.
- Virtual RAM.
- Virtual Hard Disk.

Virtual machines are simulated "guest" computers created by the hypervisor.

For example, when running Ubuntu or Kali Linux using VMware Workstation, each virtual machine behaves as if it is running on its own dedicated physical computer, even though it is actually running inside a window on the main operating system.

---

## ⚙️ Hypervisor

A Hypervisor is software that creates and manages virtual machines. It allows multiple virtual machines to share the resources of one physical computer.

**Examples:**
- VMware Workstation
- Oracle VirtualBox
- Microsoft Hyper-V
- VMware ESXi

There are two types of hypervisors:

### 1️⃣ Type 1 – Bare-Metal Hypervisor

- Runs directly on physical hardware.
- Commonly used in data centers.
- **Examples:** VMware ESXi, Microsoft Hyper-V.

### 2️⃣ Type 2 – Hosted Hypervisor

- Runs on top of an existing operating system.
- Commonly used on personal computers.
- **Examples:** VMware Workstation, Oracle VirtualBox.
