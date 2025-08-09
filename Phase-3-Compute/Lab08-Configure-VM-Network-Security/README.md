# Lab08 - Configure VM Network Security

## Key Concepts

- Network Security Groups (NSGs) regulate traffic to and from VM NICs and subnets.
- Inbound and outbound security rules control allowed ports, protocols, and sources.
- Just-In-Time (JIT) VM Access reduces attack surface by opening ports only on demand.
- NSG Flow Logs provide traffic visibility for security monitoring and troubleshooting.

## Real-World Relevance

Effective network security is essential in enterprise environments to protect VMs against unauthorized access and threats. JIT access and NSG monitoring are industry best practices to balance security and operational flexibility. Cloud administrators regularly configure and audit these settings to maintain compliance and minimize risks.

## Lab Objectives

- Configure inbound and outbound NSG rules for VM security.
- Enable and test JIT access to securely open VM ports.
- Set up NSG flow logs for traffic monitoring.
- Understand and troubleshoot common network security issues.

---

## Screenshots

- `01-vm-overview.png`          *(VM overview page)*
- `02-vm-networking.png`        *(VM Networking blade)*
- `03-nsg-overview.png`          *(NSG overview page)*
- `04-nsg-inbound-rule.png`      *(Adding inbound security rule)*
- `05-nsg-outbound-rule.png`     *(Adding outbound security rule)*
- `06-jit-configuration.png`     *(JIT access configuration)*
- `07-nsg-flow-logs.png`         *(Enabling NSG flow logs)*

---

## Navigation

- **Previous Lab:** [Lab07 - Configure VM Backup and Restore](../Lab07-Configure-VM-Backup-Restore/README.md)  
- **Next Lab:** [Lab09 - Create Custom VM Images](../Lab09-Create-Custom-VM-Images/README.md)
