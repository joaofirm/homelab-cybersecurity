# Day 03 - Active Directory Foundation

## Objective

Deploy the first Active Directory Domain Controller and establish the initial organizational structure of the SitexNow environment.

---

## Activities Completed

### Active Directory Deployment

* Installed Active Directory Domain Services (AD DS)
* Installed DNS Server role
* Promoted DC01 to Domain Controller
* Created a new forest: sitexnow.local
* Configured NetBIOS name: SITEXNOW

### Organizational Units

Created the following OUs:

* Servers
* Workstations
* User Accounts
* Groups
* IT
* HR
* Finance

### User Accounts

Created:

* joao.admin
* joao.user
* maria.rh
* carlos.finance

### Security Groups

Created:

* IT_Admins
* HR_Users
* Finance_Users

### Group Membership

* joao.admin → IT_Admins
* maria.rh → HR_Users
* carlos.finance → Finance_Users

---

## Key Learnings

### Active Directory Structure

Learned the relationship between:

* Forest
* Domain
* Organizational Units (OUs)
* Users
* Groups

### Permission Model

Users do not become administrators by changing their account type.

Administrative privileges are inherited through group membership.

Example:

joao.admin
↓
IT_Admins
↓
Domain Admins

### Domain Users

All user accounts are automatically added to the Domain Users group.

Additional permissions are granted through supplemental security groups.

---

## Snapshots

Created:

* 01 - Windows Server Configured
* 02 - Domain Controller Created
* 03 - Active Directory Base Structure

---

## Next Steps

* Create Windows 11 client VM
* Join workstation to sitexnow.local
* Validate domain authentication
* Begin Group Policy (GPO) implementation
