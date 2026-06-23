# Runbook 03 - Install Windows Server 2022

## Objective

Deploy the first Windows Server 2022 virtual machine.

---

## VM Specifications

Name:

DC01

CPU:
2 vCPU

Memory:
4 GB

Disk:
80 GB Thin Provision

Network:
VMnet2

---

## Procedure

### Create Virtual Machine

1. Create New Virtual Machine
2. Select:

Custom (Advanced)

3. Choose:

I will install the operating system later

Important:

Do NOT use Easy Install.

---

### Configure Hardware

Memory:
4096 MB

Processors:
2

Disk:
80 GB

Network:
VMnet2

---

### Install Operating System

1. Mount Windows Server 2022 ISO
2. Boot VM
3. Select:

Windows Server 2022 Standard Evaluation (Desktop Experience)

4. Select:

Custom Installation

5. Install to Disk 0

---

## Validation

Confirm successful login to Windows Server desktop.

---

## Known Issue

Error:

"Windows cannot find the Microsoft Software License Terms"

Resolution:

Disable VMware Easy Install and perform manual installation.
