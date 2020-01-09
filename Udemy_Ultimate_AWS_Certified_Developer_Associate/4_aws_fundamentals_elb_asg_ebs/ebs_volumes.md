# ebs_volumes (elastic block store)
* Its a network drive, not a physical drive
* it can be detached and moved to another instance
* It's locked to an availability zone but can be snapshotted and moved to another
* have a provisioned capacity you are billed for

## Volume Size
GP2 General purpose SSD
IOI Highest performance SSD
STI low cost hdd
sci lowest cost hdd

EBS volumes are characterized in size throughput and iops

EBS volumes can be resized
IOI iops can be resized

# EBS snapshots
* EBS volumes can be backed up with snapshots and will only take space consumed for backup
* used for volume migration
* can be scheduled

# EBS Encryption
* EBS can be encrypted at rest
* Encrypted in flight
* snapshots are also encrypted
* all volume,es created from snapshot also encrypted
* encryption and decryption are handled transparently
* encryption leverages KMS (AES-256)

# Instance Store
* Some instances dont come with EBS they come with instance store
* instance stores are physically attached to the machine
* cant be resized but are high performance
* on termination are lost

# good to know
ebs can be attached to one instance at a time
locked at availability zone
snapshots need to be taken to migrate across zones

