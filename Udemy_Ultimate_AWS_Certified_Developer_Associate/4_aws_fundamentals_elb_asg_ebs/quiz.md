# quiz

1. Load balancers provide
   1. a static dns we can use in our application
2. You are running a website with a load balancer and 10 EC2 instances. Your users are complaining about the fact that your website always asks them to re-authenticate when they switch pages. You are puzzled, because it's working just fine on your machine and in the dev environment with 1 server. What could be the reason?
   1. Stickiness not enabled on LB
3. Your application is using an Application Load Balancer. It turns out your application only sees traffic coming from private IP which are in fact your load balancer's. What should you do to find the true IP of the clients connected to your website?
   1. Look into the X-Forwarded-For header in the backend
4. You quickly created an ELB and it turns out your users are complaining about the fact that sometimes, the servers just don't work. You realise that indeed, your servers do crash from time to time. How to protect your users from seeing these crashes?
   1. Enable Health Checks
5. You are designing a high performance application that will require millions of connections to be handled, as well as low latency. The best Load Balancer for this is
   1. Network Load Balancer
6. Application Load Balancers handle all these protocols except
   1. TCP (other options were http, https, websocket)
7. The application load balancer can redirect to different target groups based on all these except...
   1.  Client IP
8. You are running at desired capacity of 3 and the maximum capacity of 3. You have alarms set at 60% CPU to scale out your application. Your application is now running at 80% capacity. What will happen?
   1. Nothing, we are already at capacity
9. I have an ASG and an ALB, and I setup my ASG to get health status of instances thanks to my ALB. One instance has just been reported unhealthy. What will happen?
   1. The ASG (AutoScaling Group) will terminate the EC2 instance (and create a new one)
10. Your boss wants to scale your ASG based on the number of requests per minute your application makes to your database.
    1. Create custom cloudwatch metric using PutMetric api and set and alarm on the new metric
11. Your instance in us-east-1a just got terminated, and the attached EBS volume is now available. Your colleague tells you he can't seem to attach it to your instance in us-east-1b.
    1. EBS volumes are AZ locked
12. Your company wants the most secure setup for your EBS volumes with minimal effort. You tell them
    1. EBS volumes are encrypted at rest and inflight using KMS encryption (AES-256)
