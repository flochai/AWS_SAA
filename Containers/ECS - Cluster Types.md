#Amazon 

### 1. EC2 Mode

- ECS management component      --->      like a control plane
- Auto Scaling Group takes cares of horizontal scalingal
- uses EC2 instances to run containers 
- it can be a good idea to combine this with spot pricing for reduced costs

### 2. FarGate Mode

- Less admin overhead because it is serverless
- there is a shared hardware platform but no visibility on others
- the containers are injected into our VPC with ENI

EC2 mode is cheaper than Fargate mode but requires more management.
Fargate is good for periodic or burst workloads because you pay fargate when you use it whereas you continually pay for ec2 mode.

---
Links:

[[AWS Index]]
[[ECS]]
[[2025-07-20]]