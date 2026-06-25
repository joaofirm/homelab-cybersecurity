# Runbook 08 - Join Windows 11 to Active Directory Domain

## Objective

Join a Windows 11 workstation to the SitexNow Active Directory environment.

---

## Prerequisites

Domain Controller operational:

* DC01
* 192.168.10.10

Domain:

* sitexnow.local

DNS configured:

* 192.168.10.10

---

## Configure Network Settings

Open:

ncpa.cpl

Navigate:

Ethernet
→ Properties
→ IPv4

Configure:

IP Address:
192.168.10.20

Subnet Mask:
255.255.255.0

DNS Server:
192.168.10.10

---

## Validate Connectivity

Execute:

ping 192.168.10.10

Expected:

Reply from 192.168.10.10

Execute:

nslookup sitexnow.local

Expected:

Successful domain resolution

---

## Join Domain

Open:

sysdm.cpl

Navigate:

Computer Name
→ Change

Select:

Domain

Enter:

sitexnow.local

---

## Authenticate

Use:

SITEXNOW\Administrator

Password:

<Defined During Deployment>

---

## Confirmation

Expected message:

Welcome to the sitexnow.local domain

---

## Restart Workstation

Reboot the workstation.

---

## Test Domain Login

Log in using:

SITEXNOW\joao.user

Expected result:

Successful domain authentication.

---

## Validation

Verify that the computer object exists in Active Directory.

Path:

Active Directory Users and Computers

Expected object:

CL01

---

## Notes

Domain Join requires:

* DNS connectivity
* Reachability to Domain Controller
* Valid administrative credentials
