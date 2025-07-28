#Amazon 

They are read only replicas of the primary instance that have their own endpoint. They replicate asynchronously and can even be used for cross-region replication. 

It is possible to create 5 read replicas per DB instance which is a good way to scale read performance. Read-replicas can have there own read-replicas but this creates lag issues because of the asynchronous replication. Read replicas can help meet low RTOs in different ways:

- read-replicas can be promoted to normal instances quickly in case of failure 
- they are good for global resilience 

---
Links:

[[AWS Index]]
[[2025-07-23]]