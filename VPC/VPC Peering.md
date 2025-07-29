
VPC Peering is a service that allows us to create a direct encrypted link between 2 VPCs in the same account or cross-account. One peering connection can connect MAX two VPCs. Same region VPCs can reference each other by security groups. VPC CIDRs must NOT overlap! 

You can't create VPC chains with VPC peering using transitive peering. Every VPC my be connected together if you want to make peer connections between more than 2 VPCs:

A ---> B <br>
B ---> C <br>
C ---> A <br>

<img width="2358" height="1140" alt="image" src="https://github.com/user-attachments/assets/adbbf0af-a8a0-4412-bedc-573ca1a4fd3a" />

---
Links:

[[AWS Index]]
[[VPCs]]
[[Networking in AWS]]
[[2025-07-29]]





