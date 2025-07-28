#Amazon 

### 1. GP2 (General Purpose 2 SSD)
	 min 1 GB - max 16 TB

*IO credit = 16KB
Credit bucket = 5.4 million credits*

The credit 'bucket' has a 100 IO credits per second refill minimum.  For volumes bigger than 33.3 GB, the refill rate depends on the volume size so refill rate:

$$ 3IOPS \times GB $$

A burst rate of 3000 IOPS helps in periods of heavy load when the bucket is depleted. 

### 2. GP3 SSD

3000 IOPS & 125 MB/s of throughput by default. 
GP3 is cheaper and has a higher max throughput (1000 vs 250)



---
Links:

[[AWS Index]]
[[AWS Storage]]
[[EC2]]
[[General Storage Types]]
[[S3]]
