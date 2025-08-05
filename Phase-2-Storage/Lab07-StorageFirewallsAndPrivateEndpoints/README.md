# Lab 07 – Storage Firewalls, Private Endpoints & Network Access Control

## Objective

This lab demonstrates how to fully secure an Azure Storage Account by leveraging private endpoints, firewall restrictions, and virtual network integration. The goal was to isolate access to the storage account to internal Azure resources while denying all public access and enabling diagnostics for future monitoring.

## Core Concepts

- Storage account network restrictions
- Private endpoint configuration
- Virtual network integration
- Firewall rules for selected networks
- DNS configuration for private access
- Security testing from internal vs. external networks

## Key Azure Resources

- Storage Account with disabled public access
- Virtual Network with dedicated subnet
- Private Endpoint connected to storage
- Private DNS Zone
- Firewall rules allowing only internal VNet access

## Validations Performed

- Verified blob access from a VM inside the VNet
- Confirmed that external access from the internet is denied
- Enabled diagnostic logging for future monitoring

## Screenshots

- `01-create-secure-storage.png`
- `02-vnet-subnet-finance.png`
- `03-private-endpoint-created.png`
- `04-firewall-selected-networks.png`
- `05-access-success-from-vnet.png`
- `06-access-denied-from-internet.png`

## Cleanup

All resources were deployed within a dedicated resource group (`RG-SecureStorage`) and can be safely deleted if no longer needed.

---

