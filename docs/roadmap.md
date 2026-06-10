
# 🗺️ Homelab Roadmap

## 📌 Project Vision

This homelab is designed to simulate a real enterprise infrastructure, providing hands-on experience in System Administration, Networking, Virtualization, Monitoring and Cybersecurity.

The objective is to build every service from scratch while documenting the learning process and the implementation decisions.

---

# 🚀 Phase 1 - Foundation

* [x] Install VMware Workstation Pro
* [x] Enable hardware virtualization
* [x] Create isolated virtual network (VMnet2)
* [x] Install Windows Server 2022
* [ ] Promote DC01 to Domain Controller
* [ ] Create the `sitexnow.local` forest

---

# 🖥️ Phase 2 - Active Directory

* [ ] Organizational Units (OU)
* [ ] Users and Groups
* [ ] Security Groups
* [ ] Administrative Accounts
* [ ] Service Accounts

---

# 🌐 Phase 3 - Network Services

* [ ] DNS configuration
* [ ] DHCP implementation
* [ ] Static reservations
* [ ] DNS Forwarders

---

# 💻 Phase 4 - Client Infrastructure

* [ ] Deploy Windows 11 client
* [ ] Join workstation to domain
* [ ] User authentication tests
* [ ] Folder redirection
* [ ] Roaming profiles (optional)

---

# 🔐 Phase 5 - Group Policy

* [ ] Password Policy
* [ ] Account Lockout Policy
* [ ] Windows Defender configuration
* [ ] Windows Update policy
* [ ] Desktop restrictions

---

# 🔥 Phase 6 - Firewall

* [ ] Deploy pfSense
* [ ] Configure WAN
* [ ] Configure LAN
* [ ] NAT
* [ ] Firewall Rules

---

# 📊 Phase 7 - Monitoring

* [ ] Deploy Zabbix
* [ ] Monitor Windows Server
* [ ] Monitor Linux
* [ ] CPU and Memory alerts
* [ ] Disk monitoring

---

# 🛡️ Phase 8 - Security Monitoring

* [ ] Deploy Wazuh
* [ ] Install Windows Agent
* [ ] Install Linux Agent
* [ ] Centralize logs
* [ ] Detect brute force attempts

---

# 🐧 Phase 9 - Linux

* [ ] Ubuntu Server
* [ ] SSH Hardening
* [ ] File sharing
* [ ] Domain integration

---

# ⚔️ Phase 10 - Offensive Security

* [ ] Deploy Kali Linux
* [ ] Internal reconnaissance
* [ ] Password auditing
* [ ] SMB enumeration
* [ ] Detection validation

---

# 🚨 Phase 11 - Incident Response

* [ ] Generate attack logs
* [ ] Analyze events in Wazuh
* [ ] Validate detections
* [ ] Document findings
* [ ] Create incident reports

---

# 🎯 Final Goal

Build a fully functional enterprise homelab capable of demonstrating practical skills in Infrastructure, System Administration and Blue Team Cybersecurity.
