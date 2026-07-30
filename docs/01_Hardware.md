# Hardware

# System Components

| Component | Specification |
|-----------|---------------|
| CPU | AMD Ryzen 7 7800X3D |
| GPU | NVIDIA RTX 2070 Super |
| RAM | 32GB DDR5 |
| Boot / VM Storage | 1TB WD Black NVMe |
| Data Storage | 8TB Seagate HDD |
| Motherboard | TBD |
| PSU | TBD |
| Case | TBD |
| Cooling | TBD |

---

# Component Purpose

## CPU

**AMD Ryzen 7 7800X3D**

Primary uses:

- Virtual machine workloads
- Game server processing
- General server tasks

The CPU was selected due to its strong single-thread performance and 3D V-Cache.

---

## GPU

**NVIDIA RTX 2070 Super**

Primary uses:

- DaVinci Resolve Studio
- Blender rendering
- GPU accelerated workloads

The GPU will be assigned to the Windows workstation VM using GPU passthrough.

---

## Memory

**32GB DDR5**

Current use:

- Virtual machines
- Containers
- Game servers

Planned upgrade:

- 64GB DDR5

Reason:

Additional memory will allow more simultaneous workloads and larger game servers.

---

## Storage

### 1TB NVMe SSD

Used for:

- Proxmox installation
- Virtual machine storage
- Applications

---

### 8TB HDD

Used for:

- Video files
- Digital assets
- Shared storage
- Archives
- Backups

---

# Future Upgrades

Potential upgrades:

- [ ] Increase RAM to 64GB
- [ ] Add additional storage drive
- [ ] Add storage redundancy
- [ ] Add UPS
- [ ] Upgrade network speed

---

# Notes

Additional hardware details will be added as the system is assembled.
