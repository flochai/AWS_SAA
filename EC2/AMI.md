#Amazon 


Amazon Machine Images <span class="red-text">(1 region)</span> can be created from EC2 instances or used to create EC2 instance. They contain attached permissions such as:

1. Public - everyone allowed
2. Owner 
3. Explicit - specified accounts allowed

They contain the boot volume of the instance (root volume in Linux for example) and [[Block Device Mapping]]. 

### <span class="red-text">Tips:</span>

- AMIs can't be edited. You need to create new AMI from the AMI you want to change. 
- They can be copied between regions 
- They include snapshots
 
---
Links:

[[AWS Index]]
[[EC2]]
[[Core Services]]
[[2025-07-09]]