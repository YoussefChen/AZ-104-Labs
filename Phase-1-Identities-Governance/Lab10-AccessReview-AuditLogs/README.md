# Lab 10 – Access Reviews & Audit Logs in Microsoft Entra ID


## Lab Objective

This lab focuses on implementing Access Reviews and leveraging Microsoft Entra ID audit and sign-in logs to strengthen governance, auditing, and identity security posture. These tools are critical for enforcing least privilege, meeting compliance requirements, and tracking user access lifecycle in real-world enterprise environments.

---

## Key Skills Learned

- Create and configure Microsoft Entra **Access Reviews** for group membership governance
- Simulate and approve/deny reviews as a delegated reviewer (group owner)
- Analyze **audit logs** to trace administrative actions and group changes
- Monitor **sign-in logs** for unusual login behavior or location-based anomalies
- Start a **Premium P2 trial** to unlock enterprise-level identity governance

---

## Real-World Relevance

In modern zero-trust environments, governance tools like Access Reviews and sign-in monitoring are essential to:

- Maintain **least privilege** across user and group access
- Comply with regulatory standards (e.g., ISO 27001, SOC 2)
- Automate **quarterly entitlement reviews**
- Detect **unauthorized access** and alert on risky sign-ins
- Investigate **role misuse**, lateral movement, and privilege creep

---

## Exam Relevance & Pitfalls

This lab directly supports key AZ-104 exam objectives in **Microsoft Entra identity governance**. Common pitfalls include:

- Confusing P1 vs P2 licensing: Access Reviews require **P2**
- Misunderstanding log retention: Default is **30 days**, not 1 year
- Thinking audit logs capture everything by default (they don’t include diagnostic settings)

---

## Clean-Up Performed

- Access Reviews deleted from the portal
- Temporary test users and groups optionally removed
- Microsoft Entra P2 trial allowed to expire naturally

---

## Screenshots

| #   | File Name                             | Description                                  |
|-----|---------------------------------------|----------------------------------------------|
| 01  | `01-create-access-review.png`         | Configuring the Access Review in Entra       |
| 02  | `03-audit-logs-group-changes.png`     | Audit log showing group or role changes      |
| 03  | `04-sign-in-logs-anomalies.png`       | Sign-in log anomalies from test users        |

---



