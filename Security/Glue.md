#Amazon 

Glue is a serverless ETL (Extract, Transform and Load). This is used to move and transform data between a source and destination. It crawls data sources and generates the Glue data catalog. 

The data catalog is a collection of metadata combined with search tools within a region. It improves the visibility of data across and organization. 
DATA Crawlers are given permissions and pointed at a target which they connect to in order to create metadata in the data catalog. 

Glue jobs extract data from a source, applies a script to perform a transformation and load the modified data in supported target such as S3, RDS and JDBC databases.

Glue is more cost effective than [[Data Pipeline]] and over time it should replace it. 


![[Pasted image 20250727105802.png]]

---
Links:

[[AWS Index]]
[[2025-07-27]]