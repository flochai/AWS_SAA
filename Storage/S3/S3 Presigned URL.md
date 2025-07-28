#Amazon 

Presigned URLs are used to give someone else the same permissions as the creator to access a bucket without having to create any role or new identity. 

The url has the details of the request encoded in the url. 

This is particularly useful to access one particular object for a limited time. For example, an app can make a request for a presigned url for the user.

This can be used for PUT or GET request. 


Exam tips: 

- It is possible to create a presigned url for an object that you don't have access to. The permissions will stay the same though.
- TEMPORARY (--expires-in)
- This url has the same identity as the generator at that moment which means maybe we don't have access anymore because the permissions have changed. 

---
Links:

[[AWS Index]]
[[AWS Storage]]
[[S3]]
[[S3 Security]]
