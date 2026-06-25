# Day 04 - First Domain Client

## Objective

Deploy the first Windows 11 workstation and integrate it into the SitexNow Active Directory environment.

---

## Activities Completed

### Windows 11 Deployment

Created a new virtual machine:

* Hostname: CL01
* Operating System: Windows 11 Pro
* Network: VMnet2 (Host-Only)
* Resources:

  * 2 vCPU
  * 8 GB RAM
  * 80 GB Disk

---

### Network Configuration

Configured static network settings:

IP Address:
192.168.10.20

Subnet Mask:
255.255.255.0

DNS Server:
192.168.10.10

The workstation was configured to use DC01 as its primary DNS server.

---

### Connectivity Validation

Successfully tested:

* Ping to DC01
* DNS resolution through Active Directory DNS
* Name resolution for domain resources

Commands used:

* ping 192.168.10.10
* ping dc01
* nslookup sitexnow.local

---

### Domain Join

Joined CL01 to:

sitexnow.local

Administrative credentials were used to authorize the join operation.

After reboot, the workstation became a trusted member of the domain.

---

### Authentication Testing

Successfully authenticated using:

SITEXNOW\joao.user

This validated:

* Active Directory communication
* DNS functionality
* Domain trust relationship
* User authentication process

---

## Key Learnings

### Active Directory Depends on DNS

Domain Join is only possible when DNS correctly resolves domain resources and Domain Controllers.

### Computers Are Objects

When a workstation joins a domain, a computer object is automatically created in Active Directory.

Example:

CL01

This object is separate from user accounts.

### Trust Relationship

The workstation establishes a secure trust relationship with the Domain Controller.

This trust is used for:

* User authentication
* Group Policy processing
* Kerberos authentication
* Secure communication with Active Directory

### Domain Authentication

Users no longer authenticate locally.

Authentication is performed by the Domain Controller.

Example:

SITEXNOW\joao.user

instead of

CL01\localuser

---

## Snapshots

Created:

* CL01 - 01 Domain Joined
* DC01 - 04 First Client Joined

---

## Next Steps

* Create and manage Group Policy Objects (GPO)
* Organize computer objects into dedicated OUs
* Apply security policies
* Begin centralized workstation management
