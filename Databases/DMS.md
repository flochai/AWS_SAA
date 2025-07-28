#Amazon 

The Database Migration Service allows us to move external databases to [[Amazon Aurora]]. It starts with an EC2 instance that replicates data between source and destination endpoints. 

There are three types of jobs:

1. Full Load (one off migration of all data)
2. Full Load + Change Data Capture (CDC)
3. CDC Only (only data changes are replicated)

DMS does not convert schemas the [[SCT]] does this. 

---
Links:

[[AWS Index]]
[[RDS]]
[[Amazon Aurora]]