# 📅 Day 01 - Building the Foundation

**Date:** June 10, 2026

---

# 🎯 Goal

Start building my enterprise cybersecurity homelab.

---

# ✅ Accomplished

- Installed VMware Workstation Pro
- Enabled virtualization support in BIOS
- Learned the differences between NAT, Bridged and Host-only networks
- Created VMnet2 using Host-only mode
- Planned the internal network (192.168.10.0/24)
- Created the first virtual machine (DC01)
- Installed Windows Server 2022 Evaluation (English)
- Solved the "Microsoft Software License Terms" error caused by VMware Easy Install
- Learned how to create and manage VMware Snapshots
- Configured the server before Active Directory promotion

---

# 📚 Concepts Learned

## NAT

Allows virtual machines to access the Internet through the host.

## Bridged

Connects the VM directly to the physical network.

## Host-only

Creates an isolated network between the host and virtual machines.

## Snapshot

A snapshot captures the state of a virtual machine before major changes, allowing quick rollback if needed.

## Workgroup vs Domain

Workgroups manage users locally on each computer.

Domains centralize authentication and management through Active Directory.

---

# ⚠️ Challenges

The VMware Easy Install feature generated the following error:

> Windows cannot find the Microsoft Software License Terms.

Solution:

- Recreated the VM
- Selected "I will install the operating system later"
- Mounted the ISO manually

The installation completed successfully.

---

# 💡 Key Takeaways

- Snapshots should always be created before critical changes.
- Host-only networking is ideal for isolated lab environments.
- Manual installation provides greater control than Easy Install.
- Understanding the reason behind each configuration is more valuable than memorizing steps.

---

# 🚀 Next Steps

- Promote DC01 to Domain Controller
- Create the sitexnow.local forest
- Configure DNS
- Create the first Active Directory users

---

# 🧠 Reflection

Today I realized that virtualization is much more than simply creating virtual machines.

Understanding network modes, snapshots and installation methods helped me see how enterprise environments are structured and how important planning is before deploying infrastructure.
