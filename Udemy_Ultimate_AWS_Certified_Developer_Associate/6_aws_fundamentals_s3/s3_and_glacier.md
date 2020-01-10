# s3_and_glacier

Glacier is another s3 tier for long term archival

* if you retrieve data in S3 and glacier you may only want a subset of it
* if you retrieve all the data network cost may be high

with s3 select/glacier select you can use SQL select queries to let S3 know exactly which attirbutes / filters you want
* ```select * from s3object s where s.\"Country (Name)\" like '%United States%'```
* save up to 80% and increase performance by 400%
* Not possible from S3, need to be done in code
* The SELECT happens within S3 or Glacier
* Works with files in CSV, JSON, or Parquet format
* Files can be compressed with GZIP or BZIP2
* No subqueries or joins are supported

