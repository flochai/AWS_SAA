#Amazon 

SCPs are policy json documents that can be attached to the root, OU or members and are used to restrict accounts. SCPs can't affect the management account. Only elements that are BOTH in the identity policies and the SCPs are allowed. 

Adrian recommends making a deny list architecture that has less admin overhead than an architecture where you deny everything and make a policy to say what is allowed. 



---
Links:

[[AWS Index]]
[[IAM]]
[[Accounts in Linux]]
[[2025-07-11]]
