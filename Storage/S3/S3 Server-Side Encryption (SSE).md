#Amazon 

Client-Side Encryption: data is encrypted before upload
Server-Side Encryption: uploaded in plain text and encrypted by the server. 

Object encryption is mandatory at rest. There are 3 types available: 

1. Server-Side Encryption with Customer-Provided Keys (SSE-C)

	 *The customer provides the keys and manages the encryption and decryption process. AWS never sees the object in plaintext form. 

2. Server-Side Encryption with Amazon S3-Managed Keys (SSE-S3): default

	*Only the object is provided, S3 handles everything for encryption without our control. The algorithm used is AES256. This method is not suitable if you need to control the keys.* *There is no role separation.* 
 
3. Server-Side Encryption with KMS Keys (SSE-KMS) 

	*KMS manages the keys which gives us more control than SSE-S3. This method is good because of isolated permissions which means that only the person who has permissions for the KMS key can see the data. Even an S3 administrator would not see the data if they don't have the KMS permissions. 


---
Links:

[[AWS Index]]
[[AWS Storage]]
[[Key Management Service (KMS)]]
