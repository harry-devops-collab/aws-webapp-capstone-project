# AWS Highly Available Web Application Deployment

## Project Overview
This project demonstrates deployment of a highly available web application on AWS using:

- Amazon VPC
- Public Subnets
- Route Tables
- Internet Gateway
- EC2 Instance
- Apache Web Server
- AMI
- Launch Template
- Target Group
- Application Load Balancer (ALB)
- Auto Scaling Group (ASG)

The goal of this project is to build a scalable and fault-tolerant architecture.

---

## Architecture
User → Application Load Balancer → Target Group → EC2 Instances → Auto Scaling Group

---

## AWS Services Used

### 1. VPC
Created custom VPC for isolated network.

### 2. Subnets
Created multiple public subnets in different availability zones.

### 3. Route Tables
Configured route tables for internet access.

### 4. Internet Gateway
Attached internet gateway to VPC.

### 5. EC2
Launched Ubuntu server.

### 6. Apache Web Server
Installed Apache and hosted sample website.

### 7. AMI
Created custom AMI from configured EC2.

### 8. Launch Template
Created launch template for Auto Scaling.

### 9. Target Group
Created target group for load balancer.

### 10. Application Load Balancer
Configured ALB for traffic distribution.

### 11. Auto Scaling Group
Configured ASG for high availability.

---

## Step-by-Step Implementation

### Step 1: Create VPC
Created custom VPC.
![VPC](screenshots/vpc.png)

### Step 2: Create Public Subnets
Created two public subnets.
![Subnets](screenshots/subnets.png)

### Step 3: Configure Route Table
Attached route table with internet access.
![Route Table](screenshots/route-tables.png)

### Step 4: Attach Internet Gateway
Connected VPC to Internet Gateway.
![Internet Gateway](screenshots/internet-gateway.png)

### Step 5: Launch EC2 Instance
Created EC2 instance and installed Apache.
![EC2](screenshots/ec2-instance.png)

### Step 6: Configure Apache Web Server
Hosted website on Apache.
![Apache](screenshots/apache-server.png)

### Step 7: Verify Website
Checked website in browser.
![Website](screenshots/deploy-server.png)

### Step 8: Create AMI
Created custom AMI from EC2.
![AMI](screenshots/ami.png)

### Step 9: Create Auto Scaling Group
Configured Launch Template + ASG.
![Auto Scaling Group](screenshots/auto-scaling-group.png)

### Step 10: Verify Auto Scaling
New instances launched automatically.
![Instances After Auto Scaling](screenshots/Instances-After-Auto-Scaling.png)

---

### Step 11: Create Load Balancer
Configured ALB.
![Load Balancer](screenshots/apache-2-server.png)

---

### Step 12: Configure Auto Scaling
Configured Auto Scaling Group.
![ASG](screenshots/auto-scaling-group.png)

---

## Challenges Faced

- Security group issue
- Route table association missing
- Load balancer health check issue

---

## Learning Outcomes

- AWS networking fundamentals
- EC2 deployment
- Apache hosting
- AMI creation
- Load balancing
- Auto scaling
- High availability architecture

---

## Final Result

Highly available web application deployed successfully using AWS infrastructure.

