# Lab 09 – Create Custom VM Images

## Path
`Phase3-VirtualMachines/Lab09-Create-Custom-VM-Images`

---
## Lab Objective

Create a reusable, generalized VM image from a fully configured base VM and deploy a new VM from that image. Explore Managed Images and the Shared Image Gallery (SIG) for enterprise distribution and versioning.

---

## What Was Achieved

- Deployed a base VM (`BaseImageVM`) and prepared it with software and configuration to serve as a golden image.
- Generalized the Windows VM using **Sysprep** and captured a **Managed Image** (`BaseImageManaged`).
- Deployed a new VM (`CustomImageVM`) from the captured managed image to validate the image.
- (Advanced) Demonstrated the creation of a **Shared Image Gallery**, created an image definition and version, and discussed replication for multi-region scenarios.
- Cleaned up test resources (optional) to avoid lingering costs.

---

## Technical Highlights / Key Concepts

- **Generalized Image vs Specialized Image**
  - *Generalized*: Run `sysprep` (Windows) or `waagent -deprovision` (Linux) to remove machine-specific information — suitable for scaling and sharing.
  - *Specialized*: Captures VM as-is (keeps identity) — useful for migration, not for template reuse.
- **Managed Image**
  - Snapshot-like resource representing a reusable OS disk and optional data disks.
- **Shared Image Gallery (SIG)**
  - Enterprise-grade image distribution with versioning, replication and RBAC support.
- **Image Versioning & Replication**
  - Use SIG to publish image versions and replicate them to other regions for fast, consistent VM deployment.
- **Licensing**
  - Verify OS licensing (Azure Hybrid Benefit / marketplace images) before creating/distributing images.

---

## Screenshots (take these at the exact moments indicated)

1. `01-basevm-basics.png`  *Capture the VM creation Basics tab filled in (name, image, size, credentials).*  
2. `02-basevm-disks.png`  *Capture the Disks tab showing the OS disk type selection.*  
3. `03-basevm-networking.png`  *Capture the Networking tab showing the VNet and Public IP settings.*  
4. `04-software-installed.png`  *Inside the VM, show installed software (IIS, or your app) and desktop indicating preparation complete.*  
5. `05-sysprep-generalize.png`  *Inside the VM, Sysprep dialog (before clicking “OK”) showing `/generalize /oobe /shutdown`.*  
6. `06-capture-image.png`  *Azure Portal : Capture VM dialog with image name `BaseImageManaged` and option to delete VM after capture.*  
7. `07-create-vm-from-image.png`  *Azure Portal : Create VM from `BaseImageManaged` (show creation form with custom image selected).*  
8. `08-shared-image-gallery.png` *(optional, advanced)*  *Shared Image Gallery overview showing image definition and version replication settings.*  

---

## Real-World Relevance

- Golden images (aka “golden AMIs” in AWS) are a standard in enterprise environments: they ensure **consistency**, **security baseline compliance**, and dramatically **speed up provisioning** during scale-outs or migrations.
- Consultants use images to bake common software and configurations (monitoring agents, security hardening, corporate certificates, baseline apps) so teams don’t repeat manual setup.
- Shared Image Gallery is essential for multi-region enterprises and for maintaining image **version control** and **auditable distribution**.

---

## Practical Notes & Gotchas

- Always **generalize** a Windows VM with Sysprep before capturing. Failing to do so produces images that cause duplicate SID issues or activation/licensing problems.
- If a VM is domain-joined, remove it from the domain before generalizing or use a specially prepared process.
- Shared Image Gallery replication can take time. Plan image publishing for maintenance windows.
- Verify any vendor or MSFT licensing implications before sharing images externally or across subscriptions.

---


## Navigation

- **Previous Lab:** [Lab 08 – Configure VM Network Security](../Lab08-Configure-VM-Network-Security/README.md)  
- **Next Lab:** End of Phase 3 (no next lab)

