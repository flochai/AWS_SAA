#Amazon 

Instance Store Volumes are ephemeral block storage devices that act like an emptyDir. Data on the volume is lost when the instance changes host (stop and start for example). 

>physically connected to an EC2 host
>included in the instance price
>only attached <span class="red-text">at launch time</span>, not after 

They have very high throughput. Example:

D3 = 4.6 GB/s
I3 = 16 GB/s

---
Links:

[[AWS Index]]
[[AWS Storage]]
