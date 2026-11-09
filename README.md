# CloudOrder – E-commerce Application

## Project Overview
CloudOrder is an e-commerce application developed to learn full-stack development, containerization and AWS cloud deployment.

## Technologies Used
- Frontend: HTML, CSS, JavaScript
- Backend: Python FastAPI
- Database: PostgreSQL
- Database Management: pgAdmin
- Containerization: Docker
- Container Registry: Amazon ECR
- Cloud Infrastructure: AWS VPC, Subnets, Internet Gateway, NAT Gateway

## Architecture
Frontend → FastAPI Backend → PostgreSQL Database

Docker is used to containerize the backend, and Amazon ECR stores the Docker image.

## AWS Implementation
- Created a VPC.
- Configured public and private subnets.
- Configured route tables.
- Created an Internet Gateway.
- Configured a NAT Gateway.
- Created an Amazon ECR repository.
- Built and pushed the Docker image to ECR.

## Screenshots
Project screenshots are available in the `screenshots` folder.

## Learning Outcomes
- Full-stack application development.
- Docker containerization.
- AWS networking fundamentals.
- Container image management using Amazon ECR.
