# Remote Access

## Overview

This document describes how users will remotely access the home server and hosted services.

The goal is to provide secure access to files, applications, and services without exposing unnecessary systems to the internet.

---

# Remote Access Tools

## Tailscale

Used for secure remote network access.

Purpose:

- Access home server resources remotely
- Connect trusted devices
- Avoid exposing internal services directly

Examples:

- Access Proxmox management
- Access file storage
- Connect to internal services

---

## Parsec / Sunshine + Moonlight

Used for remote access to the Windows workstation VM.

Purpose:

- Remote DaVinci Resolve access
- Blender rendering
- GPU accelerated applications

Requirements:

- Stable internet connection
- Low latency connection
- User authentication

---

## Caddy

Used for secure access to web-based services.

Purpose:

- Provide HTTPS access
- Route traffic to hosted applications

Examples:

- Website
- Nextcloud
- Self-hosted applications

---

## File Access

Storage access may use:

- SMB for Windows file sharing
- SFTP for secure file transfers
- Nextcloud for web/mobile access

Examples:

- Upload video files
- Access project files
- Share digital assets

---

# Access Rules

General guidelines:

- Administrative access is limited
- Users only receive access to required services
- Management interfaces should not be publicly exposed
- Authentication should be enabled wherever possible

---

# Future Improvements

Potential additions:

- Multi-factor authentication
- More advanced user permissions
- Additional remote access services
