# IAM (Identify Access Management)

Acronyms:
* IAM: Identify Access Management
* MFA: Multi Factor Authentication

IAM Types:
* User
  * test
* Group
  * Contains Users
  * Typically named by fn i.e. developer
* Role
  * Contains Machines
* Policies
  * defined in json
  * governs users, groups and roles

Least privilege principle:
* Dont grant more privilege than the user/group/machine requires 

IAM Federation: Used for large enterprises, can integrate company ldap/ad with aws

IAM 101:
* One IAM User per PHYSICAL PERSON
* One IAM Role per Application
* IAM Credentials should never be shared
* IAM Credentials should never be in code
* Never use root account except for initial setup
