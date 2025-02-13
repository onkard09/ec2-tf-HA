# Secure and Scalable Web Server on EC2 with Load Balancing and Auto Scaling
## Problem Statement:
You are working for a startup that is launching a web application. They need a highly available and scalable solution using AWS EC2, where traffic is distributed efficiently, and the setup follows best security practices.
Your task is to:
- Launch two EC2 instances in different availability zones within a VPC. The instances should:
  - Run an Nginx or Apache web server.
  - Serve a basic static HTML page.
  - Use a custom security group allowing only HTTP (port 80) and SSH (port 22) from your IP.
- Create and attach an Application Load Balancer (ALB) that:
  - Distributes traffic between the two instances.
  - Uses a target group with health checks to ensure availability.
- Implement Auto Scaling to:
  - Scale the instances up when CPU utilization exceeds 50%.
  - Scale down when utilization is below 20%.
- Secure the setup by:
  - Restricting SSH access to your own IP only.
  - Using IAM roles to provide EC2 instances with read-only access to S3 (for future logs).
- Test the setup:
  - Fetch the ALB DNS name and verify that it correctly serves the static page.
  - Simulate CPU stress to trigger Auto Scaling.
- Bonus Challenges (Optional):
  - Use Terraform or AWS CloudFormation to automate the setup.
  - Enable HTTPS using an SSL certificate from AWS Certificate Manager (ACM).
  - Store access logs in S3 for monitoring.
  - Set up CloudWatch Alarms to notify you when an instance is unhealthy.
 
  
