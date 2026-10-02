
# Student Assignment --- AWS Multi-Tier Web Application

**Student:** Ankith

## Objective

Design and implement a multi-tier web application using AWS services.

## Requirements Covered

-   [x] VPC-based network architecture
-   [x] Public and private subnet concepts
-   [x] Route tables and Internet Gateway
-   [x] NAT Gateway
-   [x] Security Groups
-   [x] EC2 application tier
-   [x] Application Load Balancer
-   [x] Target Group and health checks
-   [x] Auto Scaling Group
-   [x] Amazon RDS database tier
-   [x] IAM
-   [x] CloudWatch monitoring
-   [x] Application testing
-   [x] AWS resource cleanup after completion

## Architecture Summary

Internet traffic was received by the Application Load Balancer and
forwarded to EC2 application instances managed by an Auto Scaling Group.
The application tier communicated with the RDS database tier.

## Security

Security Groups were used to control traffic between the different
tiers. The database tier was separated from direct public access.

## Availability

The project demonstrated an Application Load Balancer and Auto Scaling
Group to improve application availability and provide instance
replacement/scaling capabilities.

## Monitoring

CloudWatch was used to observe EC2 metrics and configure
monitoring/alarms.

## Cleanup

After the project was completed and tested, the AWS resources were
deleted to prevent unnecessary charges.

## Learning Outcomes

This project provided practical experience with AWS networking, compute,
load balancing, scaling, databases, IAM, monitoring, security groups,
and cloud troubleshooting.
