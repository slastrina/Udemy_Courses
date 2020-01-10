# s3_performance

If you want a faster upload for files larger than 100mb, use multipart upload
* paralellizes PUTS for greater throughput
* maximise your network bandwidth
* decrease retry time if part fails
* must use multi-part if greater than 5gb

Use CloudFront to cache S3 objects around the world (improves reads)

S3 Transfer Acceleration (uses edge locations) - just need to change the endpoint you write to

if using SSE-KMS encryption you may be limited to your AWS limits for KMS usage (~100s - 1000s of downloads/uploads per second) (typical exam questions)

