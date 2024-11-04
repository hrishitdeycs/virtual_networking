# virtual_networking
## VPC
### AWS Console -> Services -> Networking & Content Delivery -> VPC -> Your VPCs
### VPC Name: MyVPC
### IPv4 CIDR Block: 10.0.0.0/16
### Click Create
![Screenshot (6)](https://github.com/user-attachments/assets/dc1ec107-f43b-4f8c-8689-269dffd602a8)

### Create subnets :-
### S1-Private Us-east-2a 10.0.1.0/24 Private
### S2-Private Us-east-2b 10.0.2.0/24 Private
### S3-Public Us-east-2a 10.0.3.0/24 Public
### S4-Public Us-east-2b 10.0.4.0/24 Public
![Screenshot (7)](https://github.com/user-attachments/assets/ed2d850f-42f7-4074-afe5-f1ad0714cd52)

### Create Internet gateway 
### Now attach Internet Gateway to VPC
### Create Virtual Private Gateway 
###  Now attach Virtual Private Gateway  to VPC
### Create route tables and attach to subnets
![Screenshot (8)](https://github.com/user-attachments/assets/793c6d62-971c-405e-9283-26f1071dd9db)

## ELB
###  Launch two EC2 instances in different AZs
![Screenshot (9)](https://github.com/user-attachments/assets/3d985a1a-f79f-47d3-a087-28febb549da9)

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
![Screenshot (5)](https://github.com/user-attachments/assets/ee6678f9-b7f4-4606-893b-a338e4717f83)

