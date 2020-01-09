# Elastic IP
EC2 instances gain a different public ip address on each start,  
elastic ip binds the instance random public ip to an owned static public ip similar to

elastic ip's reflect poor architectural decisions, it is better to use a random ip and assign a dns name via route 53

Best pattern is to use a load balancer instead of a public ip

An AWS account can have up to 5 elastic ip's

