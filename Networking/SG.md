#Amazon 

Security Groups are stateful which means they automatically allow response traffic. 
⚠️  They can't explicit DENY, <span class="red-text">only ALLOW</span> or implicit DENY which means <span class="red-text">they can't block</span> specific bad actors which is why NACLs are used together with SG. ⚠️ 

SG are attached to ENI (Elastic Network Interfaces) not to instances. 


---
Links:

[[NACL]]