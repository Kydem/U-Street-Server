# Network

## Overview

This document describes the network setup for the home server.

The goal is to provide:
- Secure access to server services
- Reliable connectivity for virtual machines
- Separation between server workloads and personal devices
- Room for future expansion

---

# Network Layout

```
Internet
   |
Router / Firewall
   |
Managed Switch
   |
Server
   |
Proxmox
   |
Virtual Machines
```

---

# Main Devices

| Device | Purpose |
|---|---|
| Router | Internet access and network management |
| Switch | Connects network devices |
| Home Server | Runs virtual machines and services |
| Personal Devices | PCs, laptops, phones |

---

# Network Segmentation

The network may use VLANs to separate different types of traffic.

| VLAN | Purpose |
|---|---|
| Management | Server and network administration |
| Servers | Virtual machines and hosted services |
| Personal | Trusted home devices |
| Guest | Visitor devices |

---

# Remote Access

Remote access will use secure methods such as:

- Tailscale
- VPN
- Authenticated web access

Direct exposure of management services (Proxmox, SSH, etc.) should be avoided.

---

# Future Improvements

Possible upgrades:

- Faster networking
- Additional VLANs
- Dedicated firewall hardware
- Improved wireless coverage

---

# Notes

Network design may change as the server grows.
