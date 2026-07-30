# Phase 2 - Hypervisor Installation

## Goal

Install and configure the server virtualization platform.

This phase will transform the physical hardware into a platform capable of running multiple virtual machines and services.

The goal is to create a stable foundation before deploying workloads.

---

# Task 2.1 - Install Proxmox

## Goal

Install the hypervisor operating system on the server.

## Checklist

- [ ] Download latest Proxmox installer
- [ ] Create installation media
- [ ] Boot server from installer
- [ ] Install Proxmox to NVMe drive
- [ ] Configure initial settings
- [ ] Reboot into Proxmox

## Configuration Decisions

Confirm:

- Proxmox installation location
- Hostname
- Management IP address
- Region/time settings

## Complete When

The server boots successfully into Proxmox.

---

# Task 2.2 - Configure Proxmox Management

## Goal

Set up the basic management environment.

## Checklist

- [ ] Access Proxmox web interface
- [ ] Confirm administrator access
- [ ] Update Proxmox packages
- [ ] Configure repositories
- [ ] Verify system information

## Verify

Confirm:

- CPU is detected
- RAM is detected
- GPU is detected
- Storage devices are visible
- Network interface is working

## Complete When

Proxmox can be accessed and managed.

---

# Task 2.3 - Configure Storage

## Goal

Prepare storage locations for virtual machines and data.

## Storage Plan

### NVMe SSD

Used for:

- Proxmox system files
- Virtual machine storage
- Application workloads

---

### 8TB HDD

Used for:

- File storage
- Digital assets
- Backups
- Large data files

## Checklist

- [ ] Identify storage devices
- [ ] Create storage pools
- [ ] Configure storage permissions
- [ ] Confirm available capacity

## Complete When

Proxmox can use the planned storage locations.

---

# Task 2.4 - Configure Networking

## Goal

Connect Proxmox to the planned network design.

## Checklist

- [ ] Configure network bridge
- [ ] Assign management IP
- [ ] Verify gateway settings
- [ ] Verify internet access
- [ ] Test network connectivity

## Confirm

- Proxmox can reach updates
- Other devices can access Proxmox
- Network settings are documented

## Complete When

The server can communicate reliably on the network.

---

# Task 2.5 - Configure GPU Passthrough Preparation

## Goal

Prepare the system for assigning the GPU to the Windows workstation VM.

## Checklist

- [ ] Enable IOMMU settings
- [ ] Verify GPU detection
- [ ] Confirm GPU grouping
- [ ] Document passthrough requirements

## Notes

GPU passthrough will be completed later when the Windows VM is created.

## Complete When

The server is ready for GPU passthrough configuration.

---

# Task 2.6 - Configure Basic Server Maintenance

## Goal

Create basic management practices before adding workloads.

## Checklist

- [ ] Configure automatic updates
- [ ] Configure time synchronization
- [ ] Record system information
- [ ] Set up basic monitoring access

## Document

Record:

- Proxmox version
- Hostname
- IP address
- Storage configuration

## Complete When

The server has basic maintenance practices in place.

---

# Task 2.7 - Create Initial Backup Plan

## Goal

Prepare for recovering the server configuration.

## Checklist

- [ ] Identify what should be backed up
- [ ] Configure initial VM backup location
- [ ] Document backup process

## Initial Backup Targets

Examples:

- Proxmox configuration
- VM snapshots
- Important settings

## Complete When

A basic recovery plan exists.

---

# Phase 2 Completion Checklist

- [ ] Proxmox installed
- [ ] Management access configured
- [ ] Storage configured
- [ ] Network configured
- [ ] GPU passthrough prepared
- [ ] Maintenance basics completed
- [ ] Backup approach documented

---

# Phase 2 Complete

The server is now ready to begin hosting virtual machines.

Next Phase:

**Phase 3 - Network Configuration**
