#Amazon 

Cognito provides 2 main services for authentification, authorization and user management for web/mobile apps:

1. User Pools 
> the goal is a JSON Web Token or JWT which can then be used to access resources
> most AWS services can't process JWT!
> this is database of users that can include external sources
> focused on login, signup and profiles

2. Identity Pools
> the goal is to exchange an external identity for a temporary AWS compatible one 
> these identities can be from the user pool
> an IAM role configured in the identity pool is assigned to this temporary identity


![[Pasted image 20250727104303.png]]

The user pool simplifies the management of identity tokens by only using one type of token for all users, the JWT. This process allows for a near unlimited number of users which is much better than the 5000 IAM users. 

![[Pasted image 20250727104806.png]]


---
Links:

[[AWS Index]]
[[AWS Messaging]]
[[Kinesis]]
[[2025-07-27]]