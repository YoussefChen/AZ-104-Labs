# Lab 06 — Implement Azure Bastion

## Path

`Phase3-VirtualMachines/Lab06-Implement-Azure-Bastion`

---

## Objective

Deploy Azure Bastion to enable secure, browser-based RDP/SSH to VMs, without exposing public IPs or opening ports.

---
the 
## What Was Accomplished

- Created required `AzureBastionSubnet`
- Deployed Azure Bastion in the target VNet
- Connected to a VM using portal-based web RDP
- Removed public IP from VM for secure isolation

---

## Key Concepts

| Feature        | Details                              |
|----------------|--------------------------------------|
| Bastion Host   | Secure RDP/SSH via Azure Portal      |
| Subnet Naming  | Must be named `AzureBastionSubnet`   |
| Public IP SKU  | Requires **Standard SKU**            |
| Billing Model  | Hourly-based, charged even when idle |

---

## Screenshots

- `01-create-bastion-subnet.png`
- `02-deploy-bastion.png`
- `03-bastion-connect.png`
- `04-remove-public-ip.png`

---

## Real-World Relevance

Azure Bastion is an **enterprise-ready** jumpbox replacement. Organizations aiming for zero-trust architecture rely on Bastion to avoid exposing RDP/SSH. Mastery here is expected from modern Azure admins and consultants.

---


## Navigation

- **Previous Lab:** [Lab 05 - Configure Azure Disks](../Lab05-Configure-Azure-Disks/README.md)  
- **Next Lab:** [Lab 07 - Configure VM Backup & Restore](../Lab07-Configure-VM-Backup-Restore/README.md)
