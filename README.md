
# AWS VPC + EC2 Web Server Project

## Overview
In this project, I designed a custom VPC, launched an EC2 instance, 
and configured an Apache web server that is accessible over the internet.

## Architecture
- Custom VPC (10.0.0.0/16)
- Public Subnet
- Internet Gateway
- Security Group (SSH + HTTP)
- EC2 Instance (Amazon Linux 2023, t2.micro)

## Steps Performed
1. Created a custom VPC using the "VPC and more" wizard
2. Configured a public subnet with a route to the Internet Gateway
3. Launched an EC2 instance in the public subnet
4. Configured a Security Group to allow SSH (22) and HTTP (80)
5. Connected via SSH using EC2 Instance Connect
6. Installed and started the Apache web server
7. Verified the web server was accessible via public IP

## Commands Used
\`\`\`bash
sudo yum update -y
sudo yum install -y httpd
sudo systemctl start httpd
sudo systemctl enable httpd
\`\`\`

## Skills Demonstrated
- VPC Networking
- EC2 Instance Management
- Security Groups Configuration
- Linux Server Administration
- Web Server Setup
