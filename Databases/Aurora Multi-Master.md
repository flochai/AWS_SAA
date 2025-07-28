#Amazon 

Unlike the default single-master mode for Aurora that has only one write replica, multi-master clusters can read/write from all replicas. It has the same structure but no endpoints. Applications can communicate with any of the 2 masters. 
The replications is done to the storage volumes but also between masters. 
Failover is more efficient because if one of the writer fails, it will immediately route to the other writer. 

---
Links:

[[AWS Index]]
