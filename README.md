# 3-Tier-Architecture

Designed and implemented a secure 3-tier architecture in AWS with Terraform. The VPC has 2 public and 4 private subnets, with a NAT Gateway, public EC2, private EC2s and RDS databases, internet gateway and application load balancer. This design protects sensitive data and efficiently distributes traffic, providing a secure and well-structured environment for my AWS resources. 

The 3 Tier Architecture consists of a number of layers: presentation tier, application tier, and data tier:
The presentation tier is the part that is visible to the outside world. It includes the load balancer and the public-facing EC2 instance that people to interact with my aplication. The application tier (or the logic tier) is essentially where the "brains" of my application lives. The Data tier is where the application stores and manages data. It includes the RDS instances that hold all the data that the application needs.
