#Amazon 

Opening and closing connections takes time and consumes resources which creates latency. 

RDS proxy is a managed service running in the VPC that changes the architecture so that the applications connect to the proxy instead of the database. The proxy keeps a long term connection pool to the database open. It can be used with RDS and Aurora. 

This removes the latency of opening and closing connections since there are long term connections that can be reused. Multiplexing means less connections are needed which further reduces load. It can also reduce the failover time by over 60% for Aurora. 

---
Links:

[[AWS Index]]
[[RDS]]