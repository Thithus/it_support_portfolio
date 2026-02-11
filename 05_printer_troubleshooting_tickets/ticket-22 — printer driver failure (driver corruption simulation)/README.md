# Ticket-22 — Printer Driver Failure (Driver Removal Simulation)

## Objective
Diagnose and resolve a printing failure caused by removal of the printer driver/device.

---

## Lab Environment

- Operating System: Windows 10 / Windows 11
- Device Type: Client Workstation (VM)
- Printer Type: Microsoft Print to PDF
- User Context: Standard Local User
- Admin Context: Local Administrator

---

## Issue Summary

A user reported inability to print documents due to missing printer output options.

---

## User Impact Validation

### 1) Verify Printer Functionality

Confirmed printer was installed and operational by performing a successful test print.

**Screenshot:**  
![Printer Working](images/01-printer-working.png)

---

## Issue Simulation

### 2) Review Installed Printer Device

Accessed Device Manager → Print queues and confirmed the printer was present.

**Screenshot:**  
![Driver Listed](images/02-driver-listed.png)

---

### 3) Remove Printer Device/Driver

Uninstalled Microsoft Print to PDF via Device Manager.

**Screenshot:**  
![Uninstall Confirmation](images/03-uninstall-confirmation.png)

**Screenshot:**  
![Driver Removed](images/04-driver-uninstalled.png)

---

### 4) Attempt Printing

User attempted to print but no printer output device was available.

**Screenshot:**  
![Print Failed](images/05-print-failed-driver-missing.png)

---

## Troubleshooting

### 5) Restore Printer Device

Reinstalled Microsoft Print to PDF via Windows printer setup.

**Screenshot:**  
![Driver Restored](images/06-driver-restored.png)

---

### 6) Verify Printer Restoration

Confirmed printer returned to operational state.

**Screenshot:**  
![Printer Restored](images/07-printer-restored.png)

---

## Resolution Validation

### 7) Perform Test Print

User successfully printed after restoration.

**Screenshot:**  
![Print Success](images/08-print-success.png)

---

## Root Cause

Printer driver/device was removed, preventing print operations.

---

## Resolution

Reinstalled printer device and restored printing services.

---

## Outcome

Printing functionality restored successfully.

---

## Key Learning

- Printer driver troubleshooting  
- Device removal impact analysis  
- Printer restoration workflow  
- Endpoint print service recovery
