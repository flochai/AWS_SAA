#Amazon 

Simple Queue Service is a regional public AWS service that provides managed message queues. The max size for messages is 256KB, links can be sent for large data. There are two queue types:

1. Standard: best effort but messages could be received out of order
2. FIFO: maintains the order the messages were created in

Clients pull the messages which doesn't delete them, they are hidden with a VisibilityTimeout (30 second default - from 0 to 12 hours) after which the message reappears in the queue unless it was explicitly deleted. 

![[Pasted image 20250727091240.png]]

Example Video Processing Queue:

> An app on an EC2 instance in an [[ASG]] web pool receives a video from the client which is then stored in a Master video bucket. When the video is stored, a message is generated in the queue with a link to the master video. The scaling of the web pool is based on the CPU load of the EC2 instance. 
>
> The scaling of the ASG Worker Pool is based on the length of the queue. The instances from this pool pull the messages from the queue, get the videos from the link, process them and store the transcoded videos in a different bucket. If this is successful, the message is deleted. The Web Pool then sends the transcoded videos back to the client. 

The version below is a more complex system generally used in production that includes a  SNS Topic with fanout. When a master video is uploaded, the message is first added to an SNS Topic where there are different subscribers for the different sizes of transcode. This solves the issue of having just one event message and allows for independent scaling. 

![[Pasted image 20250727081721.png]]

[[Dead-Letter Queues]] are used for problem messages if they are not processed after 5 retries. 

---
Links:

[[AWS Index]]
[[AWS Messaging]]
[[Standard vs FIFO SQS Queues]]
[[2025-07-27]]