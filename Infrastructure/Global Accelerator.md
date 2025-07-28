#Amazon 

The global accelerator is a service that optimizes the flow of data from the user to the AWS infrastructure. Both GA and CF are used to move the AWS network closer to customers but have different benefits. 

Anycast IP addresses are used to have the same IPs in different [[Edge Locations]] so that users can be routed to the closest IP to them using the public internet. The data that arrives to the Edge location is then routed directly to where is needs to go instead of hopping around like a mad bunny. 

CF moves the data to edge locations close to the user (caching) whereas GA routes traffic from the Edge Location to the AWS infrastructure. CF only caches HTTP/S content. GA transits data using TCP and UDP (but doesn't do caching). 

---
Links:
[[2025-07-28]]
