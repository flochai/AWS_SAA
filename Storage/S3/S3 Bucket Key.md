#Amazon 

[[Key Management Service (KMS)]] is limited in the number of key actions it can do per second. This can present issues if there are many requests to put objects in buckets as each object needs a DEK which creates an API call to KMS.  

To address this issue, a temporary bucket key can be generated to avoid soliciting KMS for each putobject. This bucket key will then create the DEK for each object for a time. This reduces costs and improves scalability. 


---
Links:

[[AWS Index]]
[[AWS Storage]]
[[S3]]
[[S3 Security]]
