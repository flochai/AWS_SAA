#Amazon 

Origins are where CloudFront goes to get objects with a originfetch if the object is not available in then [[Edge Locations]]. Origins are defined in the behaviors of the distribution. 
The different categories of origins are S3, media packages, media store and everything else (custom origins). 

S3 origins are the easiest to integrate. When S3 is set as a static website, it is considered as a custom origin in CF. An S3 origin can be restricted to be only accessed by CF. 

---
Links:
[[2025-07-28]]
[[Flo/3_Areas/AWS/Infrastructure/CF/CloudFront|CloudFront]]