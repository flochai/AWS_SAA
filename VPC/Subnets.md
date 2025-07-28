#Amazon 

Subnets are AZ resilient and used to add structure as well as resiliency to the [[VPCs]]. The CIDR of the subnet can not overlap with any other subnet in the VPC and must be part of the VPC CIDR range. Subnets in a VPC can communicate together by default. 

<span class="red-text">A subnet can only be in one availability zone. </span>

5 reserved IPs in every subnet:

1. First IP               --->     Network Address
2. Network +1       --->     VPC Router
3. Network +2      --->     Reserved for DNS
4. Network +3      --->     Reserved for future use 
5. Last IP               --->     Broadcast Address

---
Links:

[[AWS Index]]
[[VPCs]]
[[Networking in AWS]]
[[2025-07-09]]
