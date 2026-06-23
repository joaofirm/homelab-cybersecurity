# Runbook 01 - Install VMware Workstation Pro

## Objective

Install VMware Workstation Pro on Windows to serve as the virtualization platform for the cybersecurity homelab.

---

## Requirements

### Hardware

* CPU with Intel VT-x or AMD-V support
* Minimum 16 GB RAM
* Recommended 32 GB RAM or more
* SSD storage
* Windows 10 or Windows 11

### Software

* VMware Workstation Pro

---

## Verify Virtualization Support

Open Task Manager:

Performance → CPU

Confirm:

Virtualization: Enabled

If disabled:

1. Reboot the computer
2. Enter BIOS/UEFI
3. Enable:

   * Intel VT-x
   * Intel VT-d (optional)
   * AMD-V
   * SVM Mode

Save and reboot.

---

## Installation Procedure

1. Execute VMware Workstation Pro installer
2. Accept license agreement
3. Keep default installation path
4. Install enhanced keyboard driver
5. Complete installation
6. Reboot the computer if requested

---

## Validation

Open VMware Workstation Pro.

Confirm:

* VMware launches successfully
* Virtual Machine Library is displayed
* Virtual Network Editor is available

---

## Notes

This homelab uses VMware Workstation Pro as the primary hypervisor.

Snapshots should be created before major infrastructure changes.
