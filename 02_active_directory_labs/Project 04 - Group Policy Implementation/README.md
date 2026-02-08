# Project 04 – Group Policy Implementation

## Project Summary
Implemented centralized security and administrative policies using Group Policy Objects (GPOs) within an Active Directory domain environment.

---

## Environment
- Windows Server 2022
- Domain: landonhotel.local
- Domain Controller: DC-1
- Tool: Group Policy Management Console (GPMC)

---

## Objective
To enforce password security, account lockout protection, and user environment restrictions through centralized policy management.

---

## Policies Implemented

### 1) Password Complexity Policy
Enabled password complexity requirements to enforce strong authentication standards.

![Password Policy](images/3-password-policy.png)

---

### 2) Account Lockout Policy
Configured account lockout after 3 failed login attempts to mitigate brute-force attacks.

![Lockout Policy](images/4-lockout-policy.png)

---

### 3) Control Panel Restriction
Restricted user access to Control Panel and system settings to prevent unauthorized configuration changes.

![Control Panel Disabled](images/5-control-panel-disabled.png)

---

## GPO Linking
Linked the **Security-Baseline-GPO** to the IT Organizational Unit to apply policies to departmental users.

![GPO Linked](images/6-gpo-linked.png)

---

## Policy Update
Forced Group Policy refresh using command line.

![GPUpdate](images/7-gpupdate.png)

---

## Policy Enforcement Testing

### Control Panel Restriction Test
Users were blocked from accessing restricted system settings.

![Restriction Test](images/8-policy-test.png)
---

## Result
Successfully deployed and validated enterprise security baseline policies across domain users.

---

## Skills Demonstrated
- Group Policy Object (GPO) creation
- Security baseline implementation
- Account lockout configuration
- Password policy enforcement
- Administrative template configuration
- OU-level policy linking
- Endpoint access restriction
