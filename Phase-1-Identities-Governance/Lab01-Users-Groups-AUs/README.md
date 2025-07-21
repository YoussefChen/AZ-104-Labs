# Lab 1 – Azure AD Users, Groups, and Administrative Units

## Objective
Build an enterprise-grade identity foundation in Microsoft Azure using the Azure Portal, covering:
- Azure AD user creation
- Security groups (assigned and dynamic)
- Administrative Units (AUs)
- Scoped role assignment using AUs

---

## What Was Done

### 🔹 Users
- Created 4 users: `john.hr`, `susan.sales`, `maria.it`, and `admin.hr`
- Set department field for dynamic group filtering

### 🔹 Groups
- Created an assigned security group: `HR Staff`
- Created a dynamic group: `All Sales` using department attribute
- Added members to assigned group manually and validated auto-membership in dynamic group

### 🔹 Administrative Unit (AU)
- Created `HR Department` AU
- Scoped `john.hr` and `admin.hr` under the AU

### 🔹 Scoped Role Assignment
- Assigned `User Administrator` role to `admin.hr`
- Scoped this role **only to the AU**, restricting permissions to HR-related users only

---

## Screenshots
Located in `/screenshots/`  
Recommended screenshots to include:
- ✅ Users list                      -    01-create-users.png 
- ✅ Group creation and membership   -    02-create-group-assigned.png
- ✅ Dynamic group rule              -    03-dynamic-group-rule.png
- ✅ Administrative Unit structure   -    04-au-creation.png
- ✅ Scoped role assignment screen   -    05-au-role-assignment.png	

---

## Security Insight
Scoped admin using Administrative Units enforces **least privilege** access:
- `admin.hr` cannot view or modify users outside the HR Department AU
- This mimics **real enterprise role delegation** in large orgs

This lab shows how to control lateral movement and reduce exposure in multi-admin Azure environments — a foundational skill for any cloud security engineer.

---

## Clean-up Instructions
To avoid unnecessary resource usage:
- Delete test users (`john.hr`, `susan.sales`, etc.)
- Delete groups (`HR Staff`, `All Sales`)
- Remove role assignments from AU
- Delete the Administrative Unit after removing users and roles

---

## Linked Labs
➡️ **Next lab**:  
[Lab 2 – Custom RBAC Roles and Delegation](../Lab02-Custom-RBAC-Roles/README.md)

This lab built the foundation to move into fine-grained access control using custom roles and RBAC.

---