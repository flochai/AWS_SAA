#Amazon 

Origin Access Identities are different from IAM Roles and Users but share similarities. They are associated with CF distributions which become this OAI. The identity can be used in the S3 bucket policies which is set to deny all but the OAI (implicit deny). This means that users won't be able to directly access the resources in the bucket. 

To secure custom origins, OAI can't be used. We can use: 

1. Custom Headers + HTTPS only


- ns-77.awsdns-09.com
- ns-1335.awsdns-38.org

---
Links:
[[2025-07-28]]
[[ACM]]