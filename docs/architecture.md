
# 🏗️ Homelab Architecture

## Current Architecture

```
Host Computer
│
├── VMware Workstation Pro
│
└── VMnet2 (Host-only)
      │
      └── DC01
          Windows Server 2022
```

---

## Planned Architecture

```
                        Internet
                            │
                     VMware NAT (VMnet8)
                            │
                        FW01 (pfSense)
                    WAN            LAN
                            │
                  192.168.10.0/24
                            │
      ┌────────────┬─────────────┬────────────┐
      │            │             │            │
    DC01         CL01        Ubuntu01      Kali01
 Active Directory Windows11   Linux        Security
 DNS Server                                 Testing
      │
      ├───────────────┐
      │               │
   Zabbix          Wazuh
 Monitoring      SIEM/XDR
```

---

## Network Plan

| Network | Purpose                    |
| ------- | -------------------------- |
| VMnet2  | Internal corporate network |
| VMnet8  | Internet access (WAN)      |

---

## Internal Addressing

| Device   | IP Address    |
| -------- | ------------- |
| FW01     | 192.168.10.1  |
| DC01     | 192.168.10.10 |
| Ubuntu01 | 192.168.10.20 |
| Zabbix   | 192.168.10.30 |
| Wazuh    | 192.168.10.40 |
| Kali01   | 192.168.10.50 |
| CL01     | DHCP          |

---

## Domain

```
sitexnow.local
```

---

## NetBIOS

```
SITEXNOW
```

---

## Virtualization Platform

* VMware Workstation Pro

---

## Operating Systems

* Windows Server 2022
* Windows 11
* Ubuntu Server LTS
* pfSense
* Kali Linux
