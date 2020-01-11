# quiz

Q1: I am creating an application and would like for it to be running with minimal cost in a development environment. I should run it in
A1: Single instance mode

Q2: Application versions can be linked to
A2: many environments

Q3: I would like to customize the runtime of Elastic Beanstalk and include some of my company wide security software. I should
A3: Provide a custom platform

Q4: Environments in Elastic Beanstalk
A4: Can be named freely

Q5: I would like to update my development environment as soon as a new version is available. Because my Elastic Beanstalk environment is internal and only used by me, I don't mind downtime. Which deployment options is the best fit?
A5: All at once

Q6: I would like to update my Elastic Beanstalk application so that we are able to roll back very quickly in case of issues with the new application version. Which deployment mode is the best fit?
A6: Immutable

Q7: I want to update my Elastic Beanstalk application gradually without incurring new costs on update. My application has been over provisioned and can temporarily decrease in size for the number of serving instances, but I still want to serve my users without downtime. I do not want to incur extra costs over updates. Which deployment mode is the best fit?
A7: Rolling

Q8: We would like to update our EB application with minimal added cost, while maintaining the full capacity to serve our current users in production. Which deployment is the best fit?
A8: Rolling with additional batches

Q9: I would like to create an ElastiCache with my Elastic Beanstalk environment. I should
A9: Create elasticache.config file in the .ebextensions folder at the root of the code zip file and provide appropriate configuration

Q10: My deployments on Elastic Beanstalk have been painfully slow, and after looking at the logs, I realize this is due to the fact that my dependencies are resolved on each EC2 machine at deployment time. How can I speed up my deployment with the minimal impact?
A10: Resolve dependancies beforehand and package them in the zip file upploaded to beanstalk

Q11: What service does Elastic Beanstalk use under the hood?
A11: Cloudformation

Q12: You would like your Elastic Beanstalk environment to expose an HTTPS endpoint instead of an HTTP endpoint in order to get in-flight encryption between your clients and your web servers. What must be done to setup HTTPS on Beanstalk?
A12: Create an .ebextension file to configure the load balancer

Q13: How can you remove older versions that are not used by Elastic Beanstalk so that new versions can be created for your applications?
A13: Use lifecycle policy

Q14: You are looking to perform a set of repetitive and scheduled tasks asynchronously. Which Elastic Beanstalk environment should you setup?
A14: setup worker env with cron.yaml file

Q15: You have created a test environment in Elastic Beanstalk and as part of that environment, you have created an RDS database. How can you make sure the database can be explored after the environment is destroyed?
A15: Make a snapshot of the database before it gets deleted