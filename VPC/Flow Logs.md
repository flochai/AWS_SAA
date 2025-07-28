These *NOT REAL TIME* logs provide details about the flow of data within a VPC. They only capture metadata (IPs, ports, size), not data. They can be applied to all the ENIs of the VPC, subnet ENI or specific ENI. They can be configured to go to S3 or CloudWatch logs. 

<img width="2364" height="1132" alt="Pasted image 20250728163645" src="https://github.com/user-attachments/assets/5a79e40f-e443-434b-aae5-a838a8d5a9a9" />
<img width="2514" height="1242" alt="Pasted image 20250728163440" src="https://github.com/user-attachments/assets/e17bd9ca-cc89-4aa3-bd16-0f1a2beb99ff" />


Above we see a accept followed by a reject for the opposite traffic on the same src and dsl addresses. This generally shows that a [[SG]] and [[NACL]] are restricting the flow of traffic. 

---
Links:

[[AWS Index]]
[[VPCs]]
[[Networking in AWS]]
[[2025-07-28]]
