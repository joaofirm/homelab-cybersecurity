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

* <>.admin
* <>.user
* <>.rh
* <>.finance

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

<>.admin → IT_Admins

<>.rh → HR_Users

<>.finance → Finance_Users

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

<>.admin

* Domain Users
* IT_Admins

<>.rh

* Domain Users
* HR_Users

<>.finance

* Domain Users
* Finance_Users

<>.user

* Domain Users

---

## Notes

All users are automatically added to the Domain Users group.

Permissions are inherited through security group membership.
