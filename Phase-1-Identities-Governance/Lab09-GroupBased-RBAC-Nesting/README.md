# Lab 9 – Group-Based RBAC & Nested Security Groups

## Objective

Design a scalable, secure, and auditable access control model in Azure using:

- Azure role-based access control (RBAC) via Microsoft Entra security groups
- Nested group architecture to reflect enterprise team structures
- Role assignment scoped to a specific resource group (not full subscription)

This pattern is essential for real-world access design and aligns with Microsoft cloud security best practices.

---

## Why This Matters

Direct role assignments to individual users are a nightmare to manage at scale.

Group-based RBAC improves:
- Onboarding/Offboarding speed
- Least privilege enforcement
- Auditing and access reviews
- Access scalability and maintenance

---

## Lab Components

| Resource Type          | Resource Name           |
|------------------------|-------------------------|
| Resource Group         | `RG-Finance-EU`         |
| Entra Group (Child)    | `Finance-EU-Team`       |
| Entra Group (Parent)   | `Finance-EU-Leads`      |
| Users                  | `user.finance.1`, `user.finance.2`, `team.lead` |

---

## Screenshots

`01-create-finance-group.png`          
`02-nested-group-structure.png`       
`03-create-rg-finance.png`             
`04-assign-contributor-role-to-group.png` 
`05-user-finance1-success.png`      
`06-remove-user-finance1-noaccess.png` 
`07-cleanup-delete-groups.png` 
`08-cleanup-remove-rg.png`   

---

## Clean-Up Instructions

1. **Azure Portal → Resource groups → RG-Finance-EU → Delete**

2. In **Microsoft Entra admin center**:
   - Delete: `Finance-EU-Team`
   - Delete: `Finance-EU-Leads`

3. Optionally delete test users.

---

## Real-World Application

This model allows teams to scale securely:
- Add/remove users in Entra → permissions change instantly
- Nesting supports team-lead/department structures
- Contributor role at RG scope avoids overexposure at subscription level

---

