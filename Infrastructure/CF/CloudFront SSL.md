#Amazon 

It is possible to have:

1. HTTP or HTTPS
2. HTTPS only
3. HTTP redirected to HTTPS

Two connections are opened when a client makes a request: 

client ---> CF
CF ------> destination

Both of these connections need public certificates (self-signed certificates don't work). 

---
Links:
[[2025-07-28]]
[[ACM]]