#Amazon 


An IAM policy is a document in json format that gives permissions like a role in K8s. It specifies the resource we are performing an action on and the action. It is possible to attach policies to identities ([[IAM Groups]], users or roles). 

It is important to be aware of overlapping actions in the same OR multiple policies.
Priorities:

1. Explicit Deny 
2. Explicit Allow 
3. Default Deny (implicit)

A policy can be:
1. inline - unique to each identity it is provided to
2. managed - attach to multiple identities  

If you modify a managed policy it will apply to all the connected identities. It should be used to give rights to a large number of identities. 
Inline policies will be given for exceptional access rights to give more or less rights for specific users. 



---
Links:

[[AWS Index]]
[[IAM]]
