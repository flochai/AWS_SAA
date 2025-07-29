Border Gateway Protocol (BGP) is a TCP-based path-vector routing protocol (TCP port 179) used to control how data moves between networks (Autonomous Systems, or AS). Unlike interior protocols like OSPF, BGP is policy-driven, prioritizing routing rules and agreements rather than just shortest paths. Services like AWS Direct Connect and dynamic VPNs often rely on BGP.

Think of BGP as air traffic control for the internet. Routers (planes) must know which routes (flight paths) are safe and optimal, and BGP enforces these rules.

The internet is made up of many ASes, each managed by a single organization and identified by an Autonomous System Number (ASN) (0–65,535). BGP peers, or “neighbors,” exchange route information across networks.

	•	iBGP: routes within a single AS.
	•	eBGP: routes between different ASes.

By default, BGP selects the shortest AS path, even if a longer path performs better. AS Path Prepending can make a path look artificially longer to influence routing decisions.


<img width="1269" height="603" alt="image" src="https://github.com/user-attachments/assets/779b7292-4c87-4459-b308-0b85c6edd689" />


---
Links:

[[AWS Index]]
[[2025-07-29]]
