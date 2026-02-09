# Ticket-10 — Domain Client Connectivity Failure

## Objective
Diagnose and resolve a domain connectivity issue preventing a client machine from communicating with the Domain Controller.

---

## Lab Environment

- Client OS: Windows 11 (VM)
- Server OS: Windows Server 2022 (DC-1)
- Domain: landonhotel.local
- Network: Host-Only (192.168.56.0/24)
- DC IP: 192.168.56.10
- Tools Used: Command Prompt, DNS, Windows Firewall

---

## Issue Summary

A domain-joined client was unable to communicate with the Domain Controller, causing authentication and resource access failures.

---

## Steps Performed

### 1) Simulated DNS Misconfiguration

Configured the client with an incorrect DNS server.

**Configuration:**

IP Address: 192.168.56.50  
Subnet Mask: 255.255.255.0  
DNS: 8.8.8.8  

**Screenshot:**

![Wrong DNS Config](images/01-client-wrong-dns-config.png)

---

### 2) Tested Domain Connectivity

Executed:

`ping landonhotel.local`  
`nslookup landonhotel.local`

Observed name resolution failure.

**Screenshot:**

![DNS Failure](images/02-domain-name-resolution-failure.png)

---

### 3) Observed Authentication / Access Issues

Attempted domain login and resource access which failed due to connectivity issues.

**Screenshot:**

![Domain Access Failure](images/03-domain-login-connectivity-error.png)

---

## Root Cause

The client system was configured with an external DNS server instead of the Domain Controller, preventing domain name resolution and authentication communication.

---

## Resolution Steps

### 4) Corrected DNS Configuration

Updated DNS settings to point to the Domain Controller.

**Fixed Configuration:**

DNS: 192.168.56.10

**Screenshot:**

![DNS Fixed](images/04-client-dns-fixed.png)

---

### 5) Validated Connectivity Restoration

Executed:

`ping landonhotel.local`  
`nslookup landonhotel.local`

Confirmed successful domain resolution and communication.

**Screenshot:**

![Connectivity Restored](images/05-domain-connectivity-restored.png)

---

## Validation

- Domain name resolved successfully
- Domain Controller reachable
- Authentication restored
- Network communication stable

---

## Outcome

Successfully diagnosed and resolved a domain connectivity failure caused by DNS misconfiguration by correcting the client DNS settings.
