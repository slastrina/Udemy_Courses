# Bootstrapping EC2 instance

1. create EC2 instance as amazon linux 2 ami
2. nano size
3. Under configure instance expand advanced, and input the following block under userdata->"as text"

``` shell script
#!/bin/bash

# get admin privileges
sudo su

# install httpd (Linux 2 version)
yum update -y
yum install -y httpd.x86_64
systemctl start httpd.service
systemctl enable httpd.service
echo "Hello World from $(hostname -f)" > /var/www/html/index.html
```

4. add existing security group that exposes ssh and http
5. use existing ssh key
6. Start and observe the web server is up by travelling to the public ip
