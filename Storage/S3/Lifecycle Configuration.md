#Amazon 

A lifecycle configuration is a set of rules that can affect the whole bucket or groups of objects. The rules consists of moving objects (transition actions) or deleting objects (expiration actions). The rules are not based on access, this is only in intelligent tiering. 

<span class="red-text">One Zone IA cannot transition to Glacier Instant Retrieval. </span>

If first stored in S3 standard, there is a min of 30 days before transitioning but you can start from standard-IA or intelligent tiering. 

---
Links:

[[AWS Index]]
[[AWS Storage]]
[[S3 Storage Classes]]
[[S3 Security]]
[[S3 Performance]]