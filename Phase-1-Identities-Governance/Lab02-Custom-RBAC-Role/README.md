# Lab 2 – Custom RBAC Role and Scoped Delegation

## Objective
Create a custom Azure RBAC role with limited VM read permissions and assign it to a user at the resource group level.

---

## What Was Done

- Created a new resource group: `rg-rbac-lab`
- Created a **custom role** from scratch: `Reader - Virtual Machines Only`
- Set **precise permissions** via JSON wizard
- Scoped role to `rg-rbac-lab` only
- Assigned role to `maria.it@...` from Lab 1
- Tested in Incognito to verify **read-only VM access**

---

## Screenshots
Located in `/screenshots/`:

- `01-create-resource-group.png`
- `02-create-custom-role-permissions.png`
- `03-assignable-scope.png`
- `04-assign-custom-role-to-user.png`

---

## Security Insight
Custom RBAC roles allow **surgical precision** in access control. Assigning `maria.it` to a VM-only reader role ensures:
- Least privilege
- No write/delete access
- Clean audit trail

This is vital for regulated environments, secure multi-team collaboration, and zero-trust architectures.


---

## Linked Labs
➡️ Previous: [Lab 1 – Users, Groups, and AUs](../Lab01-Users-Groups-AUs/README.md)  
➡️ Next: [Lab 3 – Built-In Roles & Role Inheritance](../Lab03-BuiltIn-Roles-Inheritance/README.md)

---
