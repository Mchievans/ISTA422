# Azure Homework 03

## Chapter 03 Chapter 3: Azure Virtual Machines

### Name: Malachi Evans

#### Date: May 15, 2019

-------------

1. What is Azure Virtual Machines and the terminology used in the chapter to reference?
    * an instance of an actual compute node

2. How do you stop an Azure VM, and give an example?
    * to Stop but the VM is still deployed to a physical host **Stop-AzureRmVM -Name "AzEssentialDev3" -ResourceGroup "AzureEssentials" -StayProvisioned**
    * to stop and deallocate resources in the Azure CLI **azure vm stop azure vm deallocate**
3. What are three main resource providers used when working with Azure Virtual Machines, Storage,
and Compute?
* The Network resource provider (Microsoft.Network) handles all aspects of network connectivity such as IP addresses, load balancers, NICs, and so on.
* The Storage resource provider (Microsoft.Storage) handles the storage of the disks for a VM (in the context of Azure Virtual Machines).
* The Compute resource provider (Microsoft.Compute) handles details related to the VM itself, such as naming, operating system details, and configuration (size, number of disks, and so on).

4. Where are durable disks stored and what are the benefits?
    * The disks can be mounted as drives on the VM and the benefits of blob storage are high availability, durability, and geo-redundancy options.

5. What is required when creating a VM in Azure using the Resource Manager model?
    * it is required that the VM be placed within an Azure Virtual Network (VNET) and whether it will be used in an existing VNET (or create a new one).

6. What is a NIC and what does it what does it do for Azure?
    * a network interface card provides network access to resources in an Azure virtual network,

7. Why should you deploy at least two instances of the VM? What is provided?
    * To avoid a single point of failure. Azure provides an SLA (service level agreement) 99.95 percent connectivity for multiple-instance only when two or more VMs are deployed into an availability set.

8. How many ways can you connect to your VM, and what are they?
    * Two ways, either remotely or by configuring network access to allow other programs or services to communicate with the VM.

9. Who’s responsibility is it to manage the VM?
    * The User.

10. What is important when determining the scale-out approach to VMs, and what model is this referred
to? 
* Virtual Machine Scale Sets (VMSS) and configuring autoscale rules relatively easily using the ARM template or Azure portal.