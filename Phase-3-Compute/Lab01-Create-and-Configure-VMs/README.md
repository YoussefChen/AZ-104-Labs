# Phase 3 - Lab 01: Managed Disk Configuration & Performance Tiers

## Objective

In this lab, I explored how to create and configure Azure Managed Disks for high-performance VM workloads. The goal was to understand the impact of disk types (Standard HDD, Standard SSD, Premium SSD) and performance tiers on virtual machine responsiveness and scalability.

This hands-on experience helped me grasp disk-level optimizations that are essential for real-world scenarios like database servers, high IOPS applications, and storage-cost optimization.

## Key Concepts

- Managed Disk SKUs and performance characteristics
- Attaching/detaching data disks to/from Azure VMs
- Understanding burst IOPS, throughput, and disk sizing
- Live performance tier changes on supported disks

## Screenshots

- `01-create-resource-group.png`
- `02-create-win-vm-basics.png`
- `03-win-vm-disks.png`
- `04-win-vm-networking.png`
- `05-win-vm-review-create.png`
- `06-create-linux-vm-basics.png`
- `07-validate-vms.png`
- `08-cleanup-delete-resource-group.png`

## Cleanup

All resources created for this lab were deleted, including the test VM and attached disks, to avoid unnecessary Azure charges.

---

## Navigation

- **➡️ Next Lab:** [Lab 02: Configure Availability Sets & Zones](../Lab02-Configure-Availability-Sets-Zones)_
