# Ticket-20 — Printer Unavailable (Feature Disabled Simulation)

## Objective
Diagnose and resolve a printing failure caused by printer driver/feature unavailability.

---

## Lab Environment

- Operating System: Windows 10 / Windows 11
- Device Type: Client Workstation (VM)
- Printer Type: Microsoft Print to PDF
- User Context: Standard Local User
- Admin Context: Local Administrator

---

## Issue Summary

A user reported inability to print documents due to the printer appearing unavailable.

---

## User Impact Validation

### 1) Verify Printer Availability

Navigated to:

Settings → Bluetooth & devices → Printers & scanners

Confirmed Microsoft Print to PDF was installed and operational.

**Screenshot:**  
![Printer Online](images/01-printer-online.png)

---

### 2) Simulate Printer Unavailability

Disabled Microsoft Print to PDF via Windows Features.

**Screenshot:**  
![Feature Disabled](images/02-feature-disabled.png)

---

### 3) Confirm Printer Missing

Verified printer was no longer available.

**Screenshot:**  
![Printer Missing](images/03-printer-missing.png)

---

### 4) Attempt Printing

User attempted to print but no PDF printer was available.

**Screenshot:**  
![Print Failed](images/04-print-failed-missing.png)

---

## Administrative Troubleshooting

### 5) Re-Enable Printer Feature

Re-enabled Microsoft Print to PDF via Windows Features.

**Screenshot:**  
![Feature Enabled](images/05-feature-enabled.png)

---

### 6) Verify Printer Restoration

Confirmed printer returned to operational state.

**Screenshot:**  
![Printer Restored](images/06-printer-restored.png)

---

## Resolution Validation

### 7) Perform Test Print

User successfully printed after restoration.

**Screenshot:**  
![Print Success](images/07-print-success.png)

---

## Root Cause

Printer driver/feature was unavailable due to feature being disabled.

---

## Resolution

Re-enabled Microsoft Print to PDF feature and restored printing services.

---

## Outcome

Printing functionality restored successfully.

---

## Key Learning

- Printer driver/feature troubleshooting
- Windows Features dependency
- Endpoint printer restoration
- Print service validation
