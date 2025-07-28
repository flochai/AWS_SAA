#Amazon 

This is a real time data processing data service using SQL. Its destinations are [[Kinesis Firehose]], [[Lambda]] and [[Kinesis]]. A Kinesis Analytics App processes data between a source stream and a destination stream. The sources are not modified, the in-application input streams (like database copies of the stream) are modified along with extra data from reference tables.

This is an expensive service that should be used only if real-time SQL processing is needed for real time dashboards such as leaderboard in games or metrics for security or response teams. 

![[Pasted image 20250727101310.png]]


---
Links:

[[AWS Index]]
[[AWS Messaging]]
[[Kinesis]]
[[2025-07-27]]