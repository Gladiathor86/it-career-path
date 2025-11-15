# Projects Overview

This document lists and describes the key projects related to my learning journey.  
Some of them live entirely inside this repository, others may exist as separate GitHub repositories in the future.

The main idea: every project should demonstrate real skills and be reproducible.

---

## 1. Home Lab Documentation Project

Location: primarily this repository

Description:

- Full documentation of my Home Lab:
  - hardware
  - Proxmox cluster
  - storage and networking
  - services and containers
  - security practices
- Includes:
  - how I built it
  - how I maintain it
  - what I learned from issues and failures

Purpose:

- act as a reference for myself
- show real experience to potential employers
- serve as a base to experiment with automation and security

Related paths in repo:

- `docs/HomeLab_Overview.md`
- `homelab/proxmox/`
- `homelab/docker/`
- `homelab/network/`

---

## 2. Infrastructure as Code (Ansible & Terraform)

Location: `ansible/` and `terraform/` directories (to be filled as I progress)

Description:

- Ansible:
  - playbooks to:
    - configure servers
    - install services
    - apply updates
  - inventory files for my Home Lab
  - roles for reusable configurations
- Terraform:
  - initial examples for cloud resources (when I start using a specific provider)
  - infrastructure patterns that match what I do locally

Purpose:

- practice real-world DevOps workflows
- show that I can:
  - automate environments
  - keep configurations under version control
  - maintain reproducible setups

---

## 3. Kubernetes Practice Project

Location: `homelab/k3s/` and related documentation

Description:

- small Kubernetes cluster (k3s or minikube)
- experiments with:
  - Deployments, Services, Ingress
  - ConfigMaps and Secrets
  - persistent storage
  - ingress controller and TLS (later)
  - basic RBAC configurations

Potential future separate repo:
- A dedicated “k8s-lab” repository with:
  - manifests
  - Helm charts (later)
  - automation scripts

Purpose:

- prepare for CKA/CKS
- be able to operate and troubleshoot Kubernetes clusters
- link theoretical knowledge with real YAML and real deployments

---

## 4. DevSecOps & Security Testing

Location: `security/` and possibly separate repos in the future

Description:

- container image scanning workflows
- CI checks for:
  - vulnerabilities
  - outdated dependencies
- Kubernetes hardening experiments:
  - network policies
  - Pod security approaches
  - secure defaults
- documentation of:
  - Zero Trust experiments (Tailscale, Twingate)
  - DNS security
  - VPN use cases

Purpose:

- make security a natural part of the workflow
- demonstrate DevSecOps thinking
- build habits for secure defaults

---

## 5. Personal Knowledge Base & Notes

Location: `docs/` directory

Description:

- learning notes:
  - Linux administration
  - networking
  - virtualization
  - containers
  - Kubernetes
  - DevOps and DevSecOps
- certification plans and progress:
  - `docs/Certifications.md`
  - `docs/IT_Career_Path.md`
  - `docs/Learning_Roadmap.md`

Purpose:

- keep my knowledge organized
- easily revisit topics later
- provide a transparent view of my progress

---

## 6. Future Ideas

Potential future projects that may become their own repositories:

- A “Home Lab as Code” project:
  - Proxmox API usage
  - fully automated provisioning of new VMs/containers
- A full CI/CD demo:
  - app source code
  - Docker image build
  - Kubernetes deployment
  - GitHub Actions pipeline
- Cloud-specific projects:
  - when I start using AWS, Azure or GCP in a more structured way

All new projects will be linked or referenced from this document once they are created.
