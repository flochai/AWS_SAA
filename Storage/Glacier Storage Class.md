#Amazon 

Glacier storage classes are used for archiving. They offer cheaper storage but more expensive retrieval costs and longer minimum delays (90 days). They also have the 3 AZ. 

1. Glacier Instant Retrieval:

	- long lived data with very infrequent data

2. Glacier Flexible Retrieval:

	 - to publicly access the object there is a retrieval process:
		 - expedited: 1-5 min
		 - standard: 3-5 hours
		 - bulk: 5-12 hours
	 - 1/6th of cost of standard
	 - good for yearly access objects 

3. Glacier Deep Archive: 
	 - cheapest class of storage
	 - minimum billable duration is 180 days 
	 - standard 12 hours retrieval
	 - bulk up to 48 hours




---
Links:

[[AWS Index]]
[[AWS Storage]]
[[S3 Storage Classes]]
[[S3 Select & Glacier Select]]