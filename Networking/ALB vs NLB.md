#Amazon 

Both ALB and NLB have rules that are processed in priority order. 

### 1. ALB

- listens on HTTP or/and HTTPS only
- For security, the SSL connection is broken at the loadbalancer, <span class="red-text">no SSL direct to APP</span>
- slower than NLB because there are more levels to process 
- layer 7 

### 2. NLB

- listens on TCP / UDP / TLS / TCP_UDP only
- No headers, no cookies, no session stickiness
- very fast 
- Layer 4
- NLB can have static IP
- Forward TCP to instances which means unbroken encryption

---
Links:

[[2025-07-24]]
[[ELB Types]]
[[Flo/3_Areas/Kubernetes/Networking|Networking]]