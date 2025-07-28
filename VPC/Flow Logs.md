#Amazon 

These *NOT REAL TIME* logs provide details about the flow of data within a VPC. They only capture metadata (IPs, ports, size), not data. They can be applied to all the ENIs of the VPC, subnet ENI or specific ENI. They can be configured to go to S3 or CloudWatch logs. 

![[Pasted image 20250728163440.png]]
![[Pasted image 20250728163645.png]]

Above we see a accept followed by a reject for the opposite traffic on the same src and dsl addresses. This generally shows that a [[SG]] and [[NACL]] are restricting the flow of traffic. 

---
Links:

[[AWS Index]]
[[VPCs]]
[[Networking in AWS]]
[[2025-07-28]]
