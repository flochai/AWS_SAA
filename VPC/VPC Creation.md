The first decision point that **<span class="red-text">must</span> be decided in advance** is the CIDR range. Some questions we must answer:

1. What size should the VPC be?
2. Is there anything overlapping? 
3. What will happen in the future?
4. What structure am I giving my VPC? 

List all the IP ranges used by the organisation so you know what to avoid. 
VPC min is /28 which is 16 IPs and max is /16 which is 65536 IPs. 

> Adrian suggests 10.x.y.z and to avoid 10.0.y.z to 10.10.y.z
> Reserve 2 ranges per region per account. 


Create 4 availability zones for the VPC (3 normal + 1 extra)
Create 4 tiers (web / app / db / spare)
This means you need 16 subnets (/20)

<img width="3008" height="1692" alt="VPCStucture-1" src="https://github.com/user-attachments/assets/8da9f2f7-7ab2-486a-883a-a3a385a6cb4e" />


---
Links:

[[AWS Index]]
[[VPCs]]
[[Networking in AWS]]
[[2025-07-14]]
