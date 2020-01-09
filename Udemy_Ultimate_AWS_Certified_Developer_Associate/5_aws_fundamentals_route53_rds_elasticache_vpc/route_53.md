# Route 53
Route 53 is a managed DNS

DNS is a collection of rules and records which helps clients understand how to reach a server through URL's

In AWS, the most common records are:
* A: URL to IPv4
* AAAA: URL to IPv6
* CNAME: URL to URL

Route53 can use
* public domains (that we own)
* private domains (internal and resolvable within your vpc)

Route53 supports
* load balancing (via dns, client load balancing)
* health checks
* routing policys (simple, failover, geo etc)

Route53 doesnt appear much in the exam but worth knowing the records types