# Network Support Engineer LAB Practical:

## Mikrotik CHR Firewall & RADIUS Lab

This repository documents a complete hands-on lab involving Mikrotik CHR, VirtualBox, Winbox firewall configuration, RADIUS setup using Ansible, and hotspot configuration.

The project is executed step-by-step with configuration files, screenshots, and automation artifacts for clarity and reproducibility.

## Project Status
- Phase 1: VirtualBox & CHR setup – Completed
- Phase 2: Firewall configuration – Completed
- Phase 3: Ansible & RADIUS – In progress

## Phase 1 – Mikrotik CHR Setup on VirtualBox

- Installed Oracle VirtualBox and Extension Pack
- Imported Mikrotik CHR image
- Configured network adapter to obtain IP via DHCP
- Verified MAC addresses of ether1 and ether2
- Confirmed CHR accessibility

All configuration evidence is provided under:
`Screenshots/Phase-1-VirtualBox/`

## Phase 2 – Firewall Rule Configuration

- Accessed Mikrotik CHR using Winbox via MAC address
- Configured firewall rule to block TCP 443 traffic to destination 1.1.1.1
- Verified rule placement and action

Screenshot:
`Screenshots/Phase-2-Firewall/Firewall.png`

## Phase 3 – RADIUS Configuration Using Ansible

- Installed and configured Ansible on Ubuntu 24.04 using WSL
- Integrated WSL with VS Code for playbook development
- Created an Ansible inventory file (`hosts`) with Mikrotik CHR connection parameters
- Developed an Ansible playbook (`RADIUS.yml`) to configure a RADIUS client on Mikrotik CHR
- Successfully executed the playbook and validated task execution

Screenshot of Ansible execution:
`Screenshots/Phase-3-Ansible/Ansible.png`

## Phase 4 – RADIUS Verification via Winbox

- Verified RADIUS client configuration through Winbox
- Confirmed RADIUS server address, secret, and hotspot service association
- Ensured configuration applied as intended by Ansible automation

Verification screenshot:
`Screenshots/Phase-4-RADIUS/RADIUS.png`
