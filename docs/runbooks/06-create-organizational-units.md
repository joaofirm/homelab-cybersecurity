# Runbook 06 - Create Organizational Units

## Objective

Create the initial organizational structure of the SitexNow domain.

---

## Open Console

Server Manager

Tools

Active Directory Users and Computers

---

## Create OUs

Right-click:

sitexnow.local

New

Organizational Unit

Create:

* Servers
* Workstations
* User Accounts
* Groups
* IT
* HR
* Finance

---

## Expected Structure

sitexnow.local

├── Servers
├── Workstations
├── User Accounts
├── Groups
├── IT
├── HR
├── Finance

---

## Notes

The default Users container already exists and should not be replaced.

Custom user accounts should be stored in the User Accounts OU.

Workstations joined to the domain will later be moved from the default Computers container to the Workstations OU.
