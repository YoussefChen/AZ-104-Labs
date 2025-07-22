# Lab 5 – Azure Entra ID Roles vs Azure Roles

## Objective

Understand the difference between identity-level roles (Entra ID roles) and resource-level roles (Azure RBAC), and how they apply across scopes.

---

## What Was Done

- Assigned **User Administrator** (Entra ID role) to `susan.sales`
- Verified Susan could manage users but not Azure resources
- Assigned **Contributor** (Azure RBAC role) at RG level
- Verified Susan could now manage RG
- Removed both roles and cleaned up access

---

## Role Comparison Table

| Role Type           | Scope          | Used For                         |
|---------------------|----------------|----------------------------------|
| Entra ID Role       | Tenant-wide    | User/group/device management     |
| Azure RBAC Role     | Sub/RG/Res     | VM, storage, network management  |

---

## Screenshots

- `01-assign-user-admin.png`
- `02-susan-user-creation-ok.png`
- `03-susan-no-rg-access.png`
- `04-assign-contributor-rg.png`
- `05-susan-can-manage-rg.png`

---

## Security Insight

Always separate duties:
- Give **Entra ID roles** to Identity Admins
- Give **Azure roles** to Infrastructure Admins
Never give both unless absolutely necessary.

---

## Clean-up Instructions

- Remove Entra ID role from `susan.sales`
- Remove Contributor role at RG
- Delete RG if unused

---

## Linked Labs

⬅️ Previous: [Lab 4 – Management Groups and Role Inheritance](../Lab04-Management-Groups-Hierarchy/README.md)  
➡️ Next: [Lab 6 – Azure AD Conditional Access and MFA](../Lab06-Conditional-Access-MFA/README.md)

---
