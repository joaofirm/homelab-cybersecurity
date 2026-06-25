# Day 04 - DHCP Deployment & First Group Policy

**Date:** 2026-06-25

---

## Objectives

Today's goals were:

- Deploy DHCP Server
- Create and configure the first DHCP Scope
- Configure automatic IP assignment
- Validate DHCP leases
- Create and test the first Group Policy Object (GPO)

---

## What I Learned

### DHCP Server

Installed the DHCP Server role on DC01 and completed the post-deployment configuration.

Learned why a DHCP Server must be authorized in Active Directory before it can distribute IP addresses.

---

### DHCP Scope

Created the first scope:

Network:
192.168.10.0/24

Range:
192.168.10.100 - 192.168.10.199

Lease:
8 Days

Gateway:
192.168.10.1 (reserved for future pfSense deployment)

DNS:
192.168.10.10

Domain:
sitexnow.local

---

### DHCP Concepts

Today I finally connected theory with practice.

Concepts learned:

- DHCP Scope
- Lease Duration
- Address Pool
- Address Leases
- Scope Options
- Reservations
- Exclusions

Understanding these concepts became much easier after configuring a real DHCP server.

---

### Automatic Client Configuration

Changed CL01 from static configuration to DHCP.

Validated:

- Automatic IP assignment
- Automatic DNS configuration
- Automatic Domain Name configuration
- DHCP Lease creation

Used:

ipconfig /release

ipconfig /renew

ipconfig /all

---

### First Group Policy

Created my first Group Policy Object.

Policy:

Workstation Login Banner

Applied to:

OU: Workstations

Validated by:

- gpupdate
- Successful login banner display

This helped me understand how GPOs are linked to Organizational Units and automatically inherited by computers inside them.

---

## Biggest Lesson

One thing that became clear today is that Windows infrastructure is much more integrated than I initially imagined.

Active Directory, DNS, DHCP and Group Policy are not isolated technologies—they work together to automate administration across the entire network.

Configuring DHCP manually would have been easy.

Understanding why each option exists is what actually builds real administration skills.

---

## Lab Status

Current environment:

DC01
- Active Directory
- DNS
- DHCP
- Group Policy

CL01
- Joined to Domain
- DHCP Client
- Receiving Group Policies

---

## Next Session

Planned topics:

- Advanced Group Policies
- Password Policy
- Account Lockout Policy
- Drive Mapping
- File Server preparation
