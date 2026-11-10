# CloudOrder – E-commerce Application on AWS

## 1. Project Overview

CloudOrder is a full-stack e-commerce application developed using Python FastAPI, PostgreSQL, HTML, CSS and JavaScript, with containerization and deployment using AWS services.

The project demonstrates how to build an application, containerize its backend, store Docker images in Amazon ECR, and run containers using Amazon ECS with AWS Fargate.

## 2. Technology Stack

| Category | Technologies |
|---|---|
| Frontend | HTML, CSS, JavaScript |
| Backend | Python, FastAPI |
| Database | PostgreSQL, pgAdmin |
| Containerization | Docker, Docker Desktop |
| Container Registry | Amazon ECR |
| Container Orchestration | Amazon ECS |
| Container Compute | AWS Fargate |
| Networking | Amazon VPC, Subnets, Route Tables, Internet Gateway, NAT Gateway |
| Cloud Platform | Amazon Web Services (AWS) |

## 3. Architecture Overview

The application follows this architecture:

**Frontend → FastAPI Backend → PostgreSQL Database**

The backend is containerized using Docker, and the Docker image is pushed to Amazon ECR.

Amazon ECS with AWS Fargate is used to run the container without managing EC2 instances.

### AWS Architecture Flow

1. Users access the CloudOrder frontend.
2. The frontend communicates with the FastAPI backend.
3. FastAPI handles application logic and database operations.
4. Docker packages the backend application into a container image.
5. Amazon ECR stores the Docker image.
6. Amazon ECS manages the container deployment.
7. AWS Fargate provides serverless container compute capacity.
8. AWS VPC networking provides network isolation and connectivity.

## 4. AWS Services Implemented

### Amazon VPC
- Created a custom VPC.
- Configured public and private subnets.
- Configured route tables and subnet associations.
- Attached an Internet Gateway.
- Created a NAT Gateway.

### Amazon ECR
- Created an ECR repository named `cloudorder-api`.
- Authenticated Docker with Amazon ECR.
- Tagged the Docker image.
- Pushed the container image to ECR.

### Amazon ECS and AWS Fargate
- Used Amazon ECS to manage container workloads.
- Used AWS Fargate as the serverless compute engine for containers.
- Configured container deployment using the Docker image stored in Amazon ECR.
- Explored task definitions, services and container networking.

## 5. Docker Implementation

Docker was used to package the FastAPI backend and its dependencies.

Implementation included:
- Creating a Dockerfile.
- Building the Docker image.
- Running and testing containers locally.
- Tagging the image for Amazon ECR.
- Pushing the image to the ECR repository.

## 6. Project Screenshots

Screenshots demonstrating the actual implementation are available in the `screenshots` folder.

Suggested screenshots:

- `screenshots/website.png`
- `screenshots/backend-api.png`
- `screenshots/postgresql.png`
- `screenshots/docker.png`
- `screenshots/ecr.png`
- `screenshots/ecs-cluster.png`
- `screenshots/fargate-task.png`
- `screenshots/vpc.png`
- `screenshots/subnets.png`
- `screenshots/nat-gateway.png`

## 7. Challenges and Learnings

During this project, I gained practical experience with:

- Connecting a frontend to a FastAPI backend.
- Integrating PostgreSQL with Python.
- Containerizing applications using Docker.
- Troubleshooting Docker Desktop connectivity.
- Building and pushing Docker images to Amazon ECR.
- Understanding ECS clusters, task definitions and services.
- Running containers using AWS Fargate.
- Configuring AWS VPC networking and subnet routing.

## 8. Security Considerations

- Used AWS IAM roles for service access.
- Applied Security Groups to control network traffic.
- Avoided exposing database credentials.
- Kept sensitive configuration and `.env` files out of GitHub.
- Followed least-privilege access principles where applicable.

## 9. Future Enhancements

Potential improvements include:

- Configure an Application Load Balancer for application traffic.
- Use Amazon RDS for managed PostgreSQL.
- Host frontend assets using Amazon S3 and CloudFront.
- Implement CI/CD using GitHub Actions.
- Add CloudWatch monitoring and logging.
- Improve deployment automation and application scalability.

## 10. Skills Demonstrated

- Full-stack application development.
- Python and FastAPI.
- PostgreSQL database integration.
- Docker containerization.
- Amazon ECR image management.
- Amazon ECS and AWS Fargate.
- AWS VPC and networking fundamentals.
- Cloud deployment and troubleshooting.

## 11. Project Summary

CloudOrder demonstrates practical experience in developing and containerizing a full-stack e-commerce application and working with AWS container services. The project provided hands-on exposure to Amazon ECR, Amazon ECS, AWS Fargate and AWS networking concepts.
