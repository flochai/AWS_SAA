#Amazon 

An internet gateway is a region resilient service that is attached to a VPC and routes traffic between the VPC to the internet or the AWS public zone. A VPC can have 1 or 0 internet gateway. 

Steps:

1. Create IGW
2. Attach IGW to VPC
3. Create custom route table
4. Associate the route table with the web subnet
5. Create default routes with target as IGW
6. Allocate the IPv4 (and IPv6 if necessary) in subnet 

The public address does not touch the EC2 instances. The translation is done at the internet gateway. 

---
Links:

[[Linux]]
[[Flo/3_Areas/Linux/Networking|Networking]]
[[Egress-Only Internet Gateway]]