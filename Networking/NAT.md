#Linux 

Network Address Translation (NAT) is the process of giving a private ressource access to the public internet. This is done by remapping source or destination IPs. We can say it's a <span class="red-text">MANY to ONE</span> translation. 

[[IP Masquerading]] is a type of NAT and this is what is referred to by NAT on AWS. 

>In our architecture, we put the NAT gateway in the web public subnet and point it at the internet gateway using the route tables. The private subnet can have a default IPv4 rule in the route table to point to the NAT gateway in the web subnet. 

The NAT gateway (AZ resilient unlike Internet Gateway) keeps a record of transiting data in a translation table and then changes the source address of the packet to be its own IP. The packet is then moved to the [[Internet Gateway]] through the default route by the VPC router. The internet gateway changes the source address to be the public address of the NAT. For your architecture to be truly region resilient, you need one NAT gateway per AZ with their own route table. 

Billed per gateway per hour + data processing charge per GB. 

<span class="red-text">Exam Tips:</span>
NAT Gateways are managed, they can't be used for port forwarding or anything other than their function. They don't support SG, only NACL. 
They don't work with IPv6.

---
Links: 