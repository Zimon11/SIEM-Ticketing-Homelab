⬅️ [Previous: Introduction](01-introduction.md) | [Next: Installation ➡️](03-installation.md)

# 🏗️ Lab Architecture

## Overview
The set-up include SIEM(Wazuh) and Ticketing system(Osticket) installed both on Ubuntu Server in
a Virtual Machine using Hyper-V. The Ubuntu server was also in the same network as the Domain Controller. The devices IT-PC01 and the DC-01 has a Wazuh Agent installed in the both of them to monitor their logs.

---

## Architecture Components

### SIEM and Ticketing System Server
#### Operating System:
- Ubuntu
#### Software Installed:
- Wazuh
- Osticket
#### Functions: 
- Monitoring Logs
- Creating Tickets
#### IP Configuration:
- Static IP
---

### Endpoint 1(Wazuh Agents)
#### Operating System:
- Windows 11
#### Role:
- Domain-joined client computer
#### IP Configuration:
- DHCP (Router)
#### DNS Configuration:
- Points to Domain Controller IP

### Endpoint 2(Wazuh Agents)
#### Operating System:
- Windows Server 2025
#### Role:
- Domain Controller
#### IP Configuration:
- Static
#### DNS Configuration:
- Points to Domain Controller IP
---

### Virtualization Platform
#### Hypervisor:
- Hyper-V
#### Virtual Machines:
- Ubuntu Server
- Windows Server 2025 (Domain Controller)
- Windows 11 (Client)
#### Network Type: 
- External Virtual Switch
---

⬅️ [Previous: Introduction](01-introduction.md) | [Next: Installation ➡️](03-installation.md)

