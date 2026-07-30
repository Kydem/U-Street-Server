# Roadmap

This document tracks the overall progress of the U-Street Server project. It serves as a high-level overview of completed work, current priorities, and planned features.

---

## Status Legend

* Complete
* In Progress
* Planned
* Future Consideration

---

# Milestone 1 — Hardware

**Objective**

Build and validate the physical server hardware.

### Tasks

* [ ] Finalize hardware selection
* [ ] Assemble server
* [ ] Configure BIOS settings
* [ ] Update firmware
* [ ] Verify drive health
* [ ] Stress test hardware
* [ ] Verify system stability

**Completion Criteria**

* Hardware passes stress testing
* No hardware faults detected
* All storage devices recognized

---

# Milestone 2 — Base System

**Objective**

Install and configure the virtualization platform.

### Tasks

* [ ] Install Proxmox
* [ ] Configure networking
* [ ] Configure storage
* [ ] Configure backups
* [ ] Create administrator account
* [ ] Document installation

**Completion Criteria**

* Hypervisor is operational
* Storage is configured
* Backups are functioning

---

# Milestone 3 — Core Infrastructure

**Objective**

Deploy the services required for everyday operation.

### Tasks

* [ ] Deploy Docker
* [ ] Configure shared storage
* [ ] Configure SMB shares
* [ ] Create user accounts
* [ ] Verify permissions
* [ ] Document service layout

---

# Milestone 4 — Game Servers

**Objective**

Deploy dedicated game servers for the group.

### Planned Servers

* [ ] Project Zomboid
* [ ] Minecraft
* [ ] Arma Reforger
* [ ] Factorio

For each deployment:

* [ ] Install
* [ ] Configure
* [ ] Test
* [ ] Create backup schedule
* [ ] Document management procedures

---

# Milestone 5 — Storage Services

**Objective**

Provide centralized storage for media and shared files.

### Tasks

* [ ] Shared file storage
* [ ] Video editing workspace
* [ ] Network backups
* [ ] Archive storage
* [ ] Optional cloud storage platform

---

# Milestone 6 — Remote Access

**Objective**

Allow secure remote administration.

### Tasks

* [ ] VPN
* [ ] SSH configuration
* [ ] Remote desktop access
* [ ] Multi-factor authentication
* [ ] User access controls

---

# Milestone 7 — Monitoring

**Objective**

Monitor system health and resource usage.

### Tasks

* [ ] Resource monitoring
* [ ] Storage monitoring
* [ ] Temperature monitoring
* [ ] Network monitoring
* [ ] Alert notifications
* [ ] Service status dashboard

---

# Milestone 8 — Security

**Objective**

Improve security and recovery capabilities.

### Tasks

* [ ] Firewall configuration
* [ ] Automatic security updates
* [ ] Least-privilege user accounts
* [ ] Backup verification
* [ ] Disaster recovery documentation

---

# Future Ideas

The following features are not currently planned but may be added later.

* CI/CD runner
* Media server

---

# Current Priorities

## In Progress

* Aquire hardware
* Planning

## Next Up

1. Assemble hardware
2. Install Proxmox
3. Configure networking
4. Deploy the first game server

---

# Notes

This roadmap is intended to remain concise. Detailed implementation notes, configuration guides, and troubleshooting information should be documented within the `/docs` directory.

