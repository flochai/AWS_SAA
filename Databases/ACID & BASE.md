#Amazon 

ACID and BASE are DB transaction models that stem from the CAP theorem (Consistency, Availability, Partition Tolerant = resilience). It is considered impossible to provide more than 2 of the three elements of CAP. 

### 1. ACID (Consistency)

Atomic -------------------------------------->  ALL or NO succeeds 
Consistent ----------------------------------->  no in between state
Isolated -------------------------------------->  not interference between transactions
Durable -------------------------------------->  once successful, transactions are saved

[[RDS]] databases are ACID models.

### 2. BASE (Availability)

BASICALLY AVAILABLE ------------------- >  no guarantee of consistency
SOFT STATE ------------------------------>  doesn't enforce consistency
EVENTUALLY CONSISTENT --------------->  reads will eventually match writes with time

The positive aspect of the BASE model is high performance and high scalability. The consistency aspect is offloaded to the applications. 

[[DynamoDB]] is both BASE and ACID. 


### <span class="red-text">Exam Tips:</span>

- If we see the term BASE = NoSQL
- ACID = RDS
- NoSQL + ACID = DynamoDB transactions

---
Links:

[[AWS Index]]
[[2025-07-22]]