#Amazon 

Aurora is a managed database service spread across 3 different AZs that is very different from RDS. It uses the cluster model including a primary instance and 0 or more replicas that can be used for read operations. The cluster has shared SSD storage (max 128TB) spread out over 6 replicas that are spread across the AZs associated with the cluster. 

Multiple endpoints are available: 

1. Cluster Endpoint
2. Reader Endpoint (load-balanced across the readers)
3. Custom Endpoints

Features:

- Backtrack: in place rewinds to a previous point in time 
- Fast Clones: make a new database much faster than copying all the data

### Pricing:

- Storage is billed on the highest storage you used (high water mark). If you need to reduce storage costs, a brand new cluster needs to be made. 
- Compute: hourly charge per second. 
- 100% DB size in backups are included in the paid charge. 

Aurora has better value than RDS. 

---
Links:

[[AWS Index]]
[[AWS Storage]]
