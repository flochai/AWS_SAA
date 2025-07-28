#Amazon 

1. Standard: 

	- replicated over at least 3 AZ
	- frequent access 
	- most balanced class
	- This should be the default choice unless there is a specific reason to go for another.
	- No retrieval fee

2. Standard Infrequent Access:

	- lower storage class price but there is a retrieval fee unlike standard
	- billed for a minimum of 30 days 
	- minimum capacity charge is 128KB per object

3. One-Zone Infrequent Access: 

	- cheaper than standards 
	- single availability zone instead of 3 

4. Intelligent-Tiering: 

	- changing access patterns 
	- the usage of the object is monitored and auto-moved 
	- long lived data with changing usage 

5. [[Glacier Storage Class]]

---
Links:

[[AWS Index]]
[[AWS Storage]]