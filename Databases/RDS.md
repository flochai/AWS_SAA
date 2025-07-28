#Amazon 

Relational Database Service is not a DBaaS because you pay for and receive a <span class="red-text">database server</span>. You can have multiple databases running on one RDS. You do not have ssh or root access with the base RDS. 

Engines you can use include: 

- [[Postgres]]
- [[MySQL]]
- [[MariaDB]]
- Oracle Database 

You pick a DB subnet group that RDS can use. 

Billed for resource allocation:
1. instance size and type (like EC2)
2. Multi AZ or not
3. Per GB monthly fee depending on storage type (like EBS) 
4. data transfer per GB
5. backups and snapshots
6. Licensing if using commercial DB types like Oracle 

![[Pasted image 20250722173240.png]]

---
Links:

[[AWS Index]]
[[AWS Storage]]
[[Database Types]]
