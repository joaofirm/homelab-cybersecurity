# Runbook 07 - Create Users and Security Groups

## Objective

Create user accounts and security groups for the SitexNow Active Directory environment.

---

## Open Active Directory Users and Computers

Server Manager

Tools

Active Directory Users and Computers

---

## Create Users

Navigate to:

User Accounts

Create:

* joao.admin
* joao.user
* maria.rh
* carlos.finance

---

## Create Security Groups

Navigate to:

Groups

Create:

* IT_Admins
* HR_Users
* Finance_Users

Group Scope:

Global

Group Type:

Security

---

## Assign Users to Groups

Add:

joao.admin → IT_Admins

maria.rh → HR_Users

carlos.finance → Finance_Users

---

## Administrative Access

Recommended model:

User
↓
IT_Admins
↓
Domain Admins

Avoid assigning users directly to Domain Admins whenever possible.

---

## Validation

Verify group membership through:

User Properties

→ Member Of

Expected:

joao.admin

* Domain Users
* IT_Admins

maria.rh

* Domain Users
* HR_Users

carlos.finance

* Domain Users
* Finance_Users

joao.user

* Domain Users

---

## Notes

All users are automatically added to the Domain Users group.

Permissions are inherited through security group membership.
