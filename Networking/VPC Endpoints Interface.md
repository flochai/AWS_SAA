Endpoint Interfaces do a similar job to gateway endpoints by providing private access to AWS public services from a VPC. They are different because: 

- They are not highly available by default as they are added to specific subnets.
- To make it HA, you need to add one endpoint in one subnet per AZ of your VPC. 
- They only support TCP and IPv4. 

They also function differently. Instead of having a prefix list, interface endpoints use DNS like normal network interfaces. PrivateDNS, enabled by default, overrides the default DNS for services.

<img width="2366" height="1212" alt="image" src="https://github.com/user-attachments/assets/c88a5472-9fa1-48b8-9c98-76c9a46b7c15" />

---
Links:

[[AWS Index]]
[[VPCs]]
[[Networking in AWS]]
[[VPC Endpoints Gateway]]
[[2025-07-29]]




