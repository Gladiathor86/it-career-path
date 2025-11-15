# IT Career Path – My Linux • DevOps • Cloud • DevSecOps Journey

Ez a repository a saját IT karrierutamat, a tanulási jegyzeteimet és a Home Lab projektem teljes dokumentációját tartalmazza.  
A célom egy olyan átlátható, folyamatosan bővülő tudásbázis összeállítása, amely bemutatja, hogyan építem fel a Linux, DevOps, Kubernetes és Cloud irányú tudásomat valós projekteken keresztül.

---

##  Tartalom

- **docs/** – Átfogó dokumentációk  
- **homelab/** – A saját Proxmox alapú Home Lab rendszerem részletes leírásai  
- **ansible/** – Automatizálási feladatok és példák  
- **terraform/** – Infrastructure as Code példák  
- **security/** – DevSecOps fókuszú jegyzetek, konténer és cluster biztonság

---

##  Kiindulópont: Miért hoztam létre ezt a repót?

Szeretném dokumentálni:
- a tanulási folyamatomat,
- a saját Home Lab környezetem konfigurációját,
- az automatizálási megoldásaimat,
- a felkészülésemet különböző IT vizsgákra,
- és azt, hogyan építek fel egy piacképes DevOps / Cloud / DevSecOps tudást.

Ez a repo egyben szakmai portfólió is.

---

##  Karrier irányok, amiket célzok

- Linux System Administrator  
- DevOps Engineer (Junior → Medior)  
- Cloud Engineer (AWS / Azure / GCP)  
- Kubernetes Platform Engineer  
- SRE – Site Reliability Engineer  
- DevSecOps Engineer  

---

##  Tanulási Roadmap (rövid összefoglaló)

### 1. Linux alapok
- fájlrendszerek  
- jogosultságok  
- systemd  
- csomagkezelők  
- hálózati alapok  

### 2. Virtualizáció (Proxmox, KVM, LXC)
- háromnode-os Proxmox cluster  
- storage, networking, tűzfal  
- USB passthrough, VM-ek, snapshotok  

### 3. Docker & konténerek
- Compose stackek  
- image optimalizálás  
- konténerizált szolgáltatások üzemeltetése  

### 4. Kubernetes
- k3s / minikube cluster  
- Deploy, Service, Ingress  
- storage, RBAC, hálózati szabályok  

### 5. DevOps eszközök
- GitHub Actions  
- Ansible  
- Terraform  

### 6. DevSecOps
- Trivy, Falco  
- Kubernetes hardening  
- Zero Trust & VPN (Tailscale, Twingate)  

A részletes dokumentációk a **docs/** és **homelab/** könyvtárakban találhatók.

---

##  Home Lab (Proxmox Cluster)

- 3 × Lenovo M910q mini PC (i5-7500T)
- teljes Proxmox cluster  
- NFS + SMB storage  
- Docker és LXC konténeres környezet  
- Plex, qBittorrent, Gluetun, *arr stack  
- File Browser, Pi-hole, Netdata  
- Cloudflare DNS, Zero Trust tesztelés  

Részletes beállítások:  
 `homelab/proxmox/`  
 `homelab/docker/`  
 `homelab/network/`

---

## 🛠 Automatizálás (Ansible / Terraform)

- szerverek provisioningje  
- rendszerfrissítések  
- szolgáltatások telepítése  
- IaC példák cloud platformokhoz  

---

##  DevSecOps fókusz

- container scanning  
- k8s security  
- Zero Trust networking  
- VPN + DNS biztonság  

---

## Célok

- RHCSA, RHCE, EX280  
- CKA, majd CKS  
- AWS / Azure cloud vizsgák  
- teljes Home Lab automatizálása  
- GitHub Action alapú CI/CD pipeline-ok  
- saját Kubernetes szolgáltatások  

---

##  Kapcsolat

Ez a repo személyes projekt, folyamatosan bővítem.  
Külső megkereséshez: *GitHub Issues / Discussions* használható.

---

Köszönöm, hogy megnézted a repót!  
A fejlődési folyamatom naprakészen követhető itt GitHubon.
