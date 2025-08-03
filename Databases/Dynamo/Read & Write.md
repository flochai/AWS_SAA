Every operation in [[DynamoDB]] consumes at least 1 RCU or WCU. 
1 Read Con Unit is 4KB read operation per second. 
1 Write con Unit is 1KB write operation per second.

Every table has a RCU and WCU burst pool that is equal to 300 seconds of the RCU/WCU set for the table. If this pool is exceeded, an error and throttling occurs. 

### Query Operation

This is one way that data can be retrieved from the table using 1 particular key value. It is generally more cost effective to query for several items rather than 1 because of the min of 1 unit. 

<img width="1251" height="606" alt="Pasted image 20250803140200" src="https://github.com/user-attachments/assets/ec858e6f-3f74-47d7-852e-5d7775b6bf7e" />


### Scan

This is a more flexible way of obtaining data by moving through the table item by item: filtered items will be returned. It will scan through the entire table every time so the consumed capacity will be the full table. 

<img width="1247" height="589" alt="image" src="https://github.com/user-attachments/assets/cd5ef8f0-844d-4cf4-9843-dece9808198e" />

---
Links:

[[AWS Index]]
[[AWS Storage]]
