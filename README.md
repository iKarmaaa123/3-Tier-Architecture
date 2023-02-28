# 3-Tier-Architecture

I designed and implemented a 3-Tier architecture in AWS using Terraform. The architecture consists of a VPC that I divided into two public subnets. One of the subnets includes a NAT Gateway to enable private instances to communicate with the internet while keeping the infrastructure secure. The other public subnet contains a public EC2 instance that acts as the entry point for my application. In addition to the public subnets, I created four private subnets to provide a secure environment for my private EC2 instances and RDS databases. These subnets are not accessible from the internet, which adds an extra layer of security to my architecture.To ensure a secure and reliable connection between the VPC and the internet, I utilised an internet gateway. This enabled the public EC2 instance to communicate with the internet while maintaining the security of my infrastructure.

To distribute incoming application traffic across the private instances, I used an application load balancer. This ensures that traffic is evenly distributed between the two private instances, which helps to prevent overloading and ensures a reliable and smooth experience for my users.
The 3 Tier Architecture consists of a number of layers: presentation tier, application tier, and data tier:
The presentation tier is the part that is visible to the outside world. It includes the load balancer and the public-facing EC2 instance that people to interact with my aplication. The application tier (or the logic tier) is essentially where the "brains" of my application lives. The Data tier is where the application stores and manages data. It includes the RDS instances that hold all the data that the application needs.
