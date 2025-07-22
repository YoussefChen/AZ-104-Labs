# Lab 6 – Conditional Access & MFA Enforcement

## Objective

Create and test Conditional Access policies to enforce MFA for specific users and block legacy authentication protocols.

---

## What Was Done

- Disabled default security settings to avoid conflicts
- Created a policy that requires MFA for the `All Sales` group
- Verified Susan was prompted to enroll and use MFA
- Created a separate policy to block legacy authentication apps
- Demonstrated granular security without affecting the whole org

---

## Key Concepts

| Term               | Meaning                                       |
|--------------------|-----------------------------------------------|
| Conditional Access | Policy-based engine for access decisions      |
| MFA                | Additional verification beyond username/pass  |

---

## Screenshots

- `01-disable-security-defaults.png`
- `02-create-ca-policy.png`
- `03-susan-mfa-prompt.png`

---

## Clean-up Instructions

- Delete both Conditional Access policies
- (Optional) Re-enable security defaults
- (Optional) Disable MFA from user settings

---

## Linked Labs

⬅️ Previous: [Lab 5 – Azure AD Roles vs Azure Roles](../Lab05-EntraID-vs-Azure-Roles/README.md)  
➡️ Next: [Lab 7 – Privileged Identity Management (PIM)](../Lab07-PIM-Role-Elevation/README.md)

---
