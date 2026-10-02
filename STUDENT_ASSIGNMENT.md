# Student Assignment --- AWS Multi-Tier Web Application

**Student:** Ankith

## Objective

Design and implement a highly available multi-tier web application using
AWS services.

## Requirements Covered

-   [x] VPC-based network architecture
-   [x] Public and private subnet concepts
-   [x] Route tables and Internet Gateway
-   [x] Security Groups
-   [x] EC2 application tier
-   [x] Application Load Balancer
-   [x] Target Group and health checks
-   [x] Auto Scaling Group
-   [x] Amazon RDS database tier
-   [x] Amazon S3
-   [x] IAM
-   [x] CloudWatch monitoring
-   [x] Application testing
-   [x] AWS resource cleanup after completion
-   [x] Route 53 concepts/configuration where applicable

## Architecture Summary

The project used a layered architecture in which internet traffic was
received by the Application Load Balancer, forwarded to EC2 application
instances managed by an Auto Scaling Group, and the application tier
communicated with the database tier.

## Security

Security Groups were used to control traffic between the different
tiers. The database tier was designed to avoid direct public access.

## Availability

The project demonstrated the use of an Application Load Balancer and
Auto Scaling Group to improve application availability and provide
instance replacement/scaling capabilities.

## Monitoring

CloudWatch was used to observe EC2 metrics and configure
monitoring/alarms.

## Cleanup

After the project was completed and tested, the AWS resources were
deleted to prevent unnecessary charges.

## Learning Outcomes

This project provided practical experience with AWS networking, compute,
load balancing, scaling, databases, storage, IAM, monitoring, DNS
concepts, and cloud security.
