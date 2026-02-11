# Ticket-21 — Wrong Default Printer (Print Routing Issue)

## Objective
Diagnose and resolve a printing issue caused by incorrect default printer configuration.

---

## Lab Environment

- Operating System: Windows 10 / Windows 11
- Device Type: Client Workstation (VM)
- Printers Used:
  - Microsoft Print to PDF
  - Microsoft XPS Document Writer
- User Context: Standard Local User

---

## Issue Summary

A user reported that printed documents were not generating expected output due to incorrect printer routing.

---

## Environment Preparation

### 1) Enable Secondary Printer

Enabled Microsoft XPS Document Writer via Windows Features.

**Screenshot:**  
![XPS Enabled](images/01-xps-feature-enabled.png)

---

### 2) Verify Printer Availability

Confirmed both printers were installed.

**Screenshot:**  
![Printers Available](images/02-printers-available.png)

---

### 3) Disable Automatic Default Assignment

Turned off Windows automatic default printer management.

**Screenshot:**  
![Auto Default Disabled](images/03-auto-default-disabled.png)

---

## Issue Simulation

### 4) Set Wrong Default Printer

Configured XPS Writer as default.

**Screenshot:**  
![Wrong Default](images/04-wrong-default-set.png)

---

### 5) Attempt Printing

User printed document which routed to XPS output instead of PDF.

**Screenshot:**  
![Wrong Routing](images/05-print-routed-wrong-printer.png)

---

## Troubleshooting

### 6) Review Default Configuration

Verified incorrect default printer assignment.

**Screenshot:**  
![Default Review](images/06-default-printer-review.png)

---

### 7) Restore Correct Default Printer

Set Microsoft Print to PDF as default.

**Screenshot:**  
![Correct Default](images/07-correct-default-set.png)

---

## Resolution Validation

### 8) Perform Test Print

User successfully printed to correct PDF output.

**Screenshot:**  
![Print Success](images/08-print-success-pdf.png)

---

## Root Cause

Incorrect default printer configuration caused print routing issues.

---

## Resolution

Reconfigured default printer to the appropriate output device.

---

## Outcome

Printing functionality restored successfully.

---

## Key Learning

- Default printer routing troubleshooting
- User configuration validation
- Output path analysis
- Endpoint printer management
