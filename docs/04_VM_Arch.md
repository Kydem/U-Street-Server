# VM Architecture

## Overview

The server will use virtualization to separate workloads into individual environments. This allows easier management, backups, troubleshooting, and future expansion.

---

# Hypervisor

## Proxmox

The server will use Proxmox as the hypervisor.

Proxmox will manage:

- Virtual machines
- Container workloads
- Storage
- Backups
- Networking

---

# Virtual Machine Layout

| VM | Purpose | OS | CPU | RAM | Storage |
|---|---|---|---|---|---|
| Windows Workstation | DaVinci / Blender | Windows | 6-8 vCPU | 10-16GB | NVMe |
| Docker Services | Web apps and tools | Linux | 2 vCPU | 4GB | NVMe |
| Game Servers | Arma / Zomboid | Linux | 8-10 vCPU | 12GB+ | NVMe |
| Storage | File storage | Linux | 2 vCPU | 4GB | HDD |

---

# VM Details

## Windows Workstation VM

### Purpose

Provides a remote desktop environment for creative workloads.

### Applications

- DaVinci Resolve Studio
- Blender
- Other GPU accelerated applications

### Resources

| Resource | Allocation |
|---|---|
| CPU | 6-8 vCPU |
| RAM | 10-16GB |
| GPU | RTX 2070 Super passthrough |
| Storage | NVMe |

---

## Docker Services VM

### Purpose

Hosts lightweight applications and web services.

### Applications

Potential services:

- Website
- Caddy
- Authentik
- Monitoring tools
- Other containers

### Resources

| Resource | Allocation |
|---|---|
| CPU | 2 vCPU |
| RAM | 4GB |
| Storage | NVMe |

---

## Game Server VM

### Purpose

Hosts dedicated multiplayer game servers.

### Applications

Initial servers:

- Arma
- Project Zomboid

Future possibilities:

- Additional Steam servers

### Resources

| Resource | Allocation |
|---|---|
| CPU | 8-10 vCPU |
| RAM | 12GB+ |
| Storage | NVMe |

### Notes

Game servers are prioritized due to their CPU and memory requirements.

---

## Storage VM

### Purpose

Provides centralized storage for files and digital assets.

### Data Stored

- Videos
- Projects
- Documents
- Shared files
- Backups

### Resources

| Resource | Allocation |
|---|---|
| CPU | 2 vCPU |
| RAM | 4GB |
| Storage | 8TB HDD |

---

# Resource Summary

Current hardware:

- CPU: Ryzen 7 7800X3D (8 cores / 16 threads)
- RAM: 32GB DDR5
- Storage: 1TB NVMe + 8TB HDD

Planned allocation:

| Resource | Usage |
|---|---|
| CPU | Shared between VMs |
| RAM | Primarily allocated to active workloads |
| NVMe | VM storage |
| HDD | File storage |

---

# VM Priority

If resources become limited, workloads should be prioritized in this order:

1. Game Servers
2. Storage Services
3. Windows Workstation
4. Docker Services


---

# Future Expansion

Possible changes:

- Increase RAM to 64GB
- Add additional game servers
- Add redundant storage
- Separate storage into dedicated NAS hardware

---

# Notes

VM resources may be adjusted after observing real-world usage.
