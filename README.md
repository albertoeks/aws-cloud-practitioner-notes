## AWS Cloud Practitioner
Some personal notes about AWS Cloud Practitioner Exam

### AWS Benefits

Scalability = means ability to resize your resources as necessary

#### Other benefits with cloud

Agility - increase speed, easy experimentation, cultivating culture innovation

Elasticity - power to scale it resources up or down easily 

Reliability  - ability of a system to recover from infrastructure or service failures

Fault tolerance - system can remain operational even if some of the components of the system fail

High availability - ensures that your systems are always functioning and accessible

#### AWS Interfaces

 - Console (Graphical interface)
 - CLI
 - SDK
 
#### EC2 (Elastic Compute Cloud)

 - pay as you go (pay just while you’re using)
 - broad selection of HW/SW
 - global hosting

AMI - Amazon Machine Images

#### EBS (Elastic Block Store) 
storage service designed for use with EC2

 - HDD and SSD: volumes types available 
 - Snapshots: provides the ability to save snapshots of your volumes to Amazon S3
 - Elasticity: adapt your volumes as the needs of your applications
 
#### S3 (Simple Storage Service)
 
 - managed cloud storage service (isn’t associated with any particular server, you don’t have to manage any infrastructure yourself)
 - store virtually unlimited number of objects
 - access anytime, from anywhere (https://{bucket-name}/{region-specific endpoint}/{key})
 - rich security controls
 
 Bucket - key and object
 
#### AWS Global Infrastructure
 
  - AWS regions: geographic areas that host two or more availability zones
  - Availability zones: collection of data centers in a specific region
  - Edge locations: deliver content to end users with lower latency (Amazon CloudFront)
 
#### Amazon Virtual Private Cloud (VPC)
 
  - a private virtual network in the AWS cloud
  - allows complete control of network configuration
  - offers several layers of security controls
  - other AWS services deploy into VPC
 
 Features
 
  - builds upon high availability of AWS regions and availability zones
  - subnets (used to divide Amazon VPC) {you can create many subnets but fewer is recommended to limit complexity}
  - route tables (control traffic)
  - internet gateway (allow access to internet from Amazon VPC)
  - NAT gateway (private subnet)
  - network access control lists - NACL (controle access to subnets) 
 
#### AWS Security Groups
 
  - act as built-in firewalls 
  - control accessibility to instances through rules
  
#### Application Load Balancer

Application Load Balancer

Classic load balance with some improvements (e.g. supported protocols, cloudWatch metrics, access logs, health check)