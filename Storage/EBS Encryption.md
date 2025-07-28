
There is no encryption by default but at rest encryption can be put in place using KMS. This is a free service. 

A unique DEK is created by KMS for each volume (and snapshots + further EBS vols from snapshot) and loaded in the EC2 instance that encrypts the data before sending it to the volume. 

Encryption is not reversible. 


---
Links:

[[AWS Index]]
[[AWS Storage]]
[[EC2]]
[[General Storage Types]]
[[EBS Encryption]]