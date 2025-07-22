# Lab 7 – Microsoft Entra PIM & Just-in-Time Role Elevation

## Objective

Configure Microsoft Entra Privileged Identity Management (PIM) to assign eligible roles and require just-in-time activation with security controls.

---

## What Was Done

- Activated Microsoft Entra PIM
- Assigned `admin.hr` as *eligible* for Global Admin
- Simulated JIT activation with justification
- Configured MFA and justification as activation requirements
- Audited the elevation and revoked assignment for clean-up

---

## Key Concepts

| Term          | Meaning                                                      |
|---------------|--------------------------------------------------------------|
| PIM           | Privileged Identity Management – just-in-time role control   |
| Eligible Role | Role can be activated by user temporarily                    |
| JIT           | Just-in-Time – on-demand access with expiration              |

---

## Screenshots

- `01-entra-pim-activate.png`
- `02-assign-globaladmin-eligible.png`
- `03-activate-global-admin.png`
- `04-configure-pim-settings.png`
- `05-audit-activation-history.png`

---

## Clean-up Instructions

- Revoke eligible role from `admin.hr`
- Reset PIM role settings to default (optional)

---

## Linked Labs

⬅️ Previous: [Lab 6 – Conditional Access & MFA](../Lab06-Conditional-Access-MFA/README.md)  
➡️ Next: [Lab 8 – Administrative Units + Scoped Role Delegation](../Lab08-AU-Delegation/README.md)

---
