# virtual_networking
## VPC
### AWS Console -> Services -> Networking & Content Delivery -> VPC -> Your VPCs
### VPC Name: MyVPC
### IPv4 CIDR Block: 10.0.0.0/16
### Click Create
### Create subnets :-
### S1-Private Us-east-2a 10.0.1.0/24 Private
### S2-Private Us-east-2b 10.0.2.0/24 Private
### S3-Public Us-east-2a 10.0.3.0/24 Public
### S4-Public Us-east-2b 10.0.4.0/24 Public
### Create Internet gateway 
### Now attach Internet Gateway to VPC
### Create Virtual Private Gateway 
###  Now attach Virtual Private Gateway  to VPC
### Create route tables and attach to subnets
## ELB
###  Launch two EC2 instances in different AZs
### Create Classic Elastic Load Balancer
### Click Next: Assign Security Groups
### Click Next: Security Settings
### Click Next: Configure Health Checks
### Specify your default web file 
### Click Next: Add EC2 Instances
### Click Next: Add Tags
### Click Review and Create
### Click Create
### Check instances status should be InService
### Load Balancer DNS Name copy it and paste in web browser now fresh twice you will see response is coming from Server1 and Server2
### Which concludes load balancer is working fine.
