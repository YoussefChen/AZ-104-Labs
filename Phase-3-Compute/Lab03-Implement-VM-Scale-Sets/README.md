# Lab 03 — Implement VM Scale Sets

## Path

`Phase3-VirtualMachines/Lab03-Implement-VM-Scale-Sets`

---

## Lab Objective

Implement and configure Azure Virtual Machine Scale Sets with manual and automatic scaling policies to create resilient, scalable compute resources with rolling upgrades and health monitoring.

---

## What Was Achieved

- Created VM Scale Set with Windows Server 2022 images.
- Configured load balancing and network settings.
- Implemented rolling upgrade policy.
- Set autoscale rules based on CPU thresholds.
- Validated VM instances and autoscaling behavior.
- Cleaned up resources post-lab.

---

## Technical Highlights

| Feature                 | Purpose |
|-------------------------|-------------------------------------------------------------------------------|
| VM Scale Sets           | Group and manage identical VM instances with automatic scaling and upgrades.  |
| Rolling Upgrade Policy  | Ensures updates happen without downtime by upgrading VMs in batches.          |
| Autoscale Rules         | Automatically add or remove VMs based on CPU usage metrics.                   |
| Load Balancer           | Distributes traffic across VM instances for high availability.                |

---

## Screenshots

- `01-create-resource-group.png`  
- `02-vmss-basics-config.png`  
- `03-disks-config.png`  
- `04-networking-config.png`  
- `05-upgrade-policy.png`  
- `06-vmss-overview.png`  
- `07-instances-list.png`  
- `08-autoscale-rules.png`  

---

## Real-World Value

VM Scale Sets are fundamental in building scalable cloud infrastructure. Mastery of VMSS deployment and scaling policies is essential for cloud admins and consultants managing enterprise-grade Azure environments.

---


## Navigation

- **Previous Lab:** [Lab 02 - Configure Availability Sets & Zones](../Lab02-Configure-Availability-Sets-Zones/README.md)  
- **Next Lab:** [Lab 04 - Manage VM Extensions](../Lab04-Manage-VM-Extensions/README.md)
