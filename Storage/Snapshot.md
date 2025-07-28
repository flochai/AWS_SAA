#Amazon 

54.173.47.156

A snapshot is a full copy of the data on an EBS stored in [[S3]] which can improve the resiliency of our EBS from AZ to region resilient. Future snaps are incremental which means they only save the difference between the previous snapshot and the current one. 

It is possible to create new EBS volumes from snaps which means they are a good way to migrate data between regions. 

Snaps restore lazily which means the data is gradually fetched when the EBS is created from a snap. You can force a read of all the data immediately using Fast Snapshot Restore (FSR).

The billing is done on the GB per month model of used data. It is possible to snapshot often because of the incremental saving. 

---
Links:

[[EBS - Elastic Bloc Store]]
[[AWS Storage]]
[[S3]]