#Amazon 


CloudTrail is a ==regional== service that tracks ALL the API activity on AWS as an event and can automatically detect unusual activity with 90 days of history.

- By default, only management events are logged in trails. 
- It is possible to create an all regions trails and turn on global services tracking. 
- Organizational trails can be created as well. 
- The logs are stored in an S3 bucket as a set of compressed json files. 
- The logs can also go to CloudWatch logs.
- Data events come at an extra cost. 
- Global Service Events are logged into us-east-1, a trail must be created to capture that data. 
- CloudTrail logs take 15 minutes to create which is not real time. 

Tracks:

	What happened
	Who made the request
	When did it occur
	How was the request made (through the CLI)



---
Links:

[[AWS Index]]
[[Monitoring]]
