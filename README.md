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

Classic load balance with some improvements (e.g. supported protocols, cloudWatch metrics, access logs, health check)

The load balancer distributes incoming application traffic across multiple targets

#### Auto scaling 

Helps you ensure that you have the correct number of EC2 instances available to handle the load for your application

Auto scaling components
     
 - launch configuration (what?)
 - auto scaling group (where?)
 - auto scaling policy (when?)
     
Define an alarm for auto scaling through CloudWatch (eg. Whenever CPU utilization is >= 80%, auto scaling take this action…add 2 instances)

#### Route 53

DNS Service - service designed to provide an way to route end users to endpoints (translate name to IP address

DNS resolution strategies

 - simple routing
 - geo-location
 - failover
 - weighted round robin
 - latency-based
 - multi-value answer

DNS translator

 - global, highly available DNS
 - domain registration
 - public and private dns names
 - multiple routing algorithms
 - both ipv4 and ipv6
 - integrated with other AWS cloud services
 
#### RDS (Amazon Relational Database Services)

Is a managed service that sets up and operates a relational database in the cloud

Benefits:

 - highly scalable
 - high performance
 - easy to administer
 - available and durable
 - secure and compliant

DB Engines:

 - Amazon Aurora
 - MySQL
 - MS SQLserver 
 - Oracle
 - PostgreSQL
 - MariaDB
 
#### AWS Lambda
 
Is a compute service that lets you run code in response to events without provisioning or managing servers
 
  - fully-managed serverless compute
  - event-driven execution
  - sub-second metering
  - multiple language supported
  
#### AWS Elastic Beanstalk
  
Is an easy-to-use service for deploying and scaling web applications and services
  
  - platform as a service
  - allows quick deployment of your applications
  - reduces management complexity
  
#### SNS (Amazon Simple Notification Service)

Is a notification service

 - flexible, fully managed pub/sub messaging and mobile communications service
 - coordinates the delivery of messages to subscribing endpoints and clients
 - easy to setup, operate and send reliable communications
 - decouple and scale microservices, distributed systems and serverless applications
 
#### Amazon CloudWatch

Monitors your Amazon Web Services (AWS) resources and the applications you run on AWS in real time

 - collect and track metrics
 - collect and monitor log files
 - set alarms
 - automatically react to changes

#### Amazon CloudFront

Is a content delivery network (CDN) allowing your users to interact with your application in a lower latency

 - global, growing network
 - secure content at the edge
 - deep integration with key AWS services
 - high performance
 - cost effective
 - easy to use
 
#### Amazon CloudFormation

Provides a common language for you to model and provision AWS and third party application resources in your cloud environment

Infrastructure as a code - control your infrastructure through software code

#### AWS Architecture

5 pillars

1. security
   - identify and access management (IAM)
   - detective controls
   - infrastructure protection
   - data protection
   - incident response
    
2. reliability
   - recover from issues/failures
   - apply best practices in: foundations, change management and failure management
   - anticipate, respond, and prevent failures
   
3. performance efficiency
   - select customizable solutions
   - review to continually innovate
   - monitor AWS services
   - consider the trade-offs 

4. cost optimization
   - use cost-effective resources
   - matching supply with demand
   - increase expenditure awareness
   - optimize over time
  
5. operational excellence
   - manage and automate changes
   - respond to events
   - define the standards
   
- fault tolerance
  - ensures that:
    - ability of a system to remain operational
    - built-in redundancy of an application's component
    
  - services tools can assist in providing fault tolerance
    - sqs
    - s3
    - rds
    
- high availability   
  - ensures that:
    - systems are generally functioning and accessible
    - downtime is minimized
    - minimal human intervention is required
    - minimal up-front financial investment
    
  - services tools can assist in providing high availability
    - elastic load balance (ELB)
    - elastic IP address
    - route 53
    - auto scaling
    - cloudWatch
    
#### AWS Security
    
 - resilient infrastructure
 - high security
 - strong safeguards
 
 
 - continual improvement
    - rapid innovation
    - constantly evolving security services
    
    
 - pay for what you need
    - advanced security services
    - address real-time emerging risks
    - meeting needs at a lower operational cost
    
    
 - meet compliance requirements
    - governance-enabled features
       - additional oversight
       - security control
       - central automation


 - AWS shared responsibility model
    - inherit AWS security controls
    - layer your controls
    
    
 - network security
    - built-in firewalls
    - encryption in transit
    - private/dedicated connections
    - distributed denial of service (DDoS) mitigation
 
 
 - inventory and configuration management
    - deployment tools
    - inventory and configuration tools
    - template definition and management tools
    
    
 - data encryption
    - encryption capabilities
    - key management options
    - hardware-based cryptographic key storage options
    
    
 - access control and management
    - identify and access management (IAM)
    - multi-factor authentication (MFA)
    - integration and federation with corporate directories
    - Amazon Cognito
    - AWS SSO 
    
    
 - monitoring and logging
    - deep visibility into API calls
    - log aggregation and options
    - alert notifications
    
    
 - AWS marketplace
    - qualified partners to market/sell software to AWS customers
    - online software store that can run on AWS
    

#### Shared Responsibility Model

 | layer | responsibility | 
 | --- | --- |
 | User Data   | you |
 | Application | you |
 | Guest OS    | you |
 | Hypervisor  | aws |
 | Network     | aws |
 | Physical    | aws |
 
 #### Identify and Access Management (IAM)
 
 (Authentication)

 User - operator (human or machine). permanent set of credentials

 Group - Set of users

 Role - operator (human or machine). credentials with a role are temporary

(Authorization)

Policy docs - JSON file. It attaches directly to a permanent name user or to a group of users or to a role