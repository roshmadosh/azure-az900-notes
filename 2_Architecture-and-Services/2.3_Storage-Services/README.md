### Compare Azure storage services
The Azure Storage platform offers several services, all of which are accessible by HTTP/HTTPS and client libraries, and encrypt the data their storing.  

1. Blob storage: unstructured data, like AWS S3.
2. Azure Files: file shares accessible by Server Message Block (SMB) or Network File System (NFS) protocols.
3. Queue storage: for messages.
4. Disk storage: disk storage for Azure VMs.  

### Describe storage tiers
Storage tiers are configuration parameters you can define at the resource or account level that indicate the frequency with which you access your data.  
- Hot access tier: For frequent access. Lowest cost for reads for highest cost for storage.
- Cold access tier: For storage accessed roughly once a month.  
- Archive access tier: For storage accessed roughly once a year. Lowest cost for storage, highest cost for reads.  

### Describe redundancy options
1. Locally Redudant (LRS): Three copies in a single data center. 11-nines durability (99.999999999%) over a year.
2. Zone Redundant (ZRS): Replicated across three AZ in your primary region. 12-nines durability. 
3. Geo-redundant (GRS): LRS in two data centers that are in region pairs (i.e. a primary and secondary region). 16-nines durability.
4. Geo-zone Redundant (GZRS): ZRS in the primary region and LRS in secondary region. 16-nines durability.  
5. Read-Access GRS, Read-Access GZRS: Allows reads from secondary region even if primary region is up and running.  

• Describe storage account options and storage types
### Identify options for moving files, including AzCopy, Azure Storage Explorer, and Azure File Sync
**AzCopy** is a command line tool for moving files to and from locally, between storage accounts, and even between cloud service providers. You can also synchronize files (uni-directionally) so that all files saved in a source location gets moved to a target location automatically.  

**Azure Storage Explorer** is a GUI that uses AzCopy under the hood to do the same things.  

**Azure File Sync** can be installed locally and allows for bi-directional file synchronization.  

### Describe migration options, including Azure Migrate and Azure Data Box
**Azure Migrate** is a migration service that helps assess a migration prior to it happening, as well as does the migrating over a network.  
**Azure Data Box** is for migrating data offline. Suitable for migrating data over 40TB and you have little or no network capabilities. They send you an actual hard drive that they transport back to a data center.  

