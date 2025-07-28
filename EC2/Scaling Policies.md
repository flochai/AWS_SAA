#Amazon 

Scaling Policies are user defined rules that define how the [[ASG]] scales. Scaling Policies are optional  which means the ASG has static values when no policy is defined. 

Scheduled Scaling: great for known periods of additional demand or less demand

Dynamic Scaling: 

1. Simple: "CPU > 50% +1", "CPU < 50% -1"
2. Stepped Scaling: different steps based on the amplitude of the change. Example:

>50-59% do nothing
>60-69% ADD 1
>70-79% ADD 2
>80-100% ADD 3    

3. Target Tracking: desired CPU usage = 40% (example)
4. Scaling Based on SQS - ApproximateNumberOfMessagesVisible


The cooldown period is how long the ASG will pause before doing another scaling action. 
They are often used in conjunction with ELBs. 

Scaling Processes:

- Launch / Terminate - Suspend and Resume
- AddToLoadBalancer 
- AlarmNotification 
- AZRebalance
- HealthCheck - on/off
- ReplaceUnhealthy
- ScheduleActions
- Standby

---
Links:
[[ASG]]
[[2025-07-24]]