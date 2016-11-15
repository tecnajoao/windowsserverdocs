---
title: Guarded fabric and shielded VMs
ms.custom: na
ms.prod: windows-server-threshold
ms.topic: article
ms.assetid: 5c7ada81-2d97-41d4-87cf-1a7ccf06cd20
manager: dongill
author: rpsqrd
ms.technology: security-guarded-fabric
ms.date: 10/14/2016
---

# Guarded fabric and shielded VMs

>Applies To: Windows Server 2016

One of the most important goals of providing a hosted environment is to guarantee the security of the virtual machines running in the environment. As a cloud service provider or enterprise private cloud administrator, you can use a guarded fabric to provide a more secure environment for VMs. A guarded fabric consists of one Host Guardian Service (HGS) - typically, a cluster of three nodes - plus one or more guarded hosts, and a set of shielded virtual machines (VMs).

> [!IMPORTANT]
> Ensure that you have installed the latest cumulative update before you deploy shielded virtual machines in production.

## Learn more about guarded fabrics and shielded VMs

- [Guarded fabric and shielded VMs overview](Guarded-Fabric-and-Shielded-VMs.md)

- [Deploying the Host Guardian Service for guarded hosts and shielded VMs](guarded-fabric-deploying-hgs-overview.md)
    - [Setting up the Host Guardian Service - HGS](guarded-fabric-setting-up-the-host-guardian-service-hgs.md)
    - [Configuration steps for Hyper-V hosts that will become guarded hosts](guarded-fabric-configure-hgs-with-authorized-hyper-v-hosts.md)
        - [Configuring the fabric DNS for hosts that will become guarded hosts](guarded-fabric-configuring-fabric-dns.md)
        - [Admin-trusted attestation for a guarded fabric - creating a security group](guarded-fabric-admin-trusted-attestation-creating-a-security-group.md)
        - [TPM-trusted attestation for a guarded fabric - capturing information required by HGS](guarded-fabric-tpm-trusted-attestation-capturing-hardware.md)
        - [Configuring a guarded fabric - confirm hosts can attest successfully](guarded-fabric-confirm-hosts-can-attest-successfully.md)
        - [Appendix A - Configure Nano server as TPM attested guarded host](guarded-fabric-configure-nano-server-as-tpm-guarded-host.md)<br><br>

- [Hosting service provider configuration steps for guarded hosts and shielded VMs](guarded-fabric-configuration-scenarios-for-shielded-vms-overview.md)
    - [Shielded VMs - Hosting service provider deploys guarded hosts in VMM](https://technet.microsoft.com/system-center-docs/vmm/scenario/guarded-hosts)
    - [Shielded VMs - Hosting service provider creates a shielded VM template](guarded-fabric-create-a-shielded-vm-template.md)
    - [Shielded VMs - Hosting service provider prepares a VM Shielding helper VHD](guarded-fabric-vm-shielding-helper-vhd.md)
    - [Shielded VMs - Hosting service provider sets up Windows Azure Pack](guarded-fabric-hoster-sets-up-windows-azure-pack.md)<br><br>

- [Tenant configuration steps for shielded VMs](guarded-fabric-tenant-configuration-steps-for-shielded-vms.md)
    - [Shielded VMs for tenants - Creating a template disk](guarded-fabric-tenant-creates-template-disk.md) (optional)
    - [Shielded VMs for tenants - Creating shielding data to define a shielded VM](guarded-fabric-tenant-creates-shielding-data.md)
    - [Shielded VMs for tenants - Deploying a shielded VM by using Windows Azure Pack](guarded-fabric-shielded-vm-windows-azure-pack.md)
    - [Shielded VMs for tenants - Deploying a shielded VM by using Virtual Machine Manager](guarded-fabric-tenant-deploys-shielded-vm-using-vmm.md)