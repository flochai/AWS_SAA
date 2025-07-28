#Amazon 

KMS is a regional and public service that creates, stores and manages symmetric and asymmetric cryptographic keys. The keys <span class="red-text">NEVER</span> leave KMS or the region. [[Multi-Region Keys]] can be created.

KMS keys support rotation (changing of the encryption every year). 
Security standard: FIPS 140-2 (L2)

KMS is very granular with permissions which means that permissions are required for every action like decrypting or encrypting. <span class="red-text">Every</span> key has a key policy that is a type of [[Resource Policy]]. 

By default, KMS is max 4KB in size but [[DEKs]] can be used for more. 

---
Links:

[[AWS Index]]
[[Flo/3_Areas/Kubernetes/Networking]]
[[Accounts in Linux]]
[[2025-07-12]]
