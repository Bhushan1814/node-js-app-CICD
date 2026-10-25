# 🚀 Node.js Application Deployment Using Jenkins CI/CD

## 📌 Project Overview

This project demonstrates automated deployment of a Node.js application using a Jenkins CI/CD pipeline. The application source code is stored in GitHub and deployed to a Linux target server using SSH, SCP, and PM2.

## 🏗️ Architecture

text
Developer
    |
    v
GitHub Repository
    |
    v
Jenkins CI/CD Pipeline
    |
    v
Checkout Source Code
    |
    v
Install Dependencies
    |
    v
Run Tests
    |
    v
SSH / SCP File Transfer
    |
    v
Ubuntu EC2 Target Server
    |
    v
Install Production Dependencies
    |
    v
PM2 Process Management
    |
    v
Node.js Application
    |
    v
Health Check (/health)


## 🛠️ Technologies Used

* Node.js – Application development
* Express.js – Web framework
* Git and GitHub – Source code management
* Jenkins – CI/CD automation
* Linux (Ubuntu) – Target server
* AWS EC2 – Cloud infrastructure
* SSH and SCP – Secure server communication
* PM2 – Application process management
* npm – Dependency management

## ⚙️ CI/CD Workflow

1. Develop the Node.js application.
2. Push source code to GitHub.
3. Jenkins checks out the repository.
4. Install dependencies and run tests.
5. Connect to the target server through SSH.
6. Transfer application files using SCP.
7. Install production dependencies on the target server.
8. Start or restart the application using PM2.
9. Verify deployment using the health endpoint.

## 📁 Project Structure

text
node-js-app-CICD/
├── app.js
├── package.json
├── Jenkinsfile
└── README.md


## 🔐 Security

* Store SSH private keys in Jenkins Credentials.
* Restrict SSH access to trusted sources.
* Never upload private keys, passwords, or tokens to GitHub.
* Configure AWS EC2 security groups with minimum required access.

## ✅ Deployment Verification

After a successful deployment, test the following endpoints:

* Application: http://YOUR_SERVER_PUBLIC_IP:3000/
* Health check: http://YOUR_SERVER_PUBLIC_IP:3000/health

Replace YOUR_SERVER_PUBLIC_IP with the actual public IP of your target server. Ensure the relevant security-group rules permit access.

## 🧠 Key Learnings

* Jenkins Declarative Pipeline configuration
* GitHub integration with Jenkins
* Automated application deployment
* Linux server administration
* SSH-based secure file transfer
* PM2 process management
* Deployment verification and troubleshooting

## 👨‍💻 Author

*Bhushan Jagtap*

AWS Cloud & DevOps Enthusiast

## 🏷️ Tags

Jenkins CI/CD DevOps Node.js GitHub Linux AWS EC2 SSH PM2 Automation
