# IT Career Path – My Linux, DevOps, Cloud & DevSecOps Journey

This document is a detailed, first-person overview of my personal IT learning journey.  
It summarizes what I am studying, why, how I practice, what my goals are, and how I build real skills through my Home Lab and hands-on projects.

My focus areas:
- Linux System Administration  
- DevOps practices & automation  
- Cloud platforms  
- Kubernetes  
- DevSecOps & Zero Trust  

This document is part of my public learning portfolio.

---

## 1. Do I need a degree?

Based on research, community feedback and real job postings:  
**No, a degree is not required** to enter the Linux / DevOps / Cloud / Kubernetes world.

What truly matters:
- practical knowledge,  
- hands-on skills,  
- personal projects,  
- lab exercises,  
- and certifications.

A degree can be nice to have, but **it is not a blocker** in this career path.

---

## 2. Where I learn

These are the platforms that I use and recommend:

- **Red Hat Training** – official RHEL, OpenShift, automation content  
- **Linux Foundation** – LFCS, CKA, CKS  
- **O'Reilly Learning** – Kubernetes Patterns, Cloud Architecture  
- **Coursera / edX** – Google, Linux Foundation, IBM courses  
- **Udemy** – RHCSA, CKA, Docker, Ansible bootcamps  

I follow a hybrid model:  
formal courses → hands-on Home Lab → documentation → automation.

---

## 3. Certifications I aim for

| Level | Certification | Price | Reason |
|-------|---------------|--------|--------|
| Linux | RHCSA (EX200) | ~400–500 USD | Strong Linux admin foundation |
| Automation | RHCE (EX294) | ~600–700 USD | Ansible & automation skills |
| Kubernetes | CKA | ~395 USD | Core Kubernetes admin |
| Security | CKS | ~395 USD | Kubernetes security & hardening |
| Cloud-native | EX280 (OpenShift) | ~400–450 USD | Enterprise container platform |

These certifications define my long-term learning roadmap.

---

## 4. Career directions I target

- Linux System Administrator  
- DevOps Engineer (Junior → Medior)  
- Cloud Engineer (AWS / Azure / GCP)  
- Kubernetes Platform Engineer  
- SRE – Site Reliability Engineer  
- DevSecOps Engineer  

This repository documents my progress toward these roles.

---

## 5. Practical experience – My Home Lab

A critical part of my learning path is my personal **Home Lab**, which I use as a real-world playground to practice system administration, virtualization, networking, automation and security.

### My Proxmox Cluster
I built a full virtualization setup with:

- **3 × Lenovo M910q mini PCs** (i5-7500T CPUs)
- A complete **three-node Proxmox cluster**
- Properly configured:
  - IOMMU passthrough  
  - VM networking (bridges, subnets)  
  - NFS & SMB shares  
  - USB disk passthrough  
  - storage pools  
  - Proxmox firewall rules  

This cluster simulates the environment of a real DevOps / Cloud / SysAdmin position.

### Linux Server Experience
I actively deploy and manage:

- Ubuntu Server installations  
- SSH hardening & user management  
- journald & log rotation  
- firewall configuration  
- disk management (EXT4, UUID mounts, fstab)  
- service management through systemd  

### Containerization (Docker & Compose)
I operate several real services:

- Plex Media Server  
- qBittorrent + Gluetun VPN  
- *arr stack (Sonarr, Radarr, etc.)  
- File Browser  
- Pi-hole / AdGuard  
- Netdata monitoring  
- Various utility containers  

This provides steady practice in:
- container networking  
- resource allocation  
- logs  
- volumes  
- troubleshooting  

### Networking & VPN Testing
My environment includes:

- TP-Link Archer AX20 router (PPPoE, NAT)
- static DHCP reservations
- port forwarding for services
- Cloudflare DNS
- Tailscale Zero Trust overlay
- Twingate testing
- split-tunnel experiments

This gives me real-world experience in:
- DNS  
- routing  
- Zero Trust networking  
- VPN client/server behavior  

### Storage Administration
I manage multiple external drives:

- 4 TB + 2 TB USB disks (EXT4)
- Samba & NFS server setup  
- UID/GID alignment  
- permissions fixes  
- cross-OS compatibility  

These tasks are identical to real sysadmin challenges.

---

## 6. My Personal Learning Roadmap

### Stage 1 – Linux Fundamentals
- navigating Linux  
- permissions & ownership  
- users/groups  
- systemd services  
- networking basics  
- log management  

### Stage 2 – Virtualization & Systems
- Proxmox/KVM basics  
- VM lifecycle  
- snapshots & backup  
- cluster nodes  
- storage pools  
- Linux bridges, VLAN basics  

### Stage 3 – Docker & Compose
- containers vs VMs  
- Dockerfile writing  
- Compose multi-service apps  
- bind mounts & volumes  
- container networking  

### Stage 4 – Kubernetes
- pods, deployments, services  
- ingress controllers  
- persistent storage  
- RBAC  
- network policies  
- cluster troubleshooting  

### Stage 5 – DevOps & Automation
- Ansible for configuration management  
- GitHub Actions for CI/CD  
- Terraform (IaC)  
- versioning & branching strategies  

### Stage 6 – DevSecOps
- container scanning (Trivy)  
- runtime security (Falco)  
- Kubernetes hardening  
- Zero Trust networking  
- VPN security practices  

This structured roadmap ensures constant progression.

---

## 7. GitHub Projects I build

### Home Lab Documentation
- cluster architecture  
- network topology  
- services & containers  
- security considerations  

### Infrastructure as Code
- Ansible playbooks  
- automation scripts  
- provisioning steps  

### Kubernetes Study Projects
- k3s / minikube clusters  
- microservices deployment  
- ingress + TLS setup  
- monitoring (Prometheus + Grafana)  

### DevSecOps Exercises
- image scanning  
- workflow automation  
- security policies  

All of these projects appear in GitHub as part of my portfolio.

---

## 8. Summary

My current skills already place me between **junior and medior level** in areas like Linux, virtualization and containerization.  
My Home Lab gives me real-world, hands-on experience that many beginners don’t have.

My long-term plan is to build strong expertise in:

- Kubernetes  
- Cloud platforms  
- Automation  
- DevSecOps  

This document represents the foundation of my IT career path and will evolve as I grow.

