#Amazon 

It is often *not* recommended to run a database directly on EC2 but it is possible if the db does not function on AWS provided db services. There can also be a demande for a specific OS/DB combination. 

Reasons to not put databases on EC2:

1. admin overhead because of managing the EC2 
2. complicated backups and disaster recovery 
3. EC2 is on a single AZ which means failure of the AZ puts the database in danger
4. lack of features / performance compared to the db products offered by AWS
5. hard to scale the EC2 in this situation 

The business should be able to justify well why they want to run the database on EC2 for it to be a good plan. 

---
Links:

[[AWS Index]]
[[AWS Storage]]

