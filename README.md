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

## 🔧 Setup Notes

- Configured static IPs and DHCP reservations by device type
- Used Fortinet policies to isolate guest and IoT networks
- Deployed TrueNAS for snapshots and ZFS storage pools
- Used Proxmox to host Home Assistant, Bitwarden, and Mealie
- Enabled VPN for secure off-site management

---

## 📸 Screenshots

Add your own:
- `network-diagram.png`
- TrueNAS dashboard
- Proxmox VM list
- Fortinet firewall rules

---

## License

MIT License – for documentation and educational reuse.
