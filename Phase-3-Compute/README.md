# Phase 3: Manage Azure Compute Resources

## Overview
Phase 3 focused on mastering the deployment, configuration, and management of Azure Virtual Machines (VMs) and related compute services in real-world, enterprise scenarios.  
This phase went beyond basic VM creation, diving into advanced topics such as high availability, scalability, secure remote access, storage configuration, backup strategies, and automation.

By completing these labs, you’ve gained hands-on experience in **enterprise-grade Azure compute administration**, preparing you to handle diverse customer environments as a consultant.

---

## Key Concepts Covered
- **VM Provisioning & Configuration** – From scratch builds to specialized OS and disk configurations.
- **High Availability** – Implementing **Availability Sets** and **Availability Zones** for fault tolerance.
- **Scalability** – Deploying and managing **Virtual Machine Scale Sets**.
- **Automation** – Using **VM Extensions** for post-deployment configuration.
- **Disk Management** – Creating, resizing, and encrypting managed disks.
- **Secure Access** – Configuring **Azure Bastion** for RDP/SSH without public IPs.
- **Data Protection** – Implementing **VM backup and restore** with Azure Backup Vaults.
- **Security at the Network Layer** – Using **NSGs** to control inbound and outbound traffic.
- **Custom Images** – Building reusable **golden VM images** for consistent deployments.

---

## Labs Completed

### 1️⃣ Lab 01 – Create and Configure VMs  
Provisioned Windows/Linux VMs with correct networking, disks, and authentication methods.  
✅ Learned how to set proper resource naming, choose the right VM size, and secure credentials.

### 2️⃣ Lab 02 – Configure Availability Sets & Zones  
Implemented fault domain and update domain configurations for HA.  
✅ Compared benefits and limitations of Availability Sets vs. Zones.

### 3️⃣ Lab 03 – Implement VM Scale Sets  
Deployed scalable compute solutions with auto-scaling rules based on demand.  
✅ Learned to handle sudden traffic spikes and cost optimization.

### 4️⃣ Lab 04 – Manage VM Extensions  
Automated configuration with extensions like **Custom Script Extension** and **Diagnostics**.  
✅ Ensured consistent configuration across multiple machines.

### 5️⃣ Lab 05 – Configure Azure Disks  
Managed disk performance tiers, resizing, and encryption.  
✅ Explored **Standard HDD**, **Standard SSD**, and **Premium SSD** trade-offs.

### 6️⃣ Lab 06 – Implement Azure Bastion  
Secured VM access without exposing public IP addresses.  
✅ Mitigated RDP brute-force attacks via network hardening.

### 7️⃣ Lab 07 – Configure VM Backup & Restore  
Configured Azure Backup for VM protection.  
✅ Tested backup scheduling and full restore from Recovery Services Vault.

### 8️⃣ Lab 08 – Configure VM Network Security  
Created and applied **Network Security Groups (NSGs)** with fine-grained rules.  
✅ Ensured VM traffic control at subnet and NIC level.

### 9️⃣ Lab 09 – Create Custom VM Images  
Captured generalized VM images for reuse.  
✅ Enabled faster and standardized deployments across environments.

---

## Real-World Relevance
- **Consulting Engagements** – Confidently design and implement compute solutions tailored to client needs.
- **Production-Grade Operations** – Minimize downtime with proper availability and recovery planning.
- **Security-First Mindset** – Secure remote access and protect VM workloads from external threats.
- **Scalability Expertise** – Advise clients on cost-efficient scaling strategies.

---

## Navigation
⬅️ **Previous Phase**: [Phase 2 – Manage Storage Accounts & Data](../Phase2-Manage-Storage)  
➡️ **Next Phase**: Phase 4: Configure Virtual Networking
