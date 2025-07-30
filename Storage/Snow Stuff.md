
Snowball, Snowball Edge and Snowmobile are services used to move large amounts of data IN and OUT of AWS with physical storage: suitcase or truck. It can be ordered empty, loaded up and returned to AWS or with Data, empty and return. Any data that is stored is encrypted using KMS. 

### 1. Snowball

The capacity of one Snowball is 50TB or 80TB. It is interesting to use Snowball if the amount of data tot be transferred is between 10TB and 10PB. This service only includes storage, no compute. 

### 2. Snowball Edge 

This is like snowball but includes compute, faster networking and the capacity is larger. There are three types:

1. Storage Optimized (with EC2): 
> 80 TB, 24 vCPU, 32 RAM, 1TB SSD with EC2

2. Compute Optimized:
> 100 TB, 7.68 NVME, 52 vCPU, 208 RAM

3. Compute with GPU (same as above)

### 3. Snowmobile

The snowmobile is a portable data center in a shipping container on a truck. This is not economical for multi-site or for sub 10PB. 


---
Links:

[[AWS Index]]
[[2025-07-30]]
