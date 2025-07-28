#Amazon 

This is a group of related feature that can be enabled on *new* S3 buckets (support request to activate on pre-existing buckets.)

This feature requires versioning to be activated. The versions are locked. 

There are two version: 

1. Retention:
	1. compliance mode: the version can't be deleted or overwritten and the retention mode or length can't change (even root)
	2. governance mode: special permissions can change settings
		 s3:BypassGovernanceRetention


2. Legal Hold:
	- no retention period
	- on or off 
	- while legal hold is on, no deletes or changes are possible

---
Links:

[[AWS Index]]
[[AWS Storage]]
[[S3 Storage Classes]]