# Phase 3 - Virtual Machine Setup

## Goal

Create and configure the virtual machines that will run the server workloads.

This phase establishes the core environments for:

- Remote workstation access
- Game server hosting
- Application hosting
- File storage

The goal is to create clean, organized VMs before installing individual services.

---

# Task 3.1 - Create VM Templates

## Goal

Create a consistent starting point for new virtual machines.

## Checklist

- [ ] Decide operating systems required
- [ ] Download installation media
- [ ] Create base VM configurations
- [ ] Define default VM settings

## Considerations

Define:

- CPU allocation
- Memory allocation
- Storage location
- Network connection
- Backup requirements

## Complete When

Standard VM creation settings are documented.

---

# Task 3.2 - Create Windows Workstation VM

## Goal

Create the remote workstation environment for creative workloads.

## Purpose

Used for:

- DaVinci Resolve Studio
- Blender
- GPU accelerated applications

## Checklist

- [ ] Create Windows VM
- [ ] Assign CPU resources
- [ ] Assign RAM resources
- [ ] Install Windows
- [ ] Install drivers
- [ ] Configure GPU passthrough
- [ ] Test remote access

## Resource Allocation

Initial target:

- CPU: 6-8 vCPU
- RAM: 10-16GB
- Storage: NVMe
- GPU: RTX 2070 Super passthrough

## Complete When

The workstation VM can run GPU workloads remotely.

---

# Task 3.3 - Create Game Server VM

## Goal

Create an environment dedicated to game server hosting.

## Purpose

Used for:

- Arma servers
- Project Zomboid servers
- Future Steam servers

## Checklist

- [ ] Create Linux VM
- [ ] Assign CPU resources
- [ ] Assign RAM resources
- [ ] Install operating system
- [ ] Configure remote management
- [ ] Prepare Steam server environment

## Resource Allocation

Initial target:

- CPU: 8-10 vCPU
- RAM: 12GB+
- Storage: NVMe

## Complete When

The VM is ready to host game servers.

---

# Task 3.4 - Create Docker Services VM

## Goal

Create a dedicated environment for running containerized applications.

## Purpose

Used for:

- Websites
- Internal tools
- Supporting services
- Future applications

## Checklist

- [ ] Create Linux VM
- [ ] Assign resources
- [ ] Install operating system
- [ ] Install Docker
- [ ] Configure container storage
- [ ] Test container deployment

## Resource Allocation

Initial target:

- CPU: 2-4 vCPU
- RAM: 4GB+
- Storage: NVMe

## Complete When

Docker containers can be deployed and managed.

---

# Task 3.5 - Create Storage VM

## Goal

Create the storage environment for shared files and digital assets.

## Purpose

Used for:

- Video files
- Project files
- Digital assets
- Shared storage

## Checklist

- [ ] Create storage VM
- [ ] Attach storage drive
- [ ] Configure storage access
- [ ] Create shared folders
- [ ] Test file transfers

## Resource Allocation

Initial target:

- CPU: 2 vCPU
- RAM: 4GB
- Storage: 8TB HDD

## Complete When

Users can access shared storage.

---

# Task 3.6 - Configure VM Networking

## Goal

Connect each VM to the correct network.

## Checklist

- [ ] Assign VM network interfaces
- [ ] Confirm IP addressing
- [ ] Verify VM communication
- [ ] Confirm internet access where needed
- [ ] Document VM network settings

## Complete When

All VMs can communicate as intended.

---

# Task 3.7 - Configure VM Management

## Goal

Create a consistent way to manage each VM.

## Checklist

- [ ] Define VM naming convention
- [ ] Document IP addresses
- [ ] Document administrator access
- [ ] Configure updates
- [ ] Create initial backups/snapshots

## Naming Example

```
VM-WORKSTATION
VM-GAMESERVER
VM-DOCKER
VM-STORAGE
```

## Complete When

Each VM can be identified and maintained.

---

# Task 3.8 - Update Documentation

## Goal

Document the final VM layout.

## Checklist

- [ ] Update VM Architecture.md
- [ ] Record final resource allocations
- [ ] Record VM names
- [ ] Record storage assignments
- [ ] Record network assignments

## Complete When

Documentation matches the running environment.

---

# Phase 3 Completion Checklist

- [ ] VM templates created
- [ ] Windows workstation VM created
- [ ] Game server VM created
- [ ] Docker VM created
- [ ] Storage VM created
- [ ] VM networking configured
- [ ] VM documentation updated

---

# Phase 3 Complete

The server now has its core environments created and is ready for service deployment.

Next Phase:

**Phase 4 - Service Installation & Configuration**
