🚀 PhotoShare – AWS Cloud Architecture Project
This project demonstrates a secure, scalable, serverless-ready 3-tier AWS architecture for a photo sharing application using modern cloud best practices.
#🏗️ Architecture Overview

Built using:

* Amazon Web Services VPC (Public + Private Subnets)
* Amazon Web Services (Docker-based Web Server)
* Amazon Web Services (MySQL database in private subnet)
* Amazon Web Services (Image storage)
* Amazon Web Services (Serverless image metadata processing)
* Amazon Web Services (Traffic routing)
* Amazon Web Services + KMS (secure credentials)
* Amazon Web Services (monitoring & alerts)
* IAM Roles for secure access control


#🔐 Key Features

* No hardcoded credentials (Secrets Manager)
* Private database (no public access)
* Serverless image processing (Lambda)
* Scalable containerized backend (Docker on EC2)
* Centralized monitoring (CloudWatch)
* Load-balanced web traffic (ALB)


#⚙️ Deployment Flow
* User uploads image via ALB
* EC2 processes request (Docker app)
* Image stored in S3
* Lambda triggered for metadata extraction
* Data stored in RDS MySQL

