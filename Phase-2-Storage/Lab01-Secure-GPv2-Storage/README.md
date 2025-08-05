# Lab 1 – Secure General Purpose v2 (GPv2) Storage Account

## Objective
Deploy a secure and enterprise-compliant GPv2 Azure Storage Account using hardened configurations aligned with Zero Trust principles and storage governance best practices.

---

## What Was Done

### 🔹 Storage Configuration
- Created a General Purpose v2 (GPv2) Storage Account
- Configured region as North Europe and set redundancy to Geo-redundant storage (GRS)
- Enforced secure transfer and set minimum TLS version to 1.2
- Disabled all forms of public access and anonymous blob access

### 🔹 Governance & Protection
- Applied resource tags for `Owner`, `Environment`, and `Department`
- Enabled soft delete for blobs and containers with 7-day retention
- Added a resource lock to prevent accidental deletion

### 🔹 Networking & Encryption
- Limited access to selected networks (whitelisted client IP only)
- Ensured encryption with Microsoft-managed keys (default)

---

## Screenshots

| #   | File Name                           | Description                                  |
|-----|-------------------------------------|----------------------------------------------|
| 01  | `01-storage-account-basics.png`     | Storage account configuration – Basics tab   |
| 02  | `02-advanced-security-settings.png` | TLS and secure transfer enforcement          |
| 03  | `03-networking-config.png`          | Networking restricted to selected IPs        |
| 04  | `04-soft-delete-enabled.png`        | Soft delete for blobs and containers         |
| 05  | `05-encryption-settings.png`        | Microsoft-managed encryption configuration   |
| 06  | `06-tags-config.png`                | Tagging for resource governance              |
| 07  | `07-lock-added.png`                 | Resource lock added to the storage account   |

---

## Security Insight
This lab demonstrates how to deploy storage using a hardened-by-default approach. By combining secure network access, TLS-only enforcement, encryption, and immutability features like locks and soft delete, the configuration reflects enterprise-level compliance and reduces the risk of data exfiltration or misconfiguration.

---

## Clean-up Instructions
- Delete the resource group `RG-Storage-Secured` to clean up all resources created in this lab.

---

## Linked Labs
➡️ **Next lab**:  
[Lab 2 – Shared Access Signatures & Stored Access Policies](../Lab02-SAS-StoredAccessPolicy/README.md)

This lab laid the security groundwork that will support more granular data access control via SAS and stored access policies in the next lab.

---
