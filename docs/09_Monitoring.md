# Monitoring & Alerts

## Overview

This document describes the tools and processes used to monitor the health of the home server.

The goal is to quickly identify issues with:

- Server availability
- Resource usage
- Storage health
- Hosted services

---

# Monitoring Tools

## Uptime Kuma

Used for service availability monitoring.

Purpose:

- Check if services are online
- Track uptime
- Receive notifications when services fail

Examples:

- Website unavailable
- Game server offline
- Application not responding

---

## Grafana

Used for system dashboards and visualization.

Purpose:

- View server health
- Track performance trends
- Review historical data

Examples:

- CPU usage
- Memory usage
- Storage usage
- Network activity

---

## Prometheus

Used for collecting system metrics.

Purpose:

- Gather performance data
- Provide data for dashboards and alerts

Examples:

- VM resource usage
- System performance
- Service metrics

---

# Metrics to Monitor

## System Health

Monitor:

- CPU usage
- Memory usage
- Disk usage
- Temperatures
- Network activity

---

## Storage Health

Monitor:

- Available storage space
- Drive health
- Failed disks
- Backup status

---

## Virtual Machines

Monitor:

- VM availability
- CPU allocation
- Memory usage
- Disk usage

---

## Services

Monitor:

- Website availability
- Docker containers
- Game servers
- Remote access services

---

# Alerts

Important alerts:

- Server offline
- Service unavailable
- Storage nearing capacity
- Drive failure
- High resource usage
- Backup failure

---

# Notifications

Possible notification methods:

- Email
- Discord
- Mobile notifications

---

# Future Improvements

Potential additions:

- Automated remediation
- More detailed dashboards
- Hardware monitoring
- Additional alert rules
