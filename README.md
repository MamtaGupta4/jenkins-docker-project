# 🚀 CI/CD Pipeline using Jenkins, GitHub, Docker & AWS EC2

## 📌 Project Overview
This project demonstrates an end-to-end CI/CD pipeline using Jenkins, GitHub, and Docker. Whenever code is pushed to GitHub, Jenkins automatically triggers the pipeline using webhooks, builds a Docker image from a Dockerfile, and deploys it as a running container on an AWS EC2 instance. The application is hosted using Nginx and is accessible via a public IP on port 8081.

---

## ⚙️ Technologies Used
- Jenkins
- GitHub
- Docker
- AWS EC2
- Nginx
- Linux (Ubuntu)

---

## 🏗️ CI/CD Workflow
GitHub (Code Push) → Webhook Trigger → Jenkins Pipeline → Docker Image Build → Docker Container Run → AWS EC2 Deployment → Live Application

---

## 📂 Project Structure
jenkins-docker-project/  
│── Dockerfile  
│── index.html  
│── Jenkinsfile  
│── README.md  

---

## 🐳 Docker Setup
The application uses the official Nginx base image. The index.html file is copied into the Nginx default web directory, and the container exposes port 80 internally, which is mapped to port 8081 on the host machine.

---

## 🔧 Jenkins Pipeline Flow
The Jenkins pipeline performs the following steps:
1. Clone the repository from GitHub  
2. Build Docker image using Dockerfile  
3. Remove any existing container (if running)  
4. Run a new Docker container  
5. Deploy application on AWS EC2  

---

## 🔗 GitHub Webhook Integration
GitHub webhook is configured to automatically trigger Jenkins on every push to the repository.

Webhook URL:
http://<EC2-PUBLIC-IP>:8080/github-webhook/

---

## 🌐 Application Access
After successful deployment, the application is accessible at:

http://<EC2-PUBLIC-IP>:8081

---

## ✨ Features
- Fully automated CI/CD pipeline  
- GitHub webhook-based automation  
- Docker containerization  
- Jenkins automation server  
- AWS EC2 deployment  
- Zero manual deployment  

---

## 📌 Learning Outcomes
- Jenkins CI/CD pipeline setup  
- Docker image creation and containerization  
- GitHub webhook integration  
- AWS EC2 deployment  
- End-to-end DevOps workflow automation  

---

## 👩‍💻 Author
Mamta Gupta  
DevOps Engineer (Learning Phase)

---

## ⭐ Project Status
✔ Completed  
✔ CI/CD Pipeline Working  
✔ Auto Deployment Enabled  
