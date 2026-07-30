# Phase 5 - Security & Access

## Goal

Secure the server environment and establish how users will access services.

This phase focuses on protecting the server, managing users, and ensuring remote access is safe and reliable.

---

# Task 5.1 - Review Current Exposure

## Goal

Understand what services are accessible and where.

## Checklist

- [ ] Review running services
- [ ] Identify services exposed to the internet
- [ ] Identify services that should remain private
- [ ] Review open ports
- [ ] Remove unnecessary access

## Questions

Determine:

- What needs to be publicly available?
- What should only be accessible internally?
- What should require VPN access?

## Complete When

All services have a defined access method.

---

# Task 5.2 - Configure Remote Access

## Goal

Provide secure access for users outside the home network.

## Possible Tools

Examples:

- Tailscale
- WireGuard
- VPN solutions

## Checklist

- [ ] Select remote access method
- [ ] Install remote access software
- [ ] Configure user access
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

## Checklist

- [ ] Define user accounts
- [ ] Create administrator accounts
- [ ] Create standard user accounts
- [ ] Configure service permissions
- [ ] Remove unnecessary accounts

## Example Roles

| Role | Access |
|---|---|
| Administrator | Full system management |
| Member | Shared files and approved services |
| Game User | Game servers only |

## Complete When

User access is organized and documented.

---

# Task 5.4 - Configure Authentication

## Goal

Improve account security with proper authentication.

## Possible Tools

Examples:

- Authentik
- LDAP
- Built-in application authentication
- Multi-factor authentication

## Checklist

- [ ] Select authentication approach
- [ ] Configure authentication service
- [ ] Enable MFA where appropriate
- [ ] Test user login

## Complete When

Users can securely authenticate.

---

# Task 5.5 - Configure Firewall Rules

## Goal

Control network traffic between systems.

## Checklist

- [ ] Review existing firewall settings
- [ ] Allow required traffic
- [ ] Block unnecessary traffic
- [ ] Protect management interfaces
- [ ] Document important rules

## Basic Rules

Examples:

- Proxmox management stays private
- Internal services only allow required access
- Public services only expose required ports
- Guest devices cannot access server resources

## Complete When

Network access is intentional and documented.

---

# Task 5.6 - Secure Administrative Access

## Goal

Protect the systems used to manage the server.

## Checklist

- [ ] Secure Proxmox access
- [ ] Use strong administrator credentials
- [ ] Limit administrator accounts
- [ ] Review SSH access
- [ ] Disable unnecessary services

## Complete When

Administrative access is restricted and controlled.

---

# Task 5.7 - Update Documentation

## Goal

Record the final security and access setup.

## Checklist

- [ ] Update Security.md
- [ ] Update Remote Access.md
- [ ] Document user roles
- [ ] Document authentication methods
- [ ] Document access procedures

## Complete When

Users understand how to safely access the server.

---

# Phase 5 Completion Checklist

- [ ] Service exposure reviewed
- [ ] Remote access configured
- [ ] User permissions configured
- [ ] Authentication configured
- [ ] Firewall rules configured
- [ ] Administrative access secured
- [ ] Documentation updated

---

# Phase 5 Complete

The server is now accessible to users while maintaining basic security controls.

Next Phase:

**Phase 6 - Monitoring, Backups & Maintenance**
