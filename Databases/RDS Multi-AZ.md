#Amazon 

### 1. Multi-AZ Instance 

A primary instance does a synchronous replication to a unique standby instance in another AZ. No access is done to the standby, only the primary instance which is reached through the database cname. Backups are done from the standby instance to improve performance of the primary. 

If the primary instance fails, the cname will switch to pointing at the standby that becomes the new primary. There can be brief (60 to 100 secs) outages because of the DNS change. 

### 2. Multi-AZ Cluster

A fast hardware writer instance replicates to two other reader instances, each in a different AZ. Writes are considered committed when 1 reader has confirmed. Failover is faster in cluster mode because done via replication logs.
You can access the cluster in different ways:

- cluster endpoint that points at the writer
- reader endpoint 
- instance endpoint (not recommended to use these / only testing and debugging)

---
Links:

[[AWS Index]]
[[2025-07-23]]