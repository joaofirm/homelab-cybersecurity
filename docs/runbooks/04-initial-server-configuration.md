# Runbook 04 - Initial Server Configuration

## Objective

Prepare Windows Server before Active Directory deployment.

---

## Rename Server

Open:

Server Manager → Local Server

Change:

Computer Name

New Name:

DC01

Reboot.

---

## Configure Static IP

Network Settings:

IP Address:
192.168.10.10

Subnet Mask:
255.255.255.0

Gateway:
Leave blank

Preferred DNS:
192.168.10.10

---

## Validation

Run:

ipconfig /all

Verify:

Hostname:
DC01

IPv4:
192.168.10.10

DNS:
192.168.10.10

---

## Snapshot

Create Snapshot:

01 - Windows Server Configured

Purpose:

Recovery point before Active Directory installation.
