CloudFormation Template Docker Container WordPress
===============================================

Docker Containers can be used to quickly deploy a stack for testing. I have created a CloudFormation Template and uploaded to my Github repo. You can follow the instructions below to download and run the template in your AWS account. 

The CloudFormation Template will create the following resources
-----------------------------------------------------------------

- EC2 Instance
- Security Group

The User Data Section Script will configure the following
---------------------------------------------------------

- Install Docker
- Install Git
- Install Docker-Compose
- Generates docker-compose.yml file
- Download and run the WordPress Site in a Docker Container


Usage
-----
```
1. Download the CFT to a local directory  https://github.com/roymjia/EC2-bootstrap-docker-container-wordpress/blob/master/cft-ec2-docker-container.yaml
2. Log into AWS Console and to CloudFormation.
3. Click on "Create Stack" 
4. From the "Choose a Template" section, click on "Choose File" and select the previously downloaded "cft-ec2-docker-container.yaml" file. 
5. Input the required parameters and create the stack.
6. After the stack has been created, navigate to <public ip>:8000 to view your WordPress Site.
 ```
