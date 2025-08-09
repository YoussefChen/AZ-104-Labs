# Lab07 - Configure VM Backup and Restore

This lab focuses on setting up enterprise-grade backup and disaster recovery for Azure virtual machines. The objectives included creating a Recovery Services vault, defining backup policies, enabling and performing backups, and restoring VMs from backup points. This hands-on exercise aimed to deepen understanding of backup configurations, retention settings, and disaster recovery strategies critical for cloud administrators in real-world consulting environments.

## Key Concepts

- Recovery Services Vault: Centralized resource to manage backup and recovery.
- Backup Policy: Defines schedule and retention settings for VM backups.
- On-Demand Backup: Allows immediate creation of recovery points.
- Restore Operation: Recover a VM to a previous state to ensure data availability.
- Disaster Recovery: Ensuring business continuity through backups.

## Real-World Relevance

In enterprise environments, maintaining reliable backups and swift restore capabilities is essential for disaster recovery and minimizing downtime. Azure Backup offers scalable, secure VM protection without complex infrastructure, making it a key responsibility for cloud administrators and consultants managing client environments.

## Lab Objectives

- Create and configure a Recovery Services vault.
- Define and assign a custom backup policy.
- Enable backup for a VM and trigger on-demand backups.
- Restore a VM from a recovery point and validate connectivity.

---

## Screenshots

- `01-create-recovery-vault.png`  *(after creating Recovery Services vault)*
- `02-backup-policy-config.png`  *(during custom backup policy setup)*
- `03-backup-enabled.png`        *(backup enabled on VM overview page)*
- `04-on-demand-backup.png`       *(after triggering an on-demand backup)*
- `05-restore-config.png`         *(restore VM configuration screen)*
- `06-restore-job-status.png`     *(restore job progress overview)*
- `07-restored-vm-overview.png`   *(restored VM overview in Azure Portal)*
- `08-rdp-or-ssh-connection.png`  *(successful connection to restored VM)*

---

## Navigation

- **Previous Lab:** [Lab06 - Implement Azure Bastion for secure VM access](../Lab06-Implement-Azure-Bastion/README.md)
- **Next Lab:** [Lab08 - Configure VM Network Security](../Lab08-Configure-VM-Network-Security/README.md)
