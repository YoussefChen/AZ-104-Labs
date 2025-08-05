# Lab 03 – Azure Storage Lifecycle Management

## Objective

This lab demonstrates how to automate blob management using Azure Storage Lifecycle Management rules. The scenario simulates cost optimization by transitioning blobs through access tiers and removing outdated data based on metadata and naming filters.

## Key Concepts

- Lifecycle Management Rules
- Blob Access Tiers: Hot, Cool, Archive
- Prefix matching and blob filters
- Automation for cost control and storage hygiene

## Tools & Services

- **Azure Portal**
- **Azure Storage (Blob Containers)**
- **Lifecycle Management (Rules Engine)**

## Outcomes

By completing this lab, I:

- Created a dedicated container for blob lifecycle testing
- Uploaded test blobs with relevant naming patterns
- Applied access tier transitions and deletion rules using Azure’s rule engine
- Simulated and validated blob transitions manually
- Cleaned up test resources and removed applied lifecycle rules

## Screenshots

| #   | File Name                          | Description                                                    |
|-----|------------------------------------|----------------------------------------------------------------|
| 01  | `01-create-archive-container.png` | New container `archivecontainer` created for testing rules      |
| 02  | `02-upload-test-blobs.png`        | Uploaded three test blobs for lifecycle simulation              |
| 03  | `03-review-hot-access-tier.png`   | Verified that blobs are in the Hot tier by default              |
| 04  | `04-create-lifecycle-rule.png`    | Created rule `archiveOldBlobs` for tier transition and deletion |
| 05  | `05-simulate-tier-transition.png` | Manually changed tier of a blob to simulate policy behavior     |


## Clean-Up

All uploaded blobs and the lifecycle management rule were deleted after testing. The storage account is retained for use in upcoming labs.

## Related

- **Previous Lab**: [Lab 02 – Shared Access Signatures (SAS)](../Lab02-SAS-StoredAccessPolicy)
- **Next Lab**: [Lab 04 – Soft Delete, Versioning & Recovery](../Lab04-SoftDelete-Versioning)
