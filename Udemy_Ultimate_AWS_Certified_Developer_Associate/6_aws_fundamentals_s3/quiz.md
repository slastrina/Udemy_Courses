# quiz

Q1: You're trying to upload a 25 GB file on S3 and it's not working: you should use multi-part upload, 5gb is the limit for single-part upload

Q2: I tried creating an S3 bucket named "dev" but it didn't work. This is a new AWS Account and I have no buckets at all. What is the cause?
A2: Bucket names must be globally unique

Q3: You've added files in your bucket and then enabled versioning. The files you've already added will have which version?
A3: null

Q4: Your client wants to make sure the encryption is happening in S3, but wants to fully manage the encryption keys and never store them in AWS. You recommend
A4: SSE-C: client manages keys but encryption still occurs in S3

Q5: Your company wants data to be encrypted in S3, and maintain control of the rotation policy for the encryption keys. You recommend
A5: SSE-KMS

Q6: Your company does not trust S3 for encryption and wants it to happen on the application. You recommend
A6: Client Side Encryption

Q7: Which encryption method requires HTTPS?
A7: SSE-C

Q8: You have a website that loads files from another S3 bucket. When you try the URL of the files directly in your Chrome browser it works, but when the website you're visiting tries to load these files it doesn't. What's the problem?
A8: CORS is wrong

Q9: When uploading a file that is 1 GB to S3, which type of upload will give you the best throughput performance and resilience?
A9: Multipart upload to maximise throughput

Q10: You would like to retrieve a subset of your dataset stored in S3 with the CSV format. You would like to retrieve a month of data and only 3 columns out of the 10. You need to minimize compute and network costs for this, what should you use?
A10: S3 Select (SQL style queries of files in S3/glacier)

