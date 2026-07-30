# Phase 1 - Hardware Setup

## Goal

Prepare the physical server hardware for installation of the server operating environment.

This phase includes assembling the system, verifying hardware functionality, updating firmware, and preparing the machine for the next phase.

---

# Task 1.1 - Assemble Hardware

## Goal

Build the physical server and confirm all components are installed correctly.

## Checklist

- [ ] Install CPU
- [ ] Install CPU cooler
- [ ] Install RAM
- [ ] Install NVMe storage
- [ ] Install HDD storage
- [ ] Install GPU
- [ ] Install motherboard into case
- [ ] Connect power cables
- [ ] Connect case fans
- [ ] Verify all components are seated correctly

## Checks

Confirm:

- All components are detected
- Fans spin correctly
- No obvious hardware issues are present

## Complete When

The server powers on and all installed hardware is recognized.

---

# Task 1.2 - Update BIOS / Firmware

## Goal

Ensure the motherboard firmware is current and configured correctly.

## Checklist

- [ ] Check current BIOS version
- [ ] Update BIOS if needed
- [ ] Load recommended default settings
- [ ] Enable required virtualization settings
- [ ] Confirm hardware detection

## Settings to Review

- CPU virtualization (AMD-V)
- IOMMU support (for GPU passthrough)
- Boot configuration
- Memory profile settings

## Complete When

The system firmware is updated and ready for virtualization.

---

# Task 1.3 - Verify Hardware Health

## Goal

Confirm the system is stable before installing software.

## Checklist

- [ ] Verify CPU temperatures
- [ ] Verify RAM detection
- [ ] Verify storage detection
- [ ] Verify GPU detection
- [ ] Check for hardware errors

## Testing

Run basic checks:

- System boot test
- Memory test
- Storage health check

## Complete When

The hardware is operating normally.

---

# Task 1.4 - Configure Storage Devices

## Goal

Prepare the storage devices for their intended roles.

## Storage Plan

### NVMe SSD

Used for:

- Hypervisor installation
- Virtual machines
- Applications

---

### HDD

Used for:

- File storage
- Digital assets
- Shared files
- Backups

## Checklist

- [ ] Confirm drive health
- [ ] Confirm storage capacity
- [ ] Label drives if needed
- [ ] Record drive information

## Complete When

Storage devices are identified and ready for configuration.

---

# Task 1.5 - Configure Network Hardware

## Goal

Ensure the server can connect to the home network.

## Checklist

- [ ] Identify network interface
- [ ] Confirm network cable connection
- [ ] Verify network adapter detection
- [ ] Record MAC address

## Complete When

The server can communicate with the network.

---

# Task 1.6 - Record Final Hardware Configuration

## Goal

Create a record of the final physical build.

## Checklist

- [ ] Confirm final component list
- [ ] Add missing hardware details
- [ ] Take photos of the build
- [ ] Update documentation

## Update

- Hardware.md

Include:

- Final component list
- BIOS version
- Storage layout
- Any hardware changes

## Complete When

The hardware documentation matches the actual server.

---

# Phase 1 Completion Checklist

- [ ] Hardware assembled
- [ ] BIOS updated
- [ ] Virtualization enabled
- [ ] Hardware tested
- [ ] Storage verified
- [ ] Network connection verified
- [ ] Documentation updated

---

# Phase 1 Complete

The server is physically ready for software installation.

Next Phase:

**Phase 2 - Hypervisor Installation**
