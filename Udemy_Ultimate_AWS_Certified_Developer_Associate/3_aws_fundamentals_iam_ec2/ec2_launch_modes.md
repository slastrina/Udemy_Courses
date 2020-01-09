# Launch Modes
* On-Demand:
  * Pay what you use
  * billing per second after first minute
  * higher cost but no upfront payment
  * no commitment
* Reserved Instance
  * up to 75% discount
  * pay up front
  * reserve for 1-3 years
  * ideal for database instances
* convertible Reserved instance
  * up to 54% discount
  * can change the instance type
  * reserve for 1-3 years
* Scheduled Reserved Instances
  * launch within time window you reserved
* Spot Instances
  * Up to 90% off
  * bid for instance, get to keep instance as long as someone doesnt outbid
  * 2 minute notification if outbid
* Dedicated host
  * Full control of ec2 instance
  * you control the hardware
  * 3 year reservation
  * physical ec2 instance
  * ensures no one else is on that hardware
* EC2 Dedicated Instances
  * Dedicated hardware that you control
  * Other accounts under you may launch instances under the same node but private to your team

# Burstable Instances
For T2/T3 machines

Has a normal base performance however with sudden unexpected load can use burst credit to temporarily scale up and handle the increased load

CPU credit balance regenerates over time

T2 Unlimited: unlimited burst credit balance however you pay for additional cpu capacity

# Other Notes
* EC2 Instances are billed per second after the first 60 seconds (flagfall)