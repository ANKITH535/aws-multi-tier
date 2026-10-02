# AWS Multi-Tier Web Application

**Project by:** Ankith

## Project Overview

This project demonstrates the design and hands-on deployment of a
multi-tier web application on Amazon Web Services (AWS).

The project was built to practice AWS networking, compute, load
balancing, auto scaling, database services, monitoring, identity and
access management, and cloud security.

## Architecture

``` text
                    Internet
                       |
                       v
             Application Load Balancer
                       |
                       v
                Auto Scaling Group
                 /             \
                v               v
             EC2 App         EC2 App
                \               /
                 \             /
                  v           v
                    RDS Database
```

The infrastructure used an Amazon VPC with public and private subnets
and separated application and database tiers.

## AWS Services Used

-   Amazon VPC
-   Subnets
-   Route Tables
-   Internet Gateway
-   NAT Gateway
-   Security Groups
-   Amazon EC2
-   Application Load Balancer (ALB)
-   Target Groups
-   Auto Scaling Group (ASG)
-   Amazon RDS
-   AWS IAM
-   Amazon CloudWatch

## Key Implementation Areas

### 1. Networking

A dedicated VPC was used to organize the cloud environment. Subnets,
route tables, Internet Gateway, NAT Gateway, and security groups were
configured to control connectivity between the required tiers.

### 2. Application Load Balancer

An Application Load Balancer was configured to receive application
traffic and forward requests to EC2 instances through a target group.

Health checks were used to verify application instance availability.

### 3. EC2 and Auto Scaling

EC2 instances hosted the application tier. An Auto Scaling Group was
configured to maintain the required number of instances and replace
instances when necessary.

### 4. Database Tier

Amazon RDS was used for the database tier. The database was kept
separate from the public application-facing components.

### 5. Identity and Access Management

AWS IAM was used for access and permissions management.

### 6. Monitoring

Amazon CloudWatch was used for monitoring EC2 metrics and configuring
alarms.

## Testing

The project included testing the application through the load balancer,
checking target health, verifying EC2 instances, and testing Auto
Scaling behavior.

## Project Completion

The AWS environment was tested and the project was completed
successfully. After completing the hands-on work, the AWS resources were
deleted to avoid unnecessary ongoing charges.

## Skills Demonstrated

-   AWS Cloud Fundamentals
-   VPC Networking
-   EC2
-   Application Load Balancing
-   Auto Scaling
-   RDS
-   IAM
-   CloudWatch
-   Security Groups
-   High-availability concepts
-   Cloud troubleshooting

## Note

This repository contains documentation for the AWS project. The
temporary AWS resources used during the hands-on implementation were
removed after completion.
