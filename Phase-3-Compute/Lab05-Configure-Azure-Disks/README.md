# Lab 05 — Configure Azure Disks

## Path

`Phase3-VirtualMachines/Lab05-Configure-Azure-Disks`

---

## Objective

Deep-dive into Azure Managed Disks: attach, resize, format, and benchmark them while optimizing storage performance tiers, essential for scaling enterprise workloads.

---

## What Was Accomplished

- Added managed data disks to a VM.
- Initialized and formatted data disks inside Windows.
- Resized the OS disk and expanded volume.
- Performed disk performance benchmarking.
- Upgraded disk performance tier.
- Cleaned up unused disks.

---

## Key Concepts

| Feature              | Purpose                                  |
|----------------------|------------------------------------------|
| Azure Managed Disks  | Scalable, secure storage for Azure VMs.  |
| Premium SSD Tiers    | Customize disk IOPS/throughput.          |
| Host Caching         | Improve disk read/write performance.     | 
| Disk metrics         | Validate performance using `metrics`.    |

---

## Screenshots

- `01-add-disk-settings.png`
- `02-initialize-format-disk.png`
- `03-resize-os-disk.png`
- `04-disk-performance-metrics.png`
- `05-change-disk-tier.png`

---

## Real-World Relevance

Disk configuration is a **critical skill** for Azure admins and consultants. Whether designing IOPS-sensitive environments (e.g., SQL Server, SAP) or troubleshooting slow applications, knowing how to optimize and scale disk storage is non-negotiable.

---


## Navigation

- **Previous Lab:** [Lab 04 - Manage VM Extensions](../Lab04-Manage-VM-Extensions/README.md)  
- **Next Lab:** [Lab 06 - Implement Azure Bastion](../Lab06-Implement-Azure-Bastion/README.md)
