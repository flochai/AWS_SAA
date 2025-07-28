#Amazon 

TTL are used to configure how long objects can be cached at [[Edge Locations]]. The default validity is 24 hours and the object is viewed as expired 24 hours after it has been cached. This can be changed in the behavior configuration along with the min and max TTL. 

Origin Headers allow us to use object specific TTL values: 

- Cache-Control max-age (seconds)
- Cache-Control s-maxage (seconds)
- Expires (Date & Time)

Cache invalidations are applied on all the Edge Locations of a distribution. This is used to expire all the objects within a chosen path. This actions has a cost so should only be used to correct mistakes. It is better to use versioned file name (\_v1 / \_v2 /\_v3) because the app will be pointing a different file which will be cached independently. 

---
Links:
[[Flo/3_Areas/AWS/Networking/CloudFront|CloudFront]]
[[2025-07-27]]