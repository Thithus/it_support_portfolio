# 🧭 Active Directory Homelab Portfolio

Welcome to my Active Directory hands-on lab portfolio.

This repository section showcases practical implementation of core Active Directory administration, identity management, and enterprise security policy deployment using a Windows Server environment.

All labs were performed in a virtualized homelab to simulate real-world enterprise infrastructure scenarios.

---

# 🛠️ Lab Environment

* **Server OS:** Windows Server 2022
* **Client OS:** Windows 10 / 11
* **Directory Service:** Active Directory Domain Services (AD DS)
* **Domain Name:** landonhotel.local
* **Tools Used:**

  * Server Manager
  * Active Directory Users & Computers
  * Group Policy Management Console (GPMC)
  * DNS Manager

---

# 🎯 Portfolio Objectives

The goal of these labs was to build job-ready, practical skills in:

* Domain infrastructure deployment
* Identity and access management
* Organizational Unit design
* Security baseline enforcement
* Group Policy administration
* Enterprise user environment control

---

# 📂 Lab Projects

## 🔧 01 — Forest Root Domain Controller Deployment

Deployed the first Domain Controller by installing AD DS and promoting the server to create a new forest.

**Key Skills:**

* AD DS installation
* Forest creation
* DNS configuration
* Domain admin login validation

📄 Project File:
`01-Forest-Root-Domain-Controller.md`

---

## 👥 02 — User & Group Management

Created departmental users and security groups and implemented group-based administrative structure.

**Key Skills:**

* User provisioning
* Security group creation
* Group membership assignment
* Departmental identity organization

📄 Project File:
`02-User-Group-Management.md`

---

## 🏢 03 — Organizational Unit (OU) Structure Design

Designed and implemented enterprise-style OU hierarchy and delegated user placement.

**OU Structure:**

```
landonhotel.local
 ├── IT
 ├── HR
 ├── Finance
 └── Sales
```

**Key Skills:**

* OU creation
* Directory structuring
* Administrative segmentation

📄 Project File:
`03-OU-Structure-Design.md`

---

## 🔐 04 — Group Policy Implementation

Implemented centralized administrative and security policies across domain users.

**Policies Deployed:**

* Password Complexity Enforcement
* Account Lockout Protection
* Control Panel Restrictions
* OU-linked policy deployment

**Key Skills:**

* GPO creation
* Security baseline configuration
* Administrative template control
* Policy testing & enforcement

📄 Project File:
`04-Group-Policy-Implementation.md`

---

# 🧪 Testing & Validation

All policies and configurations were tested using domain client machines to verify:

* Authentication enforcement
* Account lockout behavior
* Endpoint restrictions
* Policy propagation

Screenshots and command outputs are included in each project.

---

# 📊 Skills Demonstrated

* Active Directory Deployment
* Identity & Access Management (IAM)
* Security Group Administration
* Organizational Unit Design
* Group Policy Management
* Endpoint Security Enforcement
* Windows Server Administration

---

# 🚀 Portfolio Value

These labs reflect real-world enterprise administration tasks performed by:

* IT Support Engineers
* System Administrators
* Windows Server Administrators
* SOC / Blue Team Analysts

---

# 📌 Author

**Thithushan**
IT Support / Cybersecurity Portfolio Builder

GitHub Portfolio:
[https://github.com/Thithus/it_support_portfolio](https://github.com/Thithus/it_support_portfolio)

---

⭐ More labs in Networking & Troubleshooting coming soon.
