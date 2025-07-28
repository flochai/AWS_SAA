#Amazon 

There are three types of placements groups:

1. Cluster → performance

	- pack instances close together for the highest possible performance
		- Fast direct connections because usually on the same rack and even host
		- lowest possible latency
	- all instances launched at the same time
	- single AZ
	- ⚠️ little resilience because all in same AZ and same hardware

2. Spread → HA

	- span multiple AZs 
	- separate hardware racks 
	- high resilience / HA
	- ⚠️ <span class="red-text">7 instances per AZ</span> 

3. Partition → HA+

	- similar architecture to spread but...
	- more than 7 instances per AZ
	- 7 partitions per AZ than can have many instances each
	- instances can be placed in a specific partition 


### <span class="red-text">Tips:</span>

- AMIs can't be edited. You need to create new AMI from the AMI you want to change. 

---
Links:

[[AWS Index]]
[[EC2]]
[[Core Services]]
[[2025-07-21]]