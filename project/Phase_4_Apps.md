# Phase 4 - Service Deployment

## Goal

Deploy the applications and services that will run on the virtual machines.

This phase turns the server from a collection of VMs into a functional home server environment.

---

# Task 4.1 - Prepare VM Environments

## Goal

Ensure each VM is ready for application deployment.

## Checklist

- [ ] Confirm all VMs are online
- [ ] Apply operating system updates
- [ ] Install required dependencies
- [ ] Confirm network connectivity
- [ ] Confirm storage access
- [ ] Verify administrative access

## Complete When

All VMs are ready to receive applications.

---

# Task 4.2 - Deploy File Storage Services

## Goal

Set up centralized storage for shared files and digital assets.

## Purpose

Storage will be used for:

- Video files
- Creative projects
- Digital assets
- Shared files
- Backups

## Checklist

- [ ] Configure storage folders
- [ ] Set permissions
- [ ] Configure file sharing
- [ ] Test local access
- [ ] Test remote access (if required)

## Possible Tools

Examples:

- SMB
- NFS
- Nextcloud
- SFTP

## Complete When

Users can reliably access shared storage.

---

# Task 4.3 - Deploy Docker Services

## Goal

Create the application environment for self-hosted services.

## Checklist

- [ ] Install Docker
- [ ] Configure Docker Compose
- [ ] Create application folders
- [ ] Deploy initial containers
- [ ] Confirm container health

## Initial Services

Potential deployments:

### Caddy

Purpose:

- Reverse proxy
- HTTPS certificates
- Web traffic routing

---

### Authentik

Purpose:

- User authentication
- Identity management
- Application access control

---

### Monitoring Tools

Purpose:

- Service health checks
- Resource visibility

Examples:

- Uptime Kuma
- Grafana
- Prometheus

## Complete When

The Docker environment can run and manage services.

---

# Task 4.4 - Deploy Website Hosting

## Goal

Create the environment for hosting websites or web applications.

## Checklist

- [ ] Configure web server
- [ ] Configure domain access (if applicable)
- [ ] Configure HTTPS
- [ ] Test external access
- [ ] Document deployment process

## Possible Tools

Examples:

- Caddy
- Nginx
- Docker containers

## Complete When

The website environment is operational.

---

# Task 4.5 - Deploy Game Servers

## Goal

Configure dedicated game servers for users.

## Initial Games

- Arma
- Project Zomboid

## Checklist

- [ ] Install required server software
- [ ] Configure server settings
- [ ] Configure ports
- [ ] Test multiplayer connections
- [ ] Document server management

## Considerations

Review:

- CPU usage
- RAM usage
- Storage requirements
- Number of players

## Complete When

Game servers are accessible and stable.

---

# Task 4.6 - Configure Remote Workstation Software

## Goal

Make the Windows VM usable as a remote creative workstation.

## Checklist

- [ ] Install GPU drivers
- [ ] Install DaVinci Resolve Studio
- [ ] Install Blender
- [ ] Configure remote access software
- [ ] Test GPU performance

## Possible Tools

Examples:

- Sunshine + Moonlight
- Parsec
- Remote Desktop

## Complete When

Users can remotely access the workstation and complete workloads.

---

# Task 4.7 - Configure User Access

## Goal

Provide users access to the services they need.

## Checklist

- [ ] Create user accounts
- [ ] Configure permissions
- [ ] Test user access
- [ ] Remove unnecessary access

## Example Access

| User Type | Access |
|---|---|
| Admins | Full management |
| Project Members | Shared resources |
| Friends | Game servers |
| External Users | Approved services only |

## Complete When

Users can access required services.

---

# Task 4.8 - Document Deployed Services

## Goal

Keep documentation updated as services are added.

## Checklist

- [ ] Update Services.md
- [ ] Record service locations
- [ ] Record access methods
- [ ] Record credentials location
- [ ] Document configuration changes

## Complete When

The documentation reflects the current server state.

---

# Phase 4 Completion Checklist

- [ ] Storage services deployed
- [ ] Docker environment deployed
- [ ] Website hosting configured
- [ ] Game servers running
- [ ] Remote workstation configured
- [ ] User access configured
- [ ] Services documented

---

# Phase 4 Complete

The server is now functional and providing its intended services.

Next Phase:

**Phase 5 - Security, Access & Hardening**
