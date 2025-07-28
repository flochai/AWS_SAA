#Amazon 

Dead-Letter Queues are designed to handle crashloop errors. When the maxReceiveCount is reached, the message will be moved to the queue defined in the redrive policy. An alarmed can be sent to notify the architect that a message has repeatedly failed processing. 

All SQS, including dead-letter queues, drop messages after the retention period is passed. The timestamp is not changed when the message is moved from queues! 

![[Pasted image 20250727092200.png]]

---
Links:

[[AWS Index]]
[[AWS Messaging]]
[[SQS]]
[[2025-07-27]]