#Amazon 

There are three ways a LB handles SSL connections: 

1. Bridging (default)

The connection is terminated on the ELB which means a certificate is needed. This can be problematic for high security requirements. ELB then reencrypts the data and creates a new SSL connection towards the backend. The EC2 instances also need certificates and a lot of compute is used for the cryptographic operations.

1. Pass-through

The Network load balancer listens on TCP, doesn't do any decryption and just passes the data along to the backend. This is more secure because AWS never sees certificates. EC2 still use compute to decrypt.

1. Offload

Clients connect to the ELB with https, connections are terminated and then it transits to the backend with http. The EC2 instances don't do any cryptographic operations which reduces compute. 


---
Links:

[[2025-07-24]]
[[ELB Types]]
[[Flo/3_Areas/Kubernetes/Networking|Networking]]