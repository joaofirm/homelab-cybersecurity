# Runbook 09 - Install and Configure DHCP Server

## Objective

Install and configure the DHCP Server role on Windows Server 2022 integrated with Active Directory.

---

## Environment

| Item             | Value               |
| ---------------- | ------------------- |
| Server           | DC01                |
| Operating System | Windows Server 2022 |
| Domain           | sitexnow.local      |
| Server IP        | 192.168.10.10       |

---

# Step 1 - Install DHCP Server Role

Open:

Server Manager

Manage → Add Roles and Features

Select:

* DHCP Server

Proceed with the installation.

---

# Step 2 - Complete Post-Deployment Configuration

After installation:

Notifications → Complete DHCP Configuration

Use:

SITEXNOW\Administrator

Authorize the DHCP Server in Active Directory.

---

# Step 3 - Open DHCP Console

Server Manager

Tools

DHCP

Expand:

DC01

IPv4

---

# Step 4 - Create a New Scope

Right-click:

IPv4

New Scope

Configure:

Scope Name

Corporate LAN

Description

DHCP Scope for SitexNow internal network

---

# Step 5 - Configure Address Pool

Start IP

192.168.10.100

End IP

192.168.10.199

Subnet Mask

255.255.255.0

---

# Step 6 - Exclusions

No exclusions required.

Reason:

Infrastructure addresses are outside the DHCP range.

---

# Step 7 - Lease Duration

Lease:

8 Days

---

# Step 8 - Configure DHCP Options

Default Gateway

192.168.10.1

DNS Server

192.168.10.10

Domain Name

sitexnow.local

WINS

Not configured.

---

# Step 9 - Activate Scope

Select:

Activate this Scope

Finish.

---

# Step 10 - Configure Client

On CL01:

Set IPv4 to:

* Obtain an IP address automatically
* Obtain DNS server automatically

Run:

ipconfig /release

ipconfig /renew

ipconfig /all

---

# Validation

Verify:

* DHCP Enabled = Yes
* DHCP Server = 192.168.10.10
* DNS Server = 192.168.10.10
* Default Gateway = 192.168.10.1

On DC01:

DHCP

IPv4

Corporate LAN

Address Leases

Confirm CL01 received an IP address automatically.

---

# Expected Result

The client receives:

* IPv4 Address
* Subnet Mask
* Default Gateway
* DNS Server
* DNS Domain

Automatically from the DHCP Server.
