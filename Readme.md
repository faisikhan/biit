# Learning Containerization & CICD together.

This is a Node JS app by DigitalOcean to build and run a Node JS appliation on a Docker image with the help of Dockerfile. 

So we are containerizing the application and pushing it to ECR and deploying it on AWS App Runner or ECS. We're going to cover both manual and automatic deployments.

# Requirements

## AWS CLI

We can install AWS CLI on Linux with the help of the following commands:

`curl "https://awscli.amazonaws.com/awscli-exe-linux-x86_64.zip" -o "awscliv2.zip"`

`unzip awscliv2.zip`

`./aws/install --bin-dir /usr/local/bin --install-dir /usr/local/aws-cli --update`

## Install Docker

Docker installation is simple and can be installed with the following two commands:

`apt update`

`apt install docker.io`

## Configure IAM User Credentials

`aws configure`

It will ask for the Access Key and Secret Access Key.

## Login to ECR

`aws ecr get-login-password --region us-east-1 | docker login --username AWS --password-stdin 559050236729.dkr.ecr.us-east-1.amazonaws.com`



