# Ticket-15 — Mailbox Provisioning Issue

## Objective
Diagnose and resolve a mailbox provisioning issue caused by disabled Exchange Online service within a licensed Microsoft 365 user account.

---

## Lab Environment

- Platform: Microsoft 365 Admin Center
- Tenant Type: Microsoft 365 E5 Trial
- Admin Portal: https://admin.microsoft.com

---

## Issue Summary

A user reported being unable to access their mailbox via Outlook and Outlook Web Access despite having a valid Microsoft 365 license assigned.

---

## Steps Performed

### 1) Review License Service Assignment

Verified Exchange Online service was enabled under the assigned license prior to issue simulation.

**Screenshot:**

![Exchange Enabled](images/01-exchange-enabled-before.png)

---

### 2) Simulate Mailbox Service Failure

Disabled Exchange Online service to reproduce the reported mailbox access issue.

**Screenshot:**

![Exchange Disabled](images/02-exchange-service-disabled.png)

---

### 2a) Observe Service Dependency Warning

While disabling Exchange Online, the system generated a dependency warning indicating that related services such as Microsoft Defender for Office 365 require Exchange Online to remain enabled.

**Screenshot:**

![Dependency Warning](images/02a-exchange-dependency-warning.png)

---

### 3) Verify Mailbox Service Impact

Accessed the Mail configuration tab to review mailbox provisioning state following Exchange Online service disablement.

**Screenshot:**

![Mailbox Impact](images/03-mailbox-service-impact.png)

---

### 4) Restore Exchange Online Service

Re-enabled Exchange Online service under license configuration to restore mailbox functionality.

**Screenshot:**

![Exchange Reenabled](images/04-exchange-service-reenabled.png)

---

### 5) Validate Mailbox Restoration

Confirmed mailbox provisioning and access were restored successfully.

**Screenshot:**

![Mailbox Restored](images/05-mailbox-access-restored.png)

---

## Validation

- Exchange Online service dependency verified
- Mailbox service disruption reproduced
- Dependency warning observed
- Service restored successfully
- Mailbox provisioning validated

---

## Outcome

Mailbox access was restored by re-enabling Exchange Online service within the assigned Microsoft 365 license configuration, resolving the user’s email access issue.
