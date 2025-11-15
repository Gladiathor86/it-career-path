# Certifications Roadmap

This document summarizes the certifications I plan to pursue and how they fit into my overall learning path.

I do not treat certifications as a goal on their own, but as milestones that structure my learning and prove my skills in a measurable way.

---

## 1. Linux Administration

### RHCSA – Red Hat Certified System Administrator (EX200)

- Level: Entry to intermediate
- Vendor: Red Hat
- Focus:
  - Linux administration
  - filesystems and storage
  - users and permissions
  - networking basics
  - system services
- Why it matters to me:
  - Validates solid Linux fundamentals
  - Highly respected in enterprise environments
  - Good foundation for further Red Hat exams (RHCE, EX280)

Preparation plan:
- Practice on RHEL-like systems in my Home Lab
- Map my RHEL knowledge to Ubuntu/Debian concepts and vice versa
- Use:
  - official Red Hat training (if accessible)
  - good quality RHCSA courses on Udemy or similar platforms

---

## 2. Automation & Advanced Linux

### RHCE – Red Hat Certified Engineer (EX294)

- Level: Advanced
- Vendor: Red Hat
- Focus:
  - Ansible automation
  - configuration management
  - managing multiple hosts at scale
- Why it matters:
  - Proves that I can:
    - automate Linux administration tasks
    - manage complex environments
  - Strongly relevant for DevOps and SRE roles

Preparation plan:
- Build Ansible playbooks for:
  - provisioning Home Lab servers
  - installing and configuring services
- Store all Ansible work in:
  - `ansible/` folder in this repo
- Learn:
  - roles
  - handlers
  - templates
  - inventories

---

## 3. Kubernetes

### CKA – Certified Kubernetes Administrator

- Level: Intermediate to advanced
- Vendor: Cloud Native Computing Foundation (CNCF)
- Focus:
  - Cluster architecture
  - Workloads and scheduling
  - Services and networking
  - Storage
  - Troubleshooting
- Why it matters:
  - Industry standard for Kubernetes admins
  - Matches many of the skills I want to build anyway

Preparation plan:
- Build a Kubernetes lab:
  - minikube or k3s
- Practice:
  - deploying and managing resources with `kubectl`
  - debugging pods, nodes, and services
- Use:
  - Linux Foundation CKA course (if available)
  - O'Reilly / similar books and labs

### CKS – Certified Kubernetes Security Specialist

- Level: Advanced
- Vendor: CNCF
- Focus:
  - Kubernetes security
  - runtime security
  - network policies
  - RBAC best practices
- Why it matters:
  - Aligns with my DevSecOps direction
  - Validates advanced security skills in containerized environments

Preparation plan:
- Only after CKA and real practice
- Add security-specific labs to my Home Lab clusters
- Study:
  - Pod Security standards or successors
  - image scanning and admission control
  - secrets management best practices

---

## 4. Cloud & OpenShift

### EX280 – Red Hat Certified Specialist in OpenShift Administration

- Level: Intermediate
- Vendor: Red Hat
- Focus:
  - OpenShift installation and configuration
  - application deployment
  - networking and routing
  - storage
- Why it matters:
  - OpenShift is widely used in enterprise environments
  - Bridges Kubernetes skills and real-world enterprise platforms

Preparation plan:
- Learn OpenShift concepts on top of Kubernetes knowledge
- Use:
  - Red Hat training resources (if accessible)
  - free developer editions or sandboxes where possible

---

## 5. Possible Cloud Provider Certifications (Later)

I am not committing to a specific cloud provider yet, but possible paths are:

- AWS:
  - AWS Certified Cloud Practitioner
  - AWS Certified Solutions Architect – Associate
- Azure:
  - AZ-900 (Fundamentals)
  - AZ-104 (Administrator)
- GCP:
  - Associate Cloud Engineer

These will come after I stabilize my:
- Linux
- DevOps
- Kubernetes
skills and when I actively use a specific cloud in practice.

---

## 6. Strategy

- Focus on **skills first**, then certifications.
- Use:
  - Home Lab
  - real configurations
  - automation
  as primary learning tools.
- Treat certifications as:
  - goals to structure my learning
  - proof of skills for employers
  - not as a substitute for real practice
