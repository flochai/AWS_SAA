#Amazon 

When data travels long distances, it suffers high latencies and slow transfer speeds. CloudFront solves this problem. CF is a content delivery network that uses caching ([[Edge Locations]]) and an efficient global network to improve the delivery of content from its origin to its destination. A distribution is the configuration of CF with a unique domain name that ends with cloudfront.net. It is possible to use our own domain name for this. A behavior is a subconfig with a path pattern that sits between origins and distributions. There can be one to many behaviors. 

A cache hit is when the requested object is found in the Edge Location. If there is a cache miss on the Edge Location, the request moves on to the Regional Edge Cache. If the object is not there, a process called an Origin Fetch retrieves the object from the origin and puts it in the REC. The object is then cached in the REC and in the Edge Location which will provide better latency and performance. 

![[Pasted image 20250727172942.png]]


---
Links:
[[TTL & Invalidations]]
[[2025-07-27]]