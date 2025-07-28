#Amazon 

A Network Access Control List is like a stateless firewall (rules for request and response)available in a VPC that filters the inbound and outbound data of a subnet. Connections within the subnet are not affected.

Rules are processed in order, if a match occurs, the processing stops so the order of the rules is crucial. If there are no matches, the traffic is denied by default. 

A subnet can have only one NACL but the NACL can be on many subnets.

---
Links:

[[Linux]]
[[Flo/3_Areas/Linux/Networking|Networking]]
