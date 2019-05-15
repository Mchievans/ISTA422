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

4. Where are durable disks stored and what are the benefits?

5. What is required when creating a VM in Azure using the Resource Manager model?

6. What is a NIC and what does it what does it do for Azure?

7. Why should you deploy at least two instances of the VM? What is provided?

8. How many ways can you connect to your VM, and what are they?

9. Who’s responsibility is it to manage the VM?

10. What is important when determining the scale-out approach to VMs, and what model is this referred
to?