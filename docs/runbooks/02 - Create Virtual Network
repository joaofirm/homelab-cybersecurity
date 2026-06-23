# Runbook 02 - Create Virtual Network

## Objective

Create an isolated Host-Only network for the homelab environment.

---

## Network Design

Network Name:

VMnet2

Subnet:

192.168.10.0/24

Purpose:

Internal laboratory network for servers and workstations.

---

## Procedure

1. Open VMware Workstation Pro
2. Select:

Edit → Virtual Network Editor

3. Click:

Change Settings

4. Click:

Add Network

5. Select:

VMnet2

6. Configure:

Network Type:
Host-only

Subnet IP:
192.168.10.0

Subnet Mask:
255.255.255.0

7. Disable DHCP

8. Apply changes

---

## Validation

Verify:

VMnet2 exists

Network Type:
Host-only

DHCP:
Disabled

Subnet:
192.168.10.0/24

---

## Notes

This network will be used by:

* Domain Controller
* Windows Workstation
* Linux Systems
* Security Tools

Internet access will be provided later through pfSense.
