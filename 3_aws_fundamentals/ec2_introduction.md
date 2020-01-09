# EC2 (Elastic Computer Cloud)

## Acronyms and Terminology
* EC2: Elastic Computer Cloud
* Region: Location the datacenters reside in
* Availability Zone: Datacenter the instance will reside in
* Subnet (AWS): Availability Zone

## Instance Details
* Spot Instance: Procurement of unused EC2 capacity in the AWS cloud, subject to availability
* Network: the vpc the instance will be connected to

## SSH Quick Commands
ssh -i pemfile.pem ec2-user@ipaddress

Note: pem file needs 0644 permissions or ssh tool will ignore it and authentication will fail
i.e. chmod 0400 pemfile.pem