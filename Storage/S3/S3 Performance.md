#Amazon 

Single PUT upload     --->      single stream of data / if fails, all data lost 

Multipart Upload:
	- data is broken up
	- each part is an isolated upload that can be restarted if it fails
	- min of 100MB
	- the transfer rate is better because of parallel uploads of the parts

[[S3 Transfer Acceleration]]



---
Links:

[[AWS Index]]
[[AWS Storage]]
