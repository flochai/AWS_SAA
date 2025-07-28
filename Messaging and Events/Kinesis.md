#Amazon 

Kinesis is often confused with SQS but they are actually different in many ways. 
Kinesis is a regional public data streaming service that receives huge quantities of data from many different producers (IOT, phones, servers, EC2 instances,etc). Data is deleted after 24 hours by default but the window can be extended to 365 days for extra cost. Multiple consumers can access the data within the window. 

Streams start off with one shard which provides its own capacity of 1MB/s ingestion and 2MB/s consumption. Shards are added to the stream as needed for an extra cost. 
Kinesis Data Records (1MB) are the unit of storage that can be moved to other destinations using [[Kinesis Firehose]].

Choose Kinesis over SQS when the architecture is meant to be accessed by many different consumers and producers with data persistence. 

SQS doesn't provide persistence of messages unlike Kinesis. 


---
Links:

[[AWS Index]]
[[AWS Messaging]]
[[2025-07-27]]
[[Kinesis Firehose]]
