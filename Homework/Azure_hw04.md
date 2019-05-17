# Azure Homework 04

## Chapter 03 Chapter 3: Azure Virtual Machines

### Name: Malachi Evans

#### Date: May 15, 2019

-------------

1. What is Azure Blob Service?
    * Blob service gives you the ability to store files and access them from anywhere in the world by using URLs, the REST interface, or one of the Azure SDK storage client libraries
2. What do you have to do to create Azure Blob Service?
    * Create a storage account. Once you have a storage account, you can create containers, which are similar to folders, and then put blobs in the containers.
3. What are some common scenarios where file share can be used?
    * On premise applications with multiple users, sharing configurations, sharing diagnostics and metrics, sharing tools and utilities.

4. What is Locally Redundant Storage?
    * Azure Storage provides high availability by ensuring that three copies of all data are made synchronously before a write is deemed successful, These copies are stored in a single facility in a single region.

5. Describe Azure Key Vault.
    * Azure Key Vault helps safeguard cryptographic keys and secrets used by Azure applications and services by granting access to programs to the vault.
6. What is Azure Disc Encryption?
    * This feature allows you to specify that the OS and data disks used by an IaaS VM should be encrypted. For Windows, the drives are encrypted with industry-standard BitLocker encryption technology. For Linux, encryption is performed using DM-Crypt.

7. What is Client Size Encryption?
    * The data is encrypted by the application and sent across the wire to be stored in the storage account. When retrieved, the data is decrypted by the application. Because the data is stored encrypted, this is encryption at rest.

8. What are some of the things you can do with AzCopy?
    * Upload blobs from the local folder on a machine to Azure Blob storage.
    * Upload files from the local folder on a machine to Azure File storage.
    * Copy blobs from one container to another in the same storage account.
    * Copy blobs from one storage account to another, either in the same region or in a different region.

9. Name three options in the settings blade?
    * Properties, access keys, locks
10. What did you learn from reading this chapter?
    * Azure Key Vault sounds far more secure than putting a key in a congfig file and leaving it open for exposure. 
