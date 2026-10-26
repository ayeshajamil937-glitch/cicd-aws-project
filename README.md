# cicd-aws-project
This is my CI-CD PROJECT 
🚀 CI/CD Pipeline with Docker, GitHub Actions, and AWS EC2

📌 Project Overview

This project demonstrates how to build a Dockerized web application and prepare an automated Continuous Integration and Continuous Deployment (CI/CD) pipeline using GitHub Actions, Docker, Docker Hub, and AWS EC2.

The application uses Nginx to serve a custom HTML webpage inside a Docker container. The goal is to automate the process of building the Docker image, pushing it to Docker Hub, and deploying the updated application to an AWS EC2 instance.

🛠️ Technologies Used

Docker — Containerization of the web application

Nginx — Web server for serving HTML content

Git & GitHub — Source code management

GitHub Actions — CI/CD workflow automation

Docker Hub — Docker image registry

AWS EC2 — Cloud hosting and deployment target

PowerShell — Local development and Docker commands

🏗️ Project Architecture

Developer
    |
    v
GitHub Repository
    |
    v
GitHub Actions Workflow
    |
    v
Build Docker Image
    |
    v
Push Image to Docker Hub
    |
    v
Deploy to AWS EC2
    |
    v
Docker Container (Nginx)
    |
    v
Web Application

📂 Project Structure

cicd-aws-project/
│
├── .github/
│   └── workflows/
│       └── dev.yaml
│
├── app/
│   └── index.html
│
├── Dockerfile
├── .gitignore
└── README.md

Note: The workflow file and other listed files should be present in the repository before considering this structure complete.

🌐 Application Details

The application displays a custom HTML webpage served by Nginx.

Base Image: nginx:alpine

Container Port: 80

Local Port: 3000

Local URL: http://localhost:3000

🐳 Docker Setup

Build the Docker Image

docker build -t cicd-demo .

Run the Container

docker run -d --name cicd-demo -p 3000:80 cicd-demo

Check Running Containers

docker ps

Open the Application

Visit:

http://localhost:3000

Stop the Container

docker stop cicd-demo

Remove the Container

docker rm cicd-demo

⚙️ CI/CD Pipeline

The planned automated pipeline will perform the following tasks:

Source Code Management: Store application code in GitHub.

Continuous Integration: Trigger GitHub Actions when code is pushed.

Docker Build: Build the application image using the Dockerfile.

Image Publishing: Push the image to Docker Hub.

Continuous Deployment: Connect to AWS EC2 and deploy the latest image.

Application Verification: Confirm that the application is running successfully.

🔐 Security

Store Docker Hub credentials and deployment secrets in GitHub Actions Secrets.

Never commit AWS private keys, passwords, access tokens, or sensitive .env files.

Use SSH keys for secure access to AWS EC2.

Restrict EC2 security group rules to trusted sources wherever possible.

📊 Project Status

✅ Completed

Created the project directory.

Created the HTML application.

Prepared the Dockerfile for Nginx.

Uploaded the project to GitHub.

🔄 In Progress / Planned

Verify the local Docker image and container.

Create a Docker Hub repository.

Configure GitHub Actions workflow.

Add GitHub repository secrets.

Launch and configure an AWS EC2 instance.

Automate deployment from GitHub Actions to EC2.

Test the complete CI/CD pipeline.

Update these sections as each stage is successfully completed.

🎯 Learning Objectives

Understand the fundamentals of CI/CD.

Containerize a web application using Docker.

Manage source code with Git and GitHub.

Automate builds using GitHub Actions.

Publish Docker images to Docker Hub.

Deploy containerized applications to AWS EC2.

Practice secure cloud deployment.

👩‍💻 Author

Ayesha Jamil

DevOps Engineering Practice Project

⭐ This project is part of my hands-on learning journey in Docker, CI/CD automation, GitHub Actions, and AWS cloud deployment.
