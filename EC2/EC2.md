#Amazon 

**Elastic Compute Cloud *(VM instance)***

	- boot custom servers in minutes 
	- disposable 
	- IAAS (infrastructure as a service)
	- private service by default
	- billed per second or per hour depending on software launched

- EC2 is optimal for long running compute, server type applications, traditional OS, default compute service
- <span class="red-text">AZ resilient!</span> You can't cross AZ between instances or EBS. 

EC2 can have different states that influence how much is charged:

- running
- stopped (storage still being charged)
- terminated (non reversibile)


>Capital letters show the category of the machine
	T = tiny
	M = medium 
>The number is generation  
>The small letter is the processor 
    graviton (Amazon)
    intel
>The ratio between CPU and memory is the class 
	- compute: 1/2
	- generic: 1/4
	- memory: 1/8


---
Links:

[[AWS Index]]
[[Core Services]]
[[EC2 Pricing]]
[[EC2 Auto Scaling]]
[[ELB Types]]
[[AMI]]
[[2025-07-07]]