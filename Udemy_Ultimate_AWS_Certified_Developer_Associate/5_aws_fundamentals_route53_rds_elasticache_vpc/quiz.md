# quiz

Q1: Route53 is a: Global Service

Q2: I have an ALB and I'd like to give it my own URL. I should choose a(n): Alias Record

Q3: My company would like to have a MySQL database internally that is going to be available even in case of a disaster in the AWS Cloud. I should setup
A3: Multi AZ

Q4: Our RDS database struggles to keep up with the demand of the users from our website. Our million users mostly read news, and we don't post news very often. Which solution will NOT help fix this problem?
A4: RDS Multi AZ (Other options Elasticache cluster, Read replicas)

Q5: We have setup read replicas on our RDS database, but our users are complaining that upon updating their social media posts, they do not see the update right away
A5: Read Replicas are ASYNC, synchronisation occurs over time with eventual consistency and is not instantaneous

Q6: Which RDS feature does not require us to change our SQL connection string ?
A6: Multi AZ, Read replicas are actual databases with their own connection strings and will require changing strings

Q7: Your organisation wants to enforce SSL connections on your MySQL database
A7: Apply a 'REQUIRE SSL' to all users in SQL database

Q8: You want to ensure your Redis cluster will always be available: Enable Multi AZ

Q9: Your application functions on an ASG behind an ALB. Users have to constantly log back in and you'd rather not enable stickiness on your ALB as you fear it will overload some servers. What should you do?
A9: Store session data in elasticache

Q10: You are implementing a caching strategy with ElastiCache and would like to ensure that only the data that is often requested will be loaded in ElastiCache, as your cache size is small. Which caching strategy should you implement?
A10: Lazy Loading