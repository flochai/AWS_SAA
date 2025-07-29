A site-to-site VPN is a connection over the public internet between a VPC and an on-premise network using IPSEC for encryption. They are quick to provision (less than an hour) unlike physical connections such as [[Direct Connect]]. 

<img width="1262" height="592" alt="image" src="https://github.com/user-attachments/assets/7ebd23f0-1924-40ce-84b6-2d02ba38a429" />

The above architecture is HA from the AWS side but on the customer side there is a single point of failure that negates the HA. Below is an architecture that is HA on all sides. 

<img width="1264" height="597" alt="image" src="https://github.com/user-attachments/assets/b45530eb-3fc7-4291-8917-a94551f35580" />
