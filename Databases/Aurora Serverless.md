#Amazon 

Aurora Serverless uses the concept of capacity units (ACU) with a min and max per cluster. It has the same resilience as Aurora Provisioned (6 copies across AZs).

Best used for:
- infrequently used applications or websites
- new applications because unsure of load
- variable workloads 
- unpredictable workload
- development and test because no ACU charge when paused
- multi-tenant applications
### Pricing:
Billed for the amount of ACU used and the cluster storage. 

---
Links:

[[AWS Index]]
[[AWS Storage]]
