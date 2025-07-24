# Lab 8 – Advanced Administrative Units + Scoped Delegation

## Objective

Implement Administrative Units and assign role-based access scoped to specific user groups. This simulates real-world enterprise delegation.

---

## What Was Done

- Created two Administrative Units (FR-HR, US-Sales)
- Assigned users to their respective AUs
- Delegated `User Administrator` role to `admin.hr` (FR only)
- Validated permission boundaries via portal
- Cleaned up resources

---

## Key Concepts

| Concept                  | Description                                       |
|--------------------------|---------------------------------------------------|
| AU                       | Logical container for Entra user objects          |
| Scoped Role Assignment   | Role only works inside assigned AU                |
| Delegation               | Allows regional IT to manage local identities     |

---

## Screenshots

- `01-create-au-fr-hr.png`
- `02-create-au-us-sales.png`
- `03-add-users-to-au-fr.png`
- `04-add-users-to-au-us.png`
- `05-assign-useradmin-au.png`
- `06-edit-user-fr1-success.png`
- `07-edit-user-us1-fail.png`
- `08-assign-useradmin-us-au.png`

---

## Clean-up

- Remove users from AUs
- Delete AUs
- Remove delegated role assignments

---

## Linked Labs

⬅️ Previous: [Lab 7 – PIM & Just-in-Time Access](../Lab07-PIM-Role-Elevation/README.md)  
➡️ Next: [Lab 9 – Group-Based Access Management](../Lab09-Group-Based-Access/README.md)
