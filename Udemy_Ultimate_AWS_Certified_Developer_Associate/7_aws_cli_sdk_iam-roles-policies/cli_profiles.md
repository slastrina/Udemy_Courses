# cli_profiles

aws configure --profile <profile_name>

and proceed to configure it

![configure_profile](configure_profile.png)

View inside the aws credential file:
![aws_cred_file](aws_cred_file.png)

Executing a command against a specific profile: --profile <profilename>
i.e. aws s3 ls --profile <profilename>

![using_a_profile](using_a_profile.png)

Profiles wont be on the exam but good to know
