
# ☁️ Cloud Service Models

Cloud service models explain what type of service the cloud provider offers and what responsibilities remain with the customer.

## 🔹 Three Important Cloud Service Models

1. **IaaS** – Infrastructure as a Service
2. **PaaS** – Platform as a Service
3. **SaaS** – Software as a Service

---

## 1️⃣ IaaS – Infrastructure as a Service

*Analogy: Renting an empty plot of land with utilities.*

- Renting virtual hardware, virtual servers, Virtual Machines (VMs), storage, and networks.
- The customer manages the OS, middleware, runtime, applications, data, etc.
- The provider secures the physical hardware and hypervisor.
- The customer secures the OS, network configuration, firewall rules, and data.

**Examples:**
- Amazon EC2
- Microsoft Azure Virtual Machines
- Google Compute Engine

### 🔐 Security Angle

You manage almost everything, including:

- Installing the operating system (Windows or Linux).
- Applying security patches.
- Setting up firewalls.
- Protecting your data.

You have the most control, which means you also have the most security responsibilities.

**Example:** If a server gets hacked because you forgot to update Linux, that responsibility falls on you.

---

## 2️⃣ PaaS – Platform as a Service

*Analogy: Renting a furnished apartment.*

- We upload our code, and the cloud provider handles the underlying infrastructure.
- The cloud provider manages the underlying servers, storage, and operating systems.
- You get a ready-to-use environment to build, test, and run your own applications.
- The provider secures the hardware, OS, and runtime.
- You secure the application code and data.

**Examples:**
- Heroku
- Google App Engine
- AWS Elastic Beanstalk

### 🔐 Security Angle

The provider secures the servers and operating system.

You only manage your application code and data.

- You do not need to worry about updating operating systems or managing hardware.
- Your security responsibilities focus on user access and ensuring that the code you write does not have security flaws.

---

## 3️⃣ SaaS – Software as a Service

*Analogy: Staying in a hotel.*

- You use a complete, ready-made software application over the internet, usually through a web browser.
- You do not build or maintain anything behind the scenes.

**Examples:**
- Microsoft 365
- Gmail
- Salesforce
- Zoom
- Slack
- GitHub

### 🔐 Security Angle

The provider secures almost everything.

You manage:

- User accounts.
- Passwords.
- Application settings.
- The data you put into the application.

Your security focus is **Identity and Access Management (IAM)**.

For example:
- Ensure employees use Multi-Factor Authentication (MFA).
- Prevent employees from sharing passwords.
- Ensure sensitive files are not accidentally made public.

---

# 🔐 Shared Responsibility Model

The **Shared Responsibility Model** is a security framework that defines which security tasks are handled by the cloud provider (such as Microsoft Azure or AWS) and which tasks are handled by you (the customer).

- Responsibilities change depending on the cloud service model.
- **Customer:** Responsible for data, access management, and the components they control.
- **Cloud Provider:** Responsible for physical infrastructure, physical network security, and hypervisors.
- The customer will always be responsible for data and access management.

## 📊 Shared Responsibility – On-Premises vs. Cloud

| Layer | On-Premises (Your Own Office) | IaaS (Azure VMs) | PaaS (Azure App Service) | SaaS (Microsoft 365) |
|---|---|---|---|---|
| Data & Classification | You | You | You | You |
| Devices / Endpoints | You | You | You | You |
| Accounts & Identities | You | You | You | You |
| Application Code | You | You | You | Provider |
| Network Controls | You | You | Shared | Provider |
| Operating System | You | You | Provider | Provider |
| Physical Hosts & Network | You | Provider | Provider | Provider |
| Physical Data Center | You | Provider | Provider | Provider |

---

## 📌 Key Takeaway

- **IaaS:** You manage the operating system and everything above it.
- **PaaS:** You manage your application and data.
- **SaaS:** You use the ready-made application and manage your users, access, and data.
