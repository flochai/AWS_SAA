#  AWS Shield – DDoS Protection for Your Infrastructure

**AWS Shield** is a managed DDoS protection service that defends applications running on AWS. It applies protection at the **VPC** or **Edge (CloudFront/Route 53)** level and helps mitigate 3 major types of attacks:


##  Types of DDoS Attacks Covered

1. **Network Volumetric Attacks (Layer 3)**  
   Flood the network with traffic to overwhelm infrastructure.  
   *Example:* Packet floods like UDP floods or ICMP floods.

2. **Protocol Attacks (Layer 4)**  
   Exploit protocol weaknesses (e.g., SYN floods), exhausting connection tables.  
   *Think:* Too many calls and nobody hangs up—your system can’t take new ones.

3. **Application Layer Attacks (Layer 7)**  
   Send cheap requests that trigger expensive server operations.  
   *Example:* HTTP floods targeting login or search endpoints.



## Two Shield Tiers

| Feature | **Shield Standard** | **Shield Advanced** |
|---------|---------------------|----------------------|
| Cost | Free | $3,000/month per org (1-year commitment) |
| Customization | Minimal | Extensive (via APIs & AWS WAF) |
| Coverage | Basic automatic DDoS mitigation | + Cost protection, enhanced metrics, 24/7 access to SRT |
| WAF fees included | ❌ | ✅ WAF capacity units (WCU) and request fees included |
| SRT Access | ❌ | ✅ |



## Shield Advanced Features

- **Protection Groups:** Aggregate multiple resources (like ELBs, CloudFront distros, Route 53 zones) into logical groups for consolidated protection and metrics.
- **Cost Protection:** If a DDoS attack leads to charges, AWS may waive the costs (must be an attack that Shield *should* have mitigated).
- **AWS Shield Response Team (SRT):**  
  DDoS experts that provide real-time support during and after an attack.  
  _Note: Requires enabling **health-based detection**._
- **Manual Activation:** Protections are not automatically enabled—you must **explicitly protect** resources.


## Exam Tip

- Shield **Advanced is billed per organization**, not per account.
- Health-based detection is a prerequisite for SRT involvement.
- Pairing Shield Advanced with **AWS WAF** offers layered protection at L7.
