The AWS Transit Gateway is a network transit hub that connects VPCs together and to on premises network using site-to-site VPNs and DX. It's aim is to reduce network complexity. Attachements (VPC, site-to-site VPN and Direct Connect Gateway) are used to connect to other network types and even create global networks. 

Without a TGW, a HA architecture could look like this:

<img width="1240" height="590" alt="Pasted image 20250730104547" src="https://github.com/user-attachments/assets/98d0b2a7-78e7-4249-9c54-14c4910e6f8d" />

By adding a TGW within the AWS account, we eliminate the connections between the corporate office and each VPC. The TGW is a transitive device. 


<img width="1227" height="599" alt="Pasted image 20250730104853" src="https://github.com/user-attachments/assets/8a83f65c-0a6e-4213-98cf-b001e480c6ab" />


---
Links:

[[AWS Index]]
[[2025-07-30]]
