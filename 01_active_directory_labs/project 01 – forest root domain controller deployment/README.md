# Project 01 – Forest Root Domain Controller Deployment

---

## Project Summary

This project involved deploying a centralized identity management infrastructure to manage users, computers, authentication, and security policies across an enterprise network. A Forest Root Domain Controller was installed and configured using Active Directory Domain Services.

---

## Environment

- **Server OS:** Windows Server 2022  
- **Hypervisor:** VirtualBox  
- **Server Name:** DC-1  
- **Domain Name:** landonhotel.local  
- **Role Deployed:** Active Directory Domain Services (AD DS)

---

## Project Objective

To install and configure Active Directory Domain Services and promote the server to a Forest Root Domain Controller by creating a new domain forest for enterprise identity management.

---

## Deployment Steps

### 1. AD DS Role & DNS Installation

Active Directory Domain Services and DNS roles were successfully installed via Server Manager.

📸 **Screenshot Location:**  
`images/1-AD-role.png`

![Server Manager Dashboard](images/1-AD-role.png)

---

### 2. Network Configuration Verification

Network adapter status was verified to ensure connectivity before and after deployment.

📸 **Screenshot Location:**  
`images/2-network.png`

![Network Status](images/2-network.png)

---

### 3. Domain Controller Promotion & Login

The server was promoted to a Domain Controller and restarted successfully. Domain login was verified.

📸 **Screenshot Location:**  
`images/3-domain_log.png`

![Domain Login](images/3-domain_log.png)

---

## Post-Deployment Validation

---

### Active Directory Structure Verification

Verified domain structure inside **Active Directory Users and Computers**.

📸 **Screenshot Location:**  
`images/4-ADUC.png`

![ADUC Console](images/4-ADUC.png)

---

### DNS Configuration Verification

Forward Lookup Zones confirmed for the domain.

📸 **Screenshot Location:**  
`images/5-DNS_manager.png`

![DNS Manager](images/5-DNS_manager.png)

---

### DNS Zone Records Verification

Validated AD-integrated DNS records.

📸 **Screenshot Location:**  
`images/6-DNS_zone.png`

![DNS Zones](images/6-DNS_zone.png)

---

### SYSVOL & NETLOGON Share Verification

Executed command:

```cmd
net share
```

Verified that **SYSVOL** and **NETLOGON** shares were created successfully after domain controller promotion.

📸 **Screenshot Location:**  
`images/7-netlogon.png`

![SYSVOL Share](images/7-netlogon.png)

---

## Deployment Result

The server was successfully promoted to a Forest Root Domain Controller. Active Directory, DNS, and domain authentication services were fully operational.

---

## Infrastructure Impact

- Centralized authentication enabled  
- User and computer management established  
- Foundation for Group Policy deployment created  
- Enterprise identity infrastructure operational  

---

## Tools & Services Used

- Server Manager  
- Active Directory Domain Services  
- DNS Manager  
- Active Directory Users and Computers  
- Command Prompt  

---

## Project Outcome

Successfully deployed a production-ready Forest Root Domain Controller for the **landonhotel.local** enterprise lab environment.

---

## 📂 Image Folder Structure

```text
Project-01-Forest-Root-Domain-Controller/
│
├── README.md
└── images/
    ├── 1-AD-role.png
    ├── 2-network.png
    ├── 3-domain_log.png
    ├── 4-ADUC.png
    ├── 5-DNS_manager.png
    ├── 6-DNS_zone.png
    └── 7-netlogon.png
```
