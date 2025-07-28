#Amazon 

Session stickiness means that the user info is saved (logged / cart). 

When you activate session stickiness in the load balancer settings, if a user connects to a LB, a cookie is generated which locks the device to a single backend instance for a give duration (1 to 7 days). 

It is preferable to host the session into an external database because then LB can work normally. 


---
Links:

[[2025-07-24]]
[[ELB Types]]
[[Flo/3_Areas/Kubernetes/Networking|Networking]]