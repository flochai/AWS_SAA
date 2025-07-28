#Amazon 

### 1. Vertical Scaling

- - more powerful instances are often more expensive, not proportional 
- - capped by most powerful instance
- - downtime because of instance reboot
- + if it works on an instance it will work on a more powerful instance
- + works for all applications, even monoliths 

### 2. Horizontal Scaling 

- multiple copies of the same application
- need loadbalancing
- off-host sessions (session stored in dbs)
- no limits to horizontal scaling 
- often less expensive
- more granular because each instance is a small increment compared to going for a larger instance which is generally 2x

---
Links:

[[AWS Index]]
[[EC2]]
[[2025-07-19]]
