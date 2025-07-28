#Amazon 

There are two types of backups for RDS that are stored in S3: automated and snapshots.
They are not visible in the S3 console because they are managed by AWS directly. 

Backups are generally taken from the standby instance when they exist because of the IO pause that would stop the service of the primary. The snapshots function in increments like for EBS snaps. Automated backups are done during a defined window. 

A transaction log is saved every 5 minutes that has a retention period of 0 to 35 days. When you delete an RDS instance you are offered to create a final snapshot. 

### Restores:

When you restore from an automatic backup or snapshot, a <span class="red-text">new instance</span> is created which means the apps have to be updated with the new database endpoint (change in /var/www/html).

Restoration from a snapshot is from a single point in time (creation time) which is not optimal in case of failure whereas with automated backup, the granular replication log (5min) allows for good RPO. 

Restores aren't fast, this must be considered for the RTO (Recovery Time Objective) in case of failure. 

---
Links:

[[AWS Index]]
[[2025-07-23]]