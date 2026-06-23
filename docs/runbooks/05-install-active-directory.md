# Runbook 05 - Install Active Directory

## Objective

Deploy Active Directory Domain Services and create the SitexNow domain.

---

## Install Role

Open:

Server Manager

Add Roles and Features

Select:

Active Directory Domain Services

Install.

---

## Promote Domain Controller

Open Notification Center.

Select:

Promote this server to a domain controller

---

## Deployment Configuration

Select:

Add a new forest

Root Domain:

sitexnow.local

---

## Domain Controller Options

Enable:

✓ DNS Server

✓ Global Catalog

Disable:

✗ Read-only Domain Controller

Configure DSRM password.

---

## DNS Options

Ignore warning:

"A delegation for this DNS server cannot be created"

---

## Additional Options

Verify:

NetBIOS:
SITEXNOW

---

## Install

Run prerequisite checks.

Confirm:

All prerequisite checks passed successfully.

Click:

Install

---

## Validation

Login screen displays:

SITEXNOW\Administrator

Verify tools:

* Active Directory Users and Computers
* DNS Manager
* Group Policy Management
