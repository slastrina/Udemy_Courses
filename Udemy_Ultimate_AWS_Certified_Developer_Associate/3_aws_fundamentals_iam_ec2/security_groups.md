# Security Groups
Security groups act as a firewall for EC2 instances, it regulates
* ports
* ip ranges
* inbound traffic
* outbound traffic

security groups can be attached to multiple instances
security groups are locked to a region and vpc, security groups need to be recreated for other regions or vpc's

Good practice to separate ssh from other security groups

Can reference security groups from others (hierarchical security groups)
