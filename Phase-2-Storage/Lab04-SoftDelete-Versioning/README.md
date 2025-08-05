# Lab 04 – Soft Delete, Versioning & Recovery

## Objective

This lab focuses on configuring and testing soft delete, blob versioning, and recovery mechanisms within Azure Storage. The goal was to simulate overwrite and deletion scenarios and validate the platform’s built-in recovery capabilities.

## Key Concepts

- Blob soft delete
- Container soft delete
- Blob versioning
- Manual recovery and version promotion

## Tools & Services

- Azure Portal
- Azure Storage Account
- Blob Containers
- Data Protection Features

## Outcomes

- Enabled and tested blob and container soft delete with a 7-day retention
- Uploaded and overwrote a test blob to generate version history
- Viewed, restored, and promoted older blob versions
- Recovered a deleted blob using the soft delete feature
- Cleaned up resources after validating all recovery operations

## Screenshots

| #   | File Name                               | Description                                                    |
|-----|-----------------------------------------|----------------------------------------------------------------|
| 01  | `01-enable-versioning-softdelete.png`   | Enabled blob versioning and soft delete settings               |
| 02  | `02-upload-original-blob.png`           | Uploaded initial blob to simulate real data                    |
| 03  | `03-overwrite-blob-create-version.png  `| Overwrote blob to create version history                       |
| 04  | `04-view-blob-versions.png`             | Displayed available blob versions in the container             |
| 05  | `05-deleted-blob-softdelete.png`        | Blob deleted, still visible due to soft delete                 |
| 06  | `06-recover-deleted-blob.png`           | Recovered the deleted blob using undelete                      |
| 07  | `07-restore-previous-version.png`       | Restored an earlier version of the blob                        |

## Clean-Up

All blobs and containers used in the test were removed. Lifecycle protection settings remain enabled for continuity across future labs.

## Related

- **Previous Lab**: [Lab 03 – Azure Storage Lifecycle Management](../Lab03-Lifecycle-Management)
- **Next Lab**: [Lab 05 – Storage Account Failover & Replication](../Lab05-Failover-Replication)
