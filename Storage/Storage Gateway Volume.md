Storage Gateway is a bridge between storage that exists on premises and AWS storage. It runs as as virtual machine on premises or a hardware appliance (rarer). 
It present storage using iSCSI, NFS or SMB that integrates with EBS, S3 and Glacier. 

Storage Gateway can be used for many reasons: 

- Migrations from on-premises to AWS
- Extensions of a data center into AWS (need more storage)
- Storage Tiering
- DR
- Replacement of backup systems

Volume gateway works in 2 different modes: 

1. Volume Cached

- main location of the data is on AWS in managed S3 (main diff with stored)
- the local cache stores frequently accessed data 
- this is called data center extension 

2. Volume Stored

- like a NAS or SAN volume: can create filesystems on it
- everything is stored locally on premises (good for low latency needs)
- upload buffer has a temporary copy of the local data that is asynchronously sent to AWS as an EBS snapshot 
- good for full disk backups, migration and DR
- doesn't extend storage capacity 


---
Links:

[[AWS Index]]
[[2025-07-30]]
