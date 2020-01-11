# quiz

Q1: My EC2 Instance does not have the permissions to perform an API call PutObject on S3. What should I do?
A1: i should ask admin to attach a policy to the iam role on my ec2 instance that authorises it to do that api call

Q2: The AWS CLI depends on which language? Python

Q3: I have an on-premise personal server that I'd like to use to perform AWS API calls
A3: I should run 'aws configure' and put my credentials there. invalidate when im done

Q4: I'd like to deploy an application to an on-premise server. The server needs to perform API calls to Amazon S3. Amongst the following options, the best security I can achieve is...
A4: create iam role for the application and put credentials in environment variables, here its about creating a dedicated user for that application as using your own credentials blur the lines between actual users and applications

Q5: I need my colleagues help to debug my code. When he runs the application on his machine, it's working fine, whereas I get API authorisation exceptions. What should I do?
A5: Compare his IAM policy and my iam policy in the policy simulator to understand the difference

Q6: When I run the CLI on my EC2 Instances, the CLI uses the ______ service to get _____ credentials thanks to the IAM Role that's attached.
A6: meta data | temporary

Q7: To get the instance id of my EC2 machine from the EC2 machine, the best thing is to...
A7: Query the meta data at http://169.254.169.254/latest/meta-data

Q8: I want to test whether my EC2 machine is able to perform the termination of EC2 instances. There is an IAM role attached to my EC2 Instance. I should
A8: Use the IAM policy simulator or dry run option

Q9: Can EC2 Instances retrieve the IAM Role policy JSON document that's attached to them using the CLI without any role attached?
A9: No

Q10: I have received an authorisation exception from my EC2 instance while performing an EC2 API call.
Q10: Message: ```vbguZQlpz4e1h4rtSaXnEfDAFZPii8XvCNW7dLIE4Xy-zE8VcNIeh8tf4DAn1APFw__Nr55bUE0hrS02bg50EimidVBPHH1rtWmhQOtmv5tdUY5VelEAhc5O9OC8h4fYRlegBxfUNrGSCqlH83h_HMyaqC1fQy2G7rNjmFEPcN-pue2NZc9MMZMRdfWbYszMlbkAYlrAmSMmr4F0FE6BWOUxFOCdRnuwwb8OEM9c8RXBK8F91YqgdbW_XvxYBi2_BEI2P-8gFz4LmBkba1UdEylh-WUS95XInC3OU8i3wZZ-xKExGWu1HwoqS9QAqIqm6jmn7wbTK_v9EVv0jMnCzmNxuMHpqmw2Ys3Bu3WdqvAwHxmT5W_XCbGBdtstckPXkeSyNS5hLSNLBjjRgd_I8JfPKTmB79sB_mUBSTlc28z5wjv1UBtxKBLT5GHdHQM8s2dP30cJCObRITmNvJo6Q8zaya1XYpwvCGIQrWF6-xaYQeXFCmMgyfsosIS8bVfpNyzzz2usC1mFJMlwIciissbz10YslH-PQF7Wwvn_6ypipoQVh0z80XglLVYnfbXGFv330ZyviBQnttklCecIK56OMcAxPJfTIWru57RoKedhJaHiKVEdLtILvVJgJ71wn-6wd4QA9aMh38jTpI_-cOPWLsvNq5NbtfqxQZ5BJOUs0rQpTmYRF_FtlY1k```
Q10: I want to decode the message, how do i do it
A10: Use the STS decode-authorization-message api

Q11: My KMS API call just failed against AWS. It's seems I've reached the rate limit of the KMS API. I should retry
A11: Using an exponential backoff strategy
