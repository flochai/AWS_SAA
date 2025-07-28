#Amazon 

When creating an ELB a DNS A record is created and points at the load balancing nodes that are deployed in each selected subnet of 2 or more AZs. 
A minimum of 8 free IPs are needed per subnet which means a /27 subnet minimum is recommended even if a /28 is technically enough.  

Configuration aspects to consider are:

- IPv4 or dual-stack? 
- Which availability zones and subnet will the LB use? 
- internet facing or internal? (affects the IPs that are given to the nodes public AND private or just private)

![[Pasted image 20250723194356.png]]

An internet facing LB can route to private AND public instances. 

---
Links:

[[AWS Index]]
