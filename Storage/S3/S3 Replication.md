#Amazon 

CRR: Cross-Region Replication
SRR: Same-Region Replication 

The replication configuration specifies: 

1. which IAM role to use for the process
2. the destination

When replicating between different accounts, a bucket policy is required on the destination bucket to define that a role from a separate account can write into this bucket.  

## Options:

- What to replicate: all objects or filtered objects 
- what storage class will be used in the destination (same as source by default)
- ownership (same as source by default)
- replication time control: SLA / extra monitoring 

<span class="red-text">Important: </span>

- If you enable replication on a bucket that already has objects, these objects won't be replicated. You can activate batch replication to replicate existing objects. 

- Versioning must be activated. 

- Replication is unidirectional by default but can be bidirectional on request. 

- Glacier or Glacier Deep Archive can't be replicated. 

- Delete Markers are not replicated by default, this is an option. 


---
Links:

[[AWS Index]]
[[AWS Storage]]
[[S3 Storage Classes]]
[[S3 Security]]
[[S3 Performance]]