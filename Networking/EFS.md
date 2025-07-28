The Elastic File System is the AWS implementation of NFSv4. EFS filesystems can be mounted in Linux and shared between many EC2 instances. EBS is block storage whereas EFS is file storage. 

EFS, a Linux only filesystem using POSIX permissions, is made available within a VPC via mount targets. 

- The two modes are General Purpose (default) and Max I/O (Parallel use case). 
- The two throughput modes are bursting (default) and provisioned. 
- The two storage classes available are standard and infrequent access. 

---
Links:

[[AWS Index]]