
# 📦 Lab Inventory

## Host Machine

| Component  | Specification          |
| ---------- | ---------------------- |
| CPU        | Intel Xeon E5-2696 v4  |
| Memory     | 64 GB RAM              |
| Hypervisor | VMware Workstation Pro |

---

# Virtual Machines

| Name     | Role                | Status     |
| -------- | ------------------- | ---------- |
| DC01     | Domain Controller   | 🟢 Active  |
| FW01     | pfSense Firewall    | 🔴 Planned |
| CL01     | Windows 11 Client   | 🟢 Active |
| Ubuntu01 | Linux Server        | 🔴 Planned |
| Zabbix   | Monitoring Server   | 🔴 Planned |
| Wazuh    | Security Monitoring | 🔴 Planned |
| Kali01   | Security Testing    | 🔴 Planned |

---

# Network Information

| Property         | Value           |
| ---------------- | --------------- |
| Internal Network | VMnet2          |
| Address Space    | 192.168.10.0/24 |
| Gateway          | 192.168.10.1    |
| Domain           | sitexnow.local  |

---

# Snapshots

| Snapshot                 | Purpose               |
| ------------------------ | --------------------- |
| Before Domain Controller | Before AD promotion   |
| Domain Ready             | After AD installation |
| Before GPO Testing       | Safe rollback point   |
| Before pfSense           | Network baseline      |
| Before Wazuh             | Monitoring baseline   |

---

# Learning Objectives

* VMware Virtualization
* Windows Server Administration
* Active Directory
* DNS
* Group Policy
* pfSense
* Linux Administration
* Infrastructure Monitoring
* Security Monitoring
* Blue Team Operations
* Incident Response

---

# Repository Purpose

This repository serves as a technical journal and portfolio documenting the implementation of a complete enterprise homelab focused on infrastructure and cybersecurity.

Every configuration, challenge and lesson learned will be documented throughout the project.
