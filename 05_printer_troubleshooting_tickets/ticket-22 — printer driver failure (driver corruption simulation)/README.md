# Ticket-22 — Printer Driver Failure (Driver Removal Simulation)

## Objective
Diagnose and resolve a printing failure caused by removal of the printer device/driver and restore printing functionality.

---

## Lab Environment

- Operating System: Windows 10 / Windows 11
- Device Type: Client Workstation (VM)
- Printer Type: Microsoft Print to PDF
- User Context: Standard Local User
- Admin Context: Local Administrator
- Tools Used:
  - Device Manager
  - Windows Printer Setup
  - Print Test Validation

---

## Issue Summary

A user reported inability to print documents due to missing printer output options on the workstation.

---

## User Impact Validation

### 1) Verify Printer Functionality

Logged in as the standard user and confirmed that the printer was initially installed and operational by performing a successful test print.

**Screenshot:**  
![Printer Working](images/01-printer-working.png)

---

## Issue Simulation

### 2) Review Installed Printer Device

Switched to the Administrator account and opened Device Manager.

Navigated to:

Device Manager → Print queues

Confirmed **Microsoft Print to PDF** was present.

**Screenshot:**  
![Driver Listed](images/02-driver-listed.png)

---

### 3) Remove Printer Device/Driver

Initiated device removal to simulate driver failure.

Right-clicked:

Microsoft Print to PDF → Uninstall device

Captured the uninstall confirmation prompt.

**Screenshot:**  
![Uninstall Confirmation](images/03-uninstall-confirmation.png)

Completed the uninstall process and confirmed the printer device was removed.

**Screenshot:**  
![Driver Removed](images/04-driver-uninstalled.png)

---

## User Impact Validation

### 4) Attempt Printing

Switched back to the standard user account and attempted to print a document.

Observed that the printer was no longer available, preventing print operations.

**Screenshot:**  
![Print Failed](images/05-print-failed-driver-missing.png)

---

## Troubleshooting & Resolution

### 5) Restore Printer Device

Logged in as Administrator and restored the printer using Windows printer setup.

Navigated to:

Settings → Bluetooth & devices → Printers & scanners → Add device

Reinstalled **Microsoft Print to PDF**.

**Screenshot:**  
![Driver Restored](images/06-driver-restored.png)

---

### 6) Verify Printer Restoration

Confirmed the printer reappeared in the device list and returned to operational status.

**Screenshot:**  
![Printer Restored](images/07-printer-restored.png)

---

## Resolution Validation

### 7) Perform Test Print

Returned to the standard user account and performed a test print.

Document printed successfully, confirming issue resolution.

**Screenshot:**  
![Print Success](images/08-print-success.png)

---

## Root Cause

Printer device/driver was removed from the workstation, preventing print operations.

---

## Resolution

Reinstalled the printer device and restored printing services through Windows printer configuration.

---

## Outcome

Printing functionality was successfully restored, and the user was able to resume normal print operations.

---

## Key Learning

- Printer driver/device troubleshooting
- Device removal impact analysis
- Administrative remediation workflow
- Printer restoration procedures
- End-user validation testing
