# Lab 02 — Configure Availability Sets & Availability Zones

## Path

`Phase3-VirtualMachines/Lab02-Configure-Availability-Sets-Zones`

---

## Lab Objective

This lab demonstrates the design and deployment of highly available Virtual Machine infrastructure using both **Availability Sets** and **Availability Zones** within Azure. The goal is to simulate real-world scenarios where enterprise applications demand fault tolerance and minimum downtime through zone-aware and domain-aware VM architecture.

---

## What Was Achieved

- Provisioned an **Availability Set** to distribute VMs across fault and update domains.
- Deployed two Windows VMs (`AVSet-VM1`, `AVSet-VM2`) within the same availability set to avoid single points of failure in a data center.
- Used **Availability Zones** to distribute two additional VMs (`Zone-VM1`, `Zone-VM2`) across separate physical locations within the West Europe region.
- Verified zone and domain placement using the Azure Portal.
- Compared SLA guarantees between both approaches and documented real-world applicability.

---

## Technical Highlights

| Feature               | Purpose                                                                                                             |
|-----------------------|---------------------------------------------------------------------------------------------------------------------|
| **Availability Sets** | Ensures redundancy at the compute cluster level by separating VMs across fault/update domains.                      |
| **Availability Zones**| Provides higher resiliency by physically isolating resources in separate data centers within the same Azure region. |
| **Fault Domains**     | Protect against hardware failures.                                                                                  |
| **Update Domains**    | Protect against platform-initiated maintenance events.                                                              |

---

## Screenshots Included

- `01-create-resource-group.png` — Resource group creation for the lab scope.
- `02-create-availability-set.png` — Availability Set configuration with 2 FDs and 5 UDs.
- `03-create-vm1-in-availability-set.png` — VM1 configured in availability set.
- `04-create-vm2-in-availability-set.png` — VM2 also added to the same availability set.
- `05-availability-set-instances.png` — Verification of VM placement across domains.
- `06-create-zone-vm1.png` — VM deployed into Availability Zone 1.
- `07-create-zone-vm2.png` — VM deployed into Availability Zone 2.
- `08-zone-validation.png` — Validation of VM zone placement in the Azure Portal.

---

## Real-World Value

Knowing how to architect and deploy resources using Azure Availability Sets and Zones is critical for real-world Azure administration roles. This knowledge ensures uptime guarantees and prepares environments for failover scenarios. This lab simulates the foundational infrastructure design decisions expected from a cloud consultant or administrator working with enterprise clients.

---

## Navigation

- **Previous Lab:** [Lab 01 - Create and Configure VMs](../Lab01-Create-and-Configure-VMs/README.md)  
- **Next Lab:** [Lab 03 - Implement VM Scale Sets](../Lab03-Implement-VM-Scale-Sets/README.md)
