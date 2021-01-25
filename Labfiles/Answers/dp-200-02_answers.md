# DP 200 - Implementing a Data Platform Solution
# Lab 2 - Working with Data Storage

> - students will be able to determine the appropriate storage type to implement against a given ste of business an d technical requirements.
> - Be able to create Azure storage accounts and Data Lake Storage

## Exercise 1 - Choose a data storage approach in Azure
### Task 1: Identify the data storage requirements and structures of AdventureWorks

**Question 1**
AdventureWorks are in the process of transferring a web application and its logic to Azure Web Apps and require a **data store that can be used to host the static images** that are used on the website.
|||
|---|---|
|Data Store Type | Azure Storage Account. An Azure Storage Account is a type of data storage and has different technologies (configurations) An Azure storage account contains all of your **Azure Storage data objects: blobs, files, queues, tables, and disks** |
|Configuration options | Account type should be chosen as **Blobs**. The configruation options for Azure Storage Account can be found [here](https://docs.microsoft.com/en-us/azure/storage/common/storage-introduction#blob-storage) |
|Other comments	| Consider locating the Blob store in the same location as the Azuer Web App |
---
**Question 2**
AdventureWorks are in the process of building a **predictive analytics** solution. You have been asked to set up a solution that will be used to host the production environment of their work. In the first instance, you will assess what is the appropriate storage tier to create for the solution.
|||
|---|---|
|Data Store Type | Azure Data Lake Gen2 |
|Configuration options | Account type Blob, with Hierarchical Namespace enabled |
|Other comments	| Place this content close to the head office in the Nederlands |