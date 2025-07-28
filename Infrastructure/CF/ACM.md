#Amazon 

The AWS Certificate Manager is a regional service that can function as a public or private CA to generate or import certificates. ACM can automatically renew certificates if they are generated using it. If the certificate is imported, it must be renewed by the owner. 
Certificates can only be deployed out to supported services such as [[Flo/3_Areas/AWS/Networking/CloudFront|CloudFront]] or ALBs (Not EC2). 

Certificates can't leave the regions they were generated or imported in and they have to be located in the same region than the service they are being used in. A cert in us-east-1 can only work with an ALB in us-east-1. CF certificates must be in us-east-1 from an ACM perspective, even though CF is global. 

![[Pasted image 20250727185038.png]]

---
Links:
[[Flo/3_Areas/AWS/Networking/CloudFront|CloudFront]]
[[2025-07-27]]