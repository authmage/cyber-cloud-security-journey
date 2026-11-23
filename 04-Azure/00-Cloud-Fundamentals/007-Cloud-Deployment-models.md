
# ☁️ Cloud Deployment Models

A deployment model describes how cloud infrastructure is owned, organized, and made available to users.

## 🔹 Types of Cloud Deployment Models

1. Public Cloud
2. Private Cloud
3. Hybrid Cloud
4. Community Cloud

---

## 1️⃣ Public Cloud

- Resources are owned, operated, and maintained by a third-party provider and delivered over the public internet.
- **Examples:** AWS, Microsoft Azure, Google Cloud.
- Available for use by anyone.
- No upfront CapEx is required to purchase the underlying infrastructure.
- Offers high scalability and can be accessed from anywhere.
- Provides less control over the physical hardware.
- Organizations must follow applicable compliance requirements.

---

## 2️⃣ Private Cloud

- Resources are dedicated to a single organization.
- Can be hosted on-premises or by a third-party provider.
- Provides greater control over the infrastructure.
- CapEx may be required, and scaling can be limited by available resources.
- The organization may be responsible for maintaining the hardware.

---

## 3️⃣ Hybrid Cloud

- A combination of public and private clouds.
- Both environments can be connected using VPN or ExpressRoute (an Azure service).
- Provides the benefits of both public and private clouds.
- More complex to manage.

---

## 4️⃣ Community Cloud

- Shared by several organizations that have common concerns, such as shared security requirements, compliance rules, or missions.
- **Examples:** A group of hospitals, universities, or government departments.
- Managed internally by the member organizations or by a third party.

---

## 🌐 Multi-Cloud

> **📌 Note:** Multi-cloud is not a separate NIST cloud deployment model, but it is an important concept in cloud security.

- Using multiple public cloud providers at the same time (AWS + Azure).
- Reduces vendor lock-in.
- Allows organizations to use the best services offered by each cloud provider.
- More complex to manage.
- May involve higher data transfer costs.
- Different cloud providers use different tools and technologies.

---

# 🎯 Real-Time Examples

### 1️⃣ Private Cloud

*"The company has highly sensitive intellectual property subject to strict national air-gap regulations and wants dedicated hardware."*

👉 **Private Cloud**

---

### 2️⃣ Public Cloud

*"The company wants to expand globally with minimal upfront cost and zero physical infrastructure overhead."*

👉 **Public Cloud**

---

### 3️⃣ Hybrid Cloud

*"The company wants to keep core legacy databases on-premises for compliance, but scale web front-ends during seasonal spikes."*

👉 **Hybrid Cloud** (specifically **Cloud Bursting**)

---

### 4️⃣ Community Cloud

*"Several hospitals want to collaborate and share patient telemetry under strict HIPAA-compliant, isolated infrastructure."*

👉 **Community Cloud**

---

### 5️⃣ Multi-Cloud

*"An enterprise wants to deploy its critical application across both AWS and Azure to reduce vendor lock-in, negotiate better pricing, and ensure business continuity even if an entire cloud provider experiences a global outage."*

👉 **Multi-Cloud**

**🔑 Key Buzzwords:**
- Avoid vendor lock-in.
- Cloud-agnostic.
- Cross-provider redundancy.
- Best-of-breed services.

