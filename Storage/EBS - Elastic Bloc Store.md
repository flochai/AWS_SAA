#Amazon 

EBS is a **persistent** <span class="red-text">AZ resilient</span> AWS network block storage that can only be attached to [[EC2]]. It can be different storage types, performant profiles and sizes. 

EBS can be multi-attached to several instances (managed by a cluster app) but by default we have to consider it as attached to one instance at a time. It can be mounted and unmounted between instances.

It is possible to create a [[Snapshot]] of the backup of an EBS volume which will be stored in S3. This is useful to migrate data between availability zones.

The volume can be unencrypted or encrypted with [[Key Management Service (KMS)]]. 

It is billed on a GB per month model.

![[EBS.png]]

---
Links:

[[AWS Index]]
[[AWS Storage]]
[[EC2]]
[[General Storage Types]]
[[S3]]
[[EBS Encryption]]
