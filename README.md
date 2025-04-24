# Network Home Lab Setup

This repo documents the architecture and configuration of my home lab, designed for hands-on learning in system administration, networking, and self-hosted services.

---

## 🧱 Lab Stack

- **Firewall**: Fortinet (FortiGate)
- **Storage**: TrueNAS Scale
- **Virtualization**: Proxmox VE
- **Media Server**: Plex (QuickSync)
- **Networking**: VLANs, VPN (WireGuard/OpenVPN), Reverse Proxy (Nginx)

---

## 🖥️ Lab Diagram

![Lab Topology](./network-diagram.png)

---

## ⚙️ Key Features

- VLANs for network segmentation (Trusted, Guest, IoT)
- Reverse proxy for remote access using Cloudflare Tunnel
- TrueNAS for secure backups and network shares
- Proxmox for running VMs and Docker containers
- FortiGate firewall for granular traffic control and VPN
- UPS for power redundancy and graceful shutdown

---

## 🧰 Tools & Services Used

Here are the key systems and apps running in my home lab:

### Core Infrastructure
- **Proxmox VE** – Virtualization platform for VMs and containers
- **TrueNAS Scale** – Network-attached storage with ZFS
- **Fortinet FortiGate** – Firewall, VPN, VLANs, and network segmentation

### Self-Hosted Applications
- **Plex** – Media server with Intel QuickSync
- **Bitwarden** – Self-hosted password manager
- **Mealie** – Recipe management system
- **Uptime Kuma** – Service monitoring and status tracking
- **Portainer** – Docker container management GUI
- **Home Assistant** – Smart home integration and automation
- **Nginx Proxy Manager** – Reverse proxy for secure remote access

### Access & Admin
- **JuiceSSH** – SSH management from mobile
- **Cloudflare Tunnel** – Secure remote access to services
- **WatchTower** – Auto-updates for Docker containers

---

## 🔧 Setup Notes

- Configured static IPs and DHCP reservations by device type
- Used Fortinet policies to isolate guest and IoT networks
- Deployed TrueNAS for snapshots and ZFS storage pools
- Used Proxmox to host Home Assistant, Bitwarden, and Mealie
- Enabled VPN for secure off-site management

---

## 🔐 Security Practices

- MFA enabled on all remote access services
- No port forwarding; remote access via Cloudflare Tunnel
- Firewall rules block VLAN-to-VLAN traffic by default
- Regular backups of Proxmox and TrueNAS configs

---

## License

MIT License – for documentation and educational reuse.
