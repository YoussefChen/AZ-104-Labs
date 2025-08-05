# Lab 02 – Shared Access Signatures (SAS) & Stored Access Policies

## Objective

This lab demonstrates how to securely delegate time-limited and permission-restricted access to blob data in Azure Storage. The focus is on generating Shared Access Signatures (SAS) and configuring Stored Access Policies to simulate real-world access control scenarios without exposing storage account keys.

## Key Concepts

- Service-level SAS vs. account-level SAS
- Stored Access Policies and centralized access control
- Secure, temporary access to blob data
- Real-world testing of SAS URLs via incognito sessions

## Tools & Services

- **Azure Portal**
- **Azure Storage (Blob service)**
- **Shared Access Signature (SAS)**
- **Stored Access Policies**

## Outcomes

By completing this lab, I:

- Created a private blob container for secure file access
- Uploaded a sample blob and generated a read-only SAS token
- Validated SAS access using incognito mode
- Created a stored access policy for permission expiry control
- Regenerated a SAS token linked to the policy and tested access
- Practiced cleanup to maintain a tidy Azure environment

## Screenshots

| #   | File Name                               | Description                                             |
|-----|-----------------------------------------|---------------------------------------------------------|
| 01  | `01-create-container.png`               | Blob container `publicdocs` created with private access |
| 02  | `02-upload-blob.png`                    | Uploading `confidential.txt` to the container           |
| 03  | `03-generate-service-sas.png`           | Creating service-level SAS with read-only access        |
| 04  | `04-validate-sas-url.png`               | Verifying SAS access via incognito browser              |
| 05  | `05-create-stored-access-policy.png`    | Stored access policy `readonlypolicy` configured        |
| 06  | `06-generate-sas-with-policy.png`       | SAS generated using the stored policy                   |
| 07  | `07-test-sas-policy-url.png`            | Testing the policy-bound SAS URL                        |

## Clean-Up

The `publicdocs` container and all blobs were deleted after validation. The storage account was retained for continuity with upcoming labs.

## Related

- **Previous Lab**: [Lab 01 – Secure GPv2 Storage Account](../Lab01-Secure-GPv2-Storage)
- **Next Lab**: [Lab 03 – Azure Storage Lifecycle Management](../Lab03-Lifecycle-Management)
