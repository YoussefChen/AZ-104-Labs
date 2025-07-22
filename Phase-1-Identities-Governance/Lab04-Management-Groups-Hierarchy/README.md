# Lab 4 – Management Groups, RBAC Inheritance, and Policy Hierarchies

## Objective
Master role and policy inheritance across management groups, and simulate enterprise-level hierarchy and access control.

---

## What Was Done

- Enabled Management Groups and elevated admin access
- Created hierarchy: `mg-root-secure` → `mg-prod`
- Moved subscription under `mg-prod`
- Assigned Reader role to `susan.sales` at root MG → Tested inheritance
- Assigned `Allowed Locations` policy at `mg-prod`
- Confirmed policy enforcement during deployment
- Cleaned up MGs, roles, and policy

---

## Screenshots

- `01-create-mg-hierarchy.png`
- `02-assign-reader-mg-root.png`
- `03-susan-inherited-from-mg.png`
- `04-assign-policy-mg-level.png`
- `05-policy-deny-north-europe.png`

---

## Security Insight

This is how large enterprises control access and enforce security posture:
- Management Groups allow centralized, tiered control
- RBAC and Policy **flow downward**
- Avoid assigning roles at root unless necessary
- Always test inheritance and restriction behavior

---

## Clean-up Instructions

- Unassign Reader role from `mg-root-secure`
- Delete policy assignment from `mg-prod`
- Move subscription back to Tenant Root
- Delete both Management Groups

---

## Linked Labs
⬅️ Previous: [Lab 3 – Built-in Roles and Deny Assignments](../Lab03-BuiltIn-Roles-Inheritance/README.md)  
➡️ Next: [Lab 5 – Azure EntraID Roles vs Azure Roles](../Lab05-EntraID-vs-Azure-Roles/README.md)

---
