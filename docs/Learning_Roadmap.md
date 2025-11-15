# Learning Roadmap

This document is my structured learning roadmap for Linux, DevOps, Cloud, Kubernetes and DevSecOps.

It is not a rigid plan, but a living guide. As I learn and gain more experience, I refine and extend this roadmap.

---

## 1. Foundation: Linux

Goal: Become comfortable and efficient on Linux servers without relying on a GUI.

### Topics

- Shell basics, navigation, help (`man`, `--help`)
- Filesystem layout on Linux (`/etc`, `/var`, `/home`, `/usr`, etc.)
- Permissions and ownership (`chmod`, `chown`, `umask`)
- Users and groups (`useradd`, `usermod`, `groupadd`)
- Processes and monitoring (`ps`, `top`, `htop`, `kill`, `journalctl`)
- Systemd services (`systemctl`, units, targets)
- Package management:
  - Debian/Ubuntu: `apt`
  - RHEL-like: `dnf` or `yum`
- Networking basics:
  - IP configuration
  - DNS resolution
  - `ping`, `traceroute`, `ip`, `ss`
- Basic troubleshooting

### Practice

- Use only SSH and terminal for server management
- Configure a minimal Ubuntu Server in my Home Lab
- Run and enable basic services with `systemctl`
- Document everything in this repo under `homelab/` and `docs/`

---

## 2. Virtualization & Home Lab (Proxmox, KVM, LXC)

Goal: Build and maintain a small, production-like virtualized environment.

### Topics

- Proxmox VE basics:
  - Node installation
  - Storage configuration
  - Networking (bridges, VLAN basics)
- Virtual machines:
  - Create, clone, snapshot, backup
  - Resource allocation (CPU, RAM, disk)
- LXC containers:
  - Pros and cons vs VMs
  - Typical use cases
- Cluster basics:
  - 3-node configuration
  - Node management and maintenance

### Practice

- Maintain a 3-node Proxmox cluster on Lenovo M910q mini PCs
- Run multiple servers (VMs and containers) for different roles
- Configure bridges and storage pools
- Keep a clear written record in:
  - `homelab/proxmox/cluster_setup.md`
  - `homelab/proxmox/networking.md`
  - `homelab/proxmox/storage.md`

---

## 3. Containers: Docker & Compose

Goal: Use containers as a standard way to deploy and manage services.

### Topics

- Docker basics:
  - Images, containers, networks, volumes
- Dockerfile:
  - Building custom images
  - Multi-stage builds (later)
- Docker Compose:
  - Multi-container applications
  - Environment variables and `.env` files
- Logs, resource limits, and restart policies
- Security basics:
  - Do not run everything as root
  - Minimal images

### Practice

- Run real services in containers:
  - Plex
  - qBittorrent + Gluetun
  - *arr stack
  - File Browser
  - Pi-hole / AdGuard
- Create and maintain Compose files under:
  - `homelab/docker/docker_compose/`
- Learn to troubleshoot:
  - container logs
  - network issues
  - volume permissions

---

## 4. Kubernetes

Goal: Understand and operate Kubernetes at a level that prepares for CKA and real-world clusters.

### Topics

- Core objects:
  - Pod, Deployment, ReplicaSet
  - Service (ClusterIP, NodePort, LoadBalancer)
  - ConfigMap, Secret
- Storage:
  - PersistentVolume, PersistentVolumeClaim
- Ingress and Ingress Controllers
- RBAC and ServiceAccounts
- Namespaces and multi-tenancy basics
- Networking:
  - CNI overview
  - NetworkPolicies (later)
- Troubleshooting:
  - `kubectl` basics
  - `describe`, `logs`, events

### Practice

- Build a small lab cluster:
  - k3s or minikube
- Deploy sample applications:
  - simple web apps
  - apps with persistent storage
- Configure:
  - Ingress
  - TLS with cert-manager (later)
- Document Kubernetes experiments under:
  - `homelab/k3s/`

---

## 5. DevOps & Automation

Goal: Automate repetitive tasks and adopt Infrastructure as Code practices.

### Topics

- Version control with Git and GitHub
- CI basics with GitHub Actions:
  - triggers
  - jobs
  - steps
- Ansible:
  - inventory
  - playbooks
  - roles
- Terraform (later):
  - providers
  - basic IaC structure

### Practice

- Use this repo as the main GitHub project for my journey
- Create:
  - simple CI workflow under `.github/workflows/ci.yml`
  - Ansible playbooks under `ansible/playbooks/`
  - basic Terraform examples under `terraform/examples/`
- Automate:
  - server provisioning
  - basic configuration tasks

---

## 6. DevSecOps & Security

Goal: Integrate security into the workflow from the beginning.

### Topics

- Container security:
  - image scanning (e.g. Trivy)
  - keeping images up-to-date
- Kubernetes security:
  - RBAC best practices
  - network policies (later)
  - secrets management
- Zero Trust networking:
  - Tailscale
  - Twingate
- VPN concepts and DNS security

### Practice

- Scan images used in the Home Lab
- Apply basic hardening steps on containers and servers
- Experiment with Zero Trust tools in the Home Lab
- Document security notes under:
  - `security/`

---

## 7. Long-term goals

- Be comfortable managing Linux systems in production-like environments
- Build, operate and troubleshoot:
  - Proxmox clusters
  - containerized services
  - small Kubernetes clusters
- Use automation tools daily (Ansible, CI/CD, IaC)
- Move toward professional roles:
  - DevOps
  - Cloud
  - DevSecOps

This roadmap will evolve as my skills improve and as new tools and technologies appear.
