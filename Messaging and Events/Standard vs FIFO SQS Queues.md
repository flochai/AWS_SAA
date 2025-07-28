#Amazon 

1. Standard Queues

They are like multi-lane highways that scale well (near unlimited messages). Messages are delivered at least once and can be in a different order at destination. 

2. FIFO

FIFO doesn't scale well, it is like a single lane highway. With batching, there can be 3000 messages per second and 300 without.  Messages are delivered exactly once in order. The queue must have a .fifo suffix. 


![[Pasted image 20250727085902.png]]

---
Links:

[[AWS Index]]
[[AWS Messaging]]
[[SQS]]
[[2025-07-27]]
