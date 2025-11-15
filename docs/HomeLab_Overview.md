# Home Lab Overview

This document provides an overview of my Home Lab environment.  
It is the core platform where I practice Linux administration, virtualization, networking, containers, automation and security.

---

## 1. Goals of the Home Lab

My Home Lab is designed to:

- simulate a small, realistic infrastructure
- provide a safe place to experiment
- support learning:
  - Linux
  - Proxmox
  - networking
  - Docker and containerization
  - Kubernetes (later)
  - DevOps tools
  - DevSecOps practices

Everything I do here is reproducible and documented in this repository.

---

## 2. Hardware

Current main setup:

- 3 × Lenovo ThinkCentre M910q
  - CPU: Intel i5-7500T
  - RAM: currently mixed (8 GB and 16 GB)
  - Storage:
    - 256 GB NVMe SSD in each
    - empty 2.5" SATA bay for future upgrades
- External USB drives:
  - 4 TB (EXT4, used for media, backups, and shared data)
  - 2 TB (EXT4, used for media, backups, and shared data)

Networking:

- Router: TP-Link Archer AX20
  - PPPoE connection to ISP
  - local LAN: 192.168.0.0/24
  - DHCP with static reservations for key devices

---

## 3. Virtualization Platform: Proxmox VE

All three M910q nodes run Proxmox VE and form a cluster.

### Cluster Features

- 3-node Proxmox cluster
- Nodes:
  - `stark`
  - `hulk`
  - `thor`
- Local storage:
  - each node uses its own SSD as local storage
- External storage:
  - USB disks attached to `stark` and exported via:
    - Samba
    - NFS
- Features used:
  - web-based management
  - LXC containers
  - KVM virtual machines
  - Proxmox firewall rules

Configuration details are documented under:
- `homelab/proxmox/cluster_setup.md`
- `homelab/proxmox/storage.md`
- `homelab/proxmox/networking.md`

---

## 4. Services and Workloads

The Home Lab runs a set of real, useful services. These are primarily hosted on the media node (`stark`), but not exclusively.

### Examples of services

- Media:
  - Plex Media Server
- Download and automation:
  - qBittorrent
  - Gluetun VPN (for privacy)
  - *arr stack (Sonarr, Radarr, etc.)
- File management:
  - File Browser
  - Samba and NFS shares for Windows and Linux clients
- DNS and ad-blocking:
  - Pi-hole and/or AdGuard
- Monitoring:
  - Netdata

Most of these services are:

- containerized with Docker and Docker Compose
- or running in LXC containers
- documented under `homelab/docker/` and `homelab/`

---

## 5. Networking Overview

Main network:

- Router: TP-Link Archer AX20
  - handles PPPoE, NAT, DHCP
  - DNS: usually points to external resolvers (e.g. 1.1.1.1, 8.8.8.8) or my own DNS/filtering services
- Proxmox nodes:
  - receive static DHCP reservations
  - use Linux bridges for VM and container traffic

Additional elements:

- VPN:
  - Tailscale for secure remote access and Zero Trust experiments
  - Twingate under evaluation
- DNS:
  - Cloudflare DNS client where relevant
  - Pi-hole/AdGuard for DNS-based filtering

Networking details and setups are documented under:
- `homelab/network/`

---

## 6. Storage and Filesystems

External USB disks:

- 4 TB and 2 TB
  - formatted as EXT4
  - mounted on `stark`
  - shared via:
    - Samba (for Windows)
    - NFS (for Linux/Proxmox)
- Usage:
  - media library
  - backups
  - general storage

Key practices:

- mount by UUID
- consistent directory structure for shares
- careful permission and ownership management

---

## 7. Security and Access

- Access to Proxmox:
  - via web UI (HTTPS)
  - via SSH for CLI tasks
- No direct exposure of Proxmox UI to the public internet
- Remote access:
  - through VPN solutions (e.g. Tailscale)
- System hardening:
  - regular updates
  - limiting services to internal network where possible
  - using firewall rules on Proxmox and router

---

## 8. Documentation Strategy

All important decisions, configurations and experiments are documented in this repository, especially under:

- `homelab/`
- `docs/`
- `security/`

The Home Lab is not only a playground, but also the backbone of my portfolio and learning process.
