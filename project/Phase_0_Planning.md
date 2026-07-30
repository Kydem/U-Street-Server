# Phase 0 - Planning & Design

## Goal

Before building the server, define what we are creating, how it will be structured, and what tools we will use.

This phase focuses on making the major decisions before moving into implementation.

---

# Task 0.1 - Define Project Scope

## Goal

Confirm what the server will be used for and what features are included in the first version.

## Checklist

- [ ] Confirm primary use cases
- [ ] Confirm initial services
- [ ] Identify users and access needs
- [ ] Separate required features from future ideas

## Output

Update:

- Project Overview.md

## Complete When

Everyone agrees on what the first version of the server needs to accomplish.

---

# Task 0.2 - Review Hardware

## Goal

Document the available hardware and confirm it supports the planned workloads.

## Checklist

- [ ] Document CPU, GPU, RAM, and storage
- [ ] Review hardware limitations
- [ ] Identify possible upgrades

## Questions

- Is there enough RAM for the planned VMs?
- Which workloads require the most resources?
- Are there any hardware concerns before starting?

## Output

Update:

- Hardware.md

## Complete When

The team understands the capabilities and limitations of the hardware.

---

# Task 0.3 - Plan Virtual Machines

## Goal

Define how the server resources will be divided.

## Checklist

- [ ] Define required VMs
- [ ] Assign CPU and RAM resources
- [ ] Define storage locations
- [ ] Identify VM priorities

## Planned VMs

### Windows Workstation

Used for:

- DaVinci Resolve
- Blender
- Remote desktop workloads

---

### Docker Services

Used for:

- Websites
- Applications
- Supporting services

---

### Game Server VM

Used for:

- Arma
- Project Zomboid
- Future game servers

---

### Storage VM

Used for:

- Shared files
- Digital assets
- Project storage

## Output

Update:

- VM Architecture.md

## Complete When

Each workload has a defined place to run.

---

# Task 0.4 - Plan Network

## Goal

Define how devices, users, and services will connect.

## Checklist

- [ ] Document current network setup
- [ ] Decide if VLANs are needed
- [ ] Plan server network connection
- [ ] Plan remote access

## Questions

- What services need remote access?
- What services should remain private?
- How will users connect?

## Output

Update:

- Network.md
- Remote Access.md

## Complete When

The basic network design is understood.

---

# Task 0.5 - Plan Storage

## Goal

Define where data will live and how it will be accessed.

## Checklist

- [ ] Define NVMe usage
- [ ] Define HDD usage
- [ ] Plan folder structure
- [ ] Identify important data

## Questions

- What data needs backups?
- Who needs access?
- How will files be shared?

## Output

Update:

- Storage.md

## Complete When

The storage layout is documented.

---

# Task 0.6 - Define Security Approach

## Goal

Establish basic security practices before exposing services.

## Checklist

- [ ] Define user access levels
- [ ] Decide authentication methods
- [ ] Decide remote access method
- [ ] Identify services that should not be public

## Output

Update:

- Security.md
- Remote Access.md

## Complete When

Basic access rules are defined.

---

# Task 0.7 - Select Software

## Goal

Choose the main tools used to build and manage the server.

## Decide On:

- Hypervisor
- Container platform
- Remote access tools
- Monitoring tools
- Web hosting tools

## Current Candidates

Hypervisor:

- Proxmox

Containers:

- Docker

Remote Access:

- Tailscale

Monitoring:

- Grafana / Prometheus / Uptime Kuma

## Complete When

The core software stack has been selected.

---

# Task 0.8 - Finalize Build Plan

## Goal

Create the roadmap for implementation.

## Checklist

- [ ] Create GitHub issues
- [ ] Define build phases
- [ ] Assign tasks
- [ ] Identify dependencies

## Planned Phases

1. Hardware Setup
2. Hypervisor Installation
3. Networking
4. Storage
5. VM Deployment
6. Service Deployment
7. Security Setup
8. Testing and Optimization

## Complete When

The team knows what happens next.

---

# Phase 0 Completion Checklist

- [ ] Project scope defined
- [ ] Hardware reviewed
- [ ] VM plan completed
- [ ] Network plan completed
- [ ] Storage plan completed
- [ ] Security approach defined
- [ ] Software selected
- [ ] Implementation roadmap created
