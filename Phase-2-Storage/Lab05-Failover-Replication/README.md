# Lab 05 – Storage Account Failover & Replication

## Objective

This lab focuses on designing and validating Azure Storage replication and failover capabilities to simulate disaster recovery scenarios. The aim was to test GRS, RA-GRS, and RA-GZRS configurations and validate data durability and high availability across regions.

## Key Concepts

- Geo-redundant storage (GRS)
- Read-access geo-redundant storage (RA-GRS)
- Geo-zone-redundant storage (RA-GZRS)
- Manual storage account failover
- Regional disaster simulation and verification

## Tools & Services

- Azure Portal
- Azure Storage Accounts
- Blob Containers
- Geo-replication & Configuration blade

## Outcomes

- Deployed storage accounts with GRS and RA-GRS configurations
- Observed secondary replication regions and health metrics
- Manually triggered and validated a regional failover
- Verified data durability post-failover
- Optionally tested RA-GZRS to ensure multi-zone and multi-region redundancy
- Removed all resources post-verification

## Screenshots

| #   | File Name                               | Description                                                       |
|-----|-----------------------------------------|-------------------------------------------------------------------|
| 01  | `01-create-RA-GRS-storage-account.png`  | Created GRS-based storage account                                 |
| 02  | `02-upload-blob-to-backupdata.png`      | Uploaded test blob to a replication container                     |
| 03  | `03-geo-replication-status.png`         | Viewed primary and secondary replication region details           |
| 04  | `05-initiate-storage-failover.png`      | Triggered storage account failover                                |
| 05  | `06-post-failover-primary-confirmed.png`| Confirmed new primary region and blob data integrity              |



## Clean-Up

All storage accounts and containers created during the replication and failover tests were deleted. Configuration settings may persist in diagnostics history.

## Related

- **Previous Lab**: [Lab 04 – Soft Delete, Versioning & Recovery](../Lab04-SoftDelete-Versioning-Recovery)
- **Next Lab**: [Lab 06 – Shared Access Signatures (SAS) for Secure Access](../Lab06-Shared-Access-Signatures)
