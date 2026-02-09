# Project 01 – Forest Root Domain Controller Deployment

## Project Summary
This project involved deploying a centralized identity management infrastructure using Active Directory Domain Services. A Forest Root Domain Controller was installed and configured to manage users, computers, authentication, and enterprise security policies.

---

## Environment

- Operating System: Windows Server 2022  
- Hypervisor: VirtualBox  
- Server Name: DC-1  
- Domain Name: landonhotel.local  
- Role Installed: Active Directory Domain Services (AD DS) + DNS  

---

## Project Objective
To install and configure Active Directory Domain Services and promote the server to a Forest Root Domain Controller by creating a new enterprise domain forest.

---

## Deployment Steps

### AD DS Role Installation
Installed Active Directory Domain Services and DNS roles through Server Manager.

![AD DS Role Installation](images/1-AD-role.png)

---

### Network Configuration Verification
Verified network adapter configuration and connectivity before domain deployment.

![Network Status](images/2-network.png)

---

### Domain Controller Promotion & Login
Promoted the server to a Domain Controller and verified domain authentication login.

![Domain Login](images/3-domain_log.png)

---

## Validation Checks

### Active Directory Structure Verification
Verified domain containers and default objects in Active Directory Users and Computers.

![ADUC Console](images/4-ADUC.png)

---

### DNS Configuration Verification
Confirmed DNS role installation and server service status.

![DNS Manager](images/5-DNS_manager.png)

---

### DNS Zone Records Verification
Validated AD-integrated DNS zone records for domain name resolution.

![DNS Zones](images/6-DNS_zone.png)

---

### SYSVOL & NETLOGON Share Verification
Executed command:

### SYSVOL & NETLOGON Share Verification

Executed command:

```cmd
net share
```

Verified SYSVOL and NETLOGON shares were successfully created.

![SYSVOL NETLOGON Shares](images/7-netlogon.png)


---

## Result
The server was successfully promoted to a Forest Root Domain Controller. Active Directory, DNS, and domain authentication services were fully operational.

---

## Infrastructure Impact

- Centralized authentication enabled  
- User and computer management established  
- Foundation for Group Policy deployment created  
- Enterprise identity infrastructure operational  

---

## Tools Used

- Server Manager  
- Active Directory Domain Services  
- DNS Manager  
- Active Directory Users and Computers  
- Command Prompt  

---

## Project Outcome
Successfully deployed a production-ready Forest Root Domain Controller for the **landonhotel.local** enterprise lab environment.
```

