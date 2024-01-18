# Multi-tier Web Architecture with Load Balancing & Auto-Scaling

I have successfully deployed a multi-tier web architecture using load balancing and auto-scaling. This configuration enhances the reliability and scalability of the client's web application. The following steps were taken during the implementation:

## Project Overview

The objective of this project was to create a scalable and reliable infrastructure to support a web application. Key features of the deployment include:

- **VPC Creation:** Established a Virtual Private Cloud (VPC) with two public and two private subnets, configured with a single CIDR block.

- **Elastic Load Balancer (ELB):** Created an Elastic Load Balancer with a security group to enable internet users to access the HTTP web server page via the relevant port.

- **EC2 Security Group Configuration:** Configured a separate security group for EC2 instances, allowing web traffic only from the ELB.

- **Auto-Scaling:** Launched auto-scaling using a WordPress AMI from the AWS Marketplace to ensure dynamic scaling based on demand.

- **Auto-Scaling Launch Group:** Configured the auto-scaling launch group with minimum, maximum, and desired values set to 2. EC2 instances were launched in a private subnet and made available behind the ELB after launching.

- **Notifications:** Set up notifications to receive alerts on create, terminate, and failed events via email and SMS using the AWS Notification Service.

- **ELB DNS Verification:** Checked the ELB DNS on a web browser to ensure accessibility to the WordPress website.

## Technology Stack

- **AWS Services:**
  - Amazon VPC
  - Elastic Load Balancer (ELB)
  - EC2 Instances
  - Auto-Scaling
  - AWS Marketplace (WordPress AMI)
  - AWS Notification Service

## Deployment Process

The deployment process focused on creating a scalable and reliable architecture, utilizing AWS services to ensure optimal performance.

## Notifications

Alerts for various events, including instance creation, termination, and failures, were configured to keep administrators informed in real-time.

## Accessibility

The ELB DNS was verified on a web browser, confirming the successful accessibility of the WordPress website.

## Conclusion

This project successfully implemented a multi-tier web architecture with load balancing and auto-scaling, providing a robust and scalable infrastructure for the client's web application.

