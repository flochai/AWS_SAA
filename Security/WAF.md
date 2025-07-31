The Web Application Firewall is the AWS implementation of a layer 7 firewall. The following is a complex architecture example using WAF. 

<img width="1212" height="592" alt="Pasted image 20250731082316" src="https://github.com/user-attachments/assets/12343616-569e-412f-91e7-1a45f36b769e" />

### 1. WACL

The Web ACL is the rule groups and rules of the firewall applied to the resources we want to protect. These rules are processed in a sequential order which can be modified. Web ACL Capacity Units are the unit of compute for the rules which have a default of 1500 WCU (increase via support ticket). A resource can have 1 WACL but 1 WACL can be used with many resources at the same time. 

### 2. Rule Groups

These are groups of rules that are used with WACL. They can be created or found on the AWS marketplace: most are free but some have a cost. Multiple WACL can reference a group of rules. 

### 3. Rules

Rules have a simple structure: 

- Type: regular or rate-based 
- Statement: defines what the rule checks for (WHAT or COUNT or WHAT + COUNT)
- Action: what is done by WAF (allow, block, count, captcha, label, custom response)

⚠️ body check only limited to the first 8192c

### 4. Pricing 

There is a monthly charge for each WACLs.
There is a monthly charge per rule.
There is a charge per million request.
Some rule groups can have extra costs (bot control, catcha, fraud control, etc). 

---
Links:

[[AWS Index]]
[[2025-07-31]]
