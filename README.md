# Zero Trust Infrastructure

Design and deployment of a Zero Trust infrastructure for a fictional 50-employee company, with automated provisioning, monitoring and security detection.

> Final year project (PFE), TS Réseaux et Systèmes Informatiques

## Problem
The company runs a flat network: one compromised workstation exposes every server. The goal is to segment the network, enforce strong authentication, automate deployment and detect attacks.

## Architecture
Diagram coming soon in `docs/`.

## Tech stack
| Domain | Tools |
|---|---|
| Virtualization | Proxmox VE |
| Firewall / VPN | pfSense or OPNsense, WireGuard |
| Identity | Active Directory, Authentik/Keycloak (MFA) |
| Automation | Terraform, Ansible |
| Monitoring | Prometheus, Grafana |
| Security (SIEM/IDS) | Wazuh, Suricata |

## Repository structure
- `docs/`: report notes and diagrams
- `terraform/`: VM provisioning on Proxmox
- `ansible/`: hardening and service deployment
- `scripts/`: helper scripts

## Progress
- [x] Repository created
- [ ] Lab setup (Proxmox)
- [ ] Network segmentation (VLANs, firewall)
- [ ] Identity and VPN (AD, MFA, WireGuard)
- [ ] Automation (Terraform, Ansible)
- [ ] Monitoring and SIEM
- [ ] Attack simulations and validation
