# aws_sdk
Using AWS from within an application as opposed to the CLI

Multiple official and unofficial SDK's:
* Java
* .NET
* Node
* PHP
* Python (named boto3 / botocore)
* Go
* Ruby
* C++

If region not configured, will default to us-east-1

The CLI is based on the python sdk boto

## Credential Security
Recommend to use default credential provider chain
The default credential provider chain works seamlessly with
* AWS credentials at ~/.aws/credentials (on our computers only on premise, not ec2)
* Instance Profile credentials using IAM roles for EC2 machines
* Environment variables
  * AWS_ACCES_KEY_ID, AWS_SECRET_ACCESS_KEY

Overall NEVER STORE AWS CREDENTIALS IN CODE, use one of the inherited mechanism above, and 100% IAM roles within AWS services

## Exponential Backoff
If an API called in the SDK fails with too many calls needing retries, it will exponentially backoff
These apply to rate limited API
Retry mechanism included in SDK API calls

![exp_backoff](exp_backoff.png)

