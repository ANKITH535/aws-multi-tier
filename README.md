# AWS Multi-Tier Web Application

**Project by:** Ankith

## Project Overview

This project demonstrates the design and deployment of a multi-tier web
application on Amazon Web Services (AWS).

The environment was built as a hands-on cloud project to practice AWS
networking, compute, load balancing, auto scaling, database services,
storage, monitoring, and access management.

## Architecture

The application follows a multi-tier architecture:

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

The infrastructure was organized using an Amazon VPC with public and
private networking components.

## AWS Services Used

-   Amazon VPC
-   Subnets
-   Route Tables
-   Internet Gateway
-   Security Groups
-   Amazon EC2
-   Application Load Balancer (ALB)
-   Target Groups
-   Auto Scaling Group (ASG)
-   Amazon RDS
-   Amazon S3
-   AWS IAM
-   Amazon CloudWatch
-   Amazon Route 53 (where configured)

## Key Implementation Areas

### 1. Networking

A dedicated VPC was used to organize the cloud environment. Subnets,
route tables, and security groups were configured to control
connectivity between the application and database tiers.

### 2. Application Load Balancer

An Application Load Balancer was configured to receive application
traffic and forward requests to the EC2 instances through a target
group.

Health checks were used to verify the availability of the application
instances.

### 3. EC2 and Auto Scaling

EC2 instances hosted the application tier. An Auto Scaling Group was
configured to maintain the required number of instances and replace
instances when necessary.

### 4. Database Tier

Amazon RDS was used for the database tier. The database was kept
separate from the public application-facing components.

### 5. Storage

Amazon S3 was used for cloud object storage as part of the project.

### 6. Identity and Access Management

AWS IAM was used to manage permissions and access to AWS resources.

### 7. Monitoring

Amazon CloudWatch was used for monitoring and alarms, including
EC2-related metrics.

### 8. DNS

Route 53 was studied/configured as part of the project for DNS
management where applicable.

## Testing

The project included testing the application through the load balancer,
checking target health, verifying EC2 instances, testing Auto Scaling
behavior, and checking connectivity between the required AWS components.

## Project Completion

The AWS environment was tested and the project was completed
successfully. After completing the hands-on work, the temporary AWS
resources were deleted to avoid unnecessary ongoing charges.

## Skills Demonstrated

-   AWS Cloud Fundamentals
-   VPC Networking
-   EC2
-   Application Load Balancing
-   Auto Scaling
-   RDS
-   S3
-   IAM
-   CloudWatch
-   Route 53
-   Security Groups
-   High-availability concepts
-   Cloud troubleshooting

## Note

This repository contains project documentation and learning material for
the AWS implementation. AWS resources used during the hands-on lab were
removed after completion.
