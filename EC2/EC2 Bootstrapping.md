#Amazon 

Bootstrapping in EC2 is when scripts and configuration are run when an instance is first launched. This allows us to have an instance start in a pre-configured way which is great for automation. 

User Data, limited to 16KB, is only executed by the OS at the initial launch and can be accessed at the following url: http://169.254.169.254/latest/user-data

There is a metric called Boot-Time-To-Service-Time that is greatly reduced by AMI baking and bootstrapping. 

<span class="red-text">User Data is not secure! Don't pass secrets!</span>

---
Links:

[[AWS Index]]
[[EC2]]