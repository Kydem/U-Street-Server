# Phase 5 - Security & Access

## Goal

Secure the server environment and establish how users will access services.

This phase focuses on protecting the server, managing users, and configuring the tools required for secure remote access, authentication, and network control.

---

# Task 5.1 - Review Current Exposure

## Goal

Understand what services are accessible and determine how each service should be accessed.

Before adding security controls, identify what needs to be protected.

## Checklist

- [ ] Review running services
- [ ] Identify services exposed to the internet
- [ ] Identify services that should remain private
- [ ] Review open ports
- [ ] Remove unnecessary access
- [ ] Document service access requirements

## Questions

Determine:

- What services need public access?
- What services should only be available internally?
- What services should require VPN access?
- Who needs access to each service?

## Example Access Model

| Service | Access Method |
|---|---|
| Proxmox | Private network / VPN only |
| Storage | Private network / VPN only |
| Game Servers | Public or VPN depending on use case |
| Website | Public internet |
| Internal Applications | VPN or authentication portal |

## Complete When

All services have a defined access method.

---

# Task 5.2 - Configure Remote Access

## Goal

Provide secure access for users outside the home network.

## Recommended Tool

### Tailscale

Purpose:

- Secure remote network access
- Device authentication
- Private connections between users and server

## Alternative Tools

Examples:

- WireGuard
- Router-based VPN

## Configuration Steps

- [ ] Create remote access account
- [ ] Install Tailscale/VPN software
- [ ] Connect server to remote network
- [ ] Add trusted user devices
- [ ] Configure access permissions
- [ ] Test remote connection
- [ ] Document connection process

## Access Examples

Remote users may access:

- File storage
- Game servers
- Remote workstation
- Internal applications

## Complete When

Authorized users can securely connect remotely.

---

# Task 5.3 - Configure User Accounts & Permissions

## Goal

Ensure users only have access to the services they need.

## Configuration Steps

- [ ] Define user roles
- [ ] Create administrator accounts
- [ ] Create standard user accounts
- [ ] Configure service permissions
- [ ] Remove unused accounts

## Example Roles

| Role | Access |
|---|---|
| Administrator | Full server management |
| Member | Shared files and approved services |
| Game User | Game servers only |

## Potential Tools

Examples:

- Proxmox user management
- Linux users/groups
- Application-level accounts
- Authentik groups

## Complete When

User access is organized and documented.

---

# Task 5.4 - Configure Authentication

## Goal

Improve account security and simplify user management.

## Possible Tools

Examples:

- Authentik
- LDAP
- Application built-in authentication
- Multi-factor authentication (MFA)

## Configuration Steps

- [ ] Select authentication approach
- [ ] Deploy authentication service if needed
- [ ] Create user accounts
- [ ] Configure groups and permissions
- [ ] Enable MFA where appropriate
- [ ] Connect supported applications
- [ ] Test user login

## Complete When

Users can securely authenticate to required services.

---

# Task 5.5 - Configure Firewall Rules

## Goal

Control communication between devices, VMs, and services.

## Tools

Examples:

- Router firewall
- Proxmox firewall
- VM operating system firewalls

## Configuration Steps

- [ ] Review existing firewall settings
- [ ] Define required traffic
- [ ] Allow required connections
- [ ] Block unnecessary traffic
- [ ] Protect management interfaces
- [ ] Document firewall rules

## Basic Rules

Examples:

- Proxmox management stays private
- Internal services only allow required access
- Public services only expose required ports
- Guest devices cannot access server resources
- VMs only communicate where required

## Complete When

Network access is intentional and documented.

---

# Task 5.6 - Secure Administrative Access

## Goal

Protect the systems used to manage the server.

## Systems To Secure

- Proxmox
- Linux VMs
- Windows workstation VM
- Network equipment

## Configuration Steps

- [ ] Change default credentials
- [ ] Create individual administrator accounts
- [ ] Limit administrator access
- [ ] Enable MFA where available
- [ ] Review SSH access
- [ ] Disable unnecessary services
- [ ] Verify management interfaces are private

## Complete When

Administrative access is restricted and controlled.

---

# Task 5.7 - Secure Web Services

## Goal

Secure services that are accessed through a web browser.

## Tool

### Caddy

Purpose:

- Reverse proxy
- HTTPS certificates
- Route traffic to internal services

## Configuration Steps

- [ ] Deploy Caddy
- [ ] Configure domains (if applicable)
- [ ] Configure HTTPS
- [ ] Route services through Caddy
- [ ] Test secure access

## Complete When

Web services can be accessed securely.

---

# Task 5.8 - Update Documentation

## Goal

Record the final security and access configuration.

## Checklist

- [ ] Update Security.md
- [ ] Update Remote Access.md
- [ ] Document user roles
- [ ] Document authentication methods
- [ ] Document firewall rules
- [ ] Document access procedures

## Complete When

Users understand how to securely access the server.

---

# Phase 5 Completion Checklist

- [ ] Service exposure reviewed
- [ ] Remote access configured
- [ ] User permissions configured
- [ ] Authentication configured
- [ ] Firewall rules configured
- [ ] Administrative access secured
- [ ] Web services secured
- [ ] Documentation updated

---

# Phase 5 Complete

The server is now accessible to users while maintaining basic security controls.

Next Phase:

**Phase 6 - Monitoring, Backups & Maintenance**
