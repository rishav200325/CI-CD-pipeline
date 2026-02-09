# Full CI/CD Pipeline Project

Includes Jenkins, GitHub Actions, Docker, AWS EC2 & ECR.

A production-grade CI/CD pipeline demonstrating automated build, test, containerization, and deployment of a Flask application using Jenkins, GitHub Actions, Docker, and AWS (EC2 & ECR).

📌 Project Overview

This project showcases how modern DevOps pipelines are built and deployed in real-world environments.
Every code push triggers automated testing, Docker image creation, and deployment to AWS infrastructure without manual intervention.

🛠 Tech Stack
Category	Technologies
Programming	Python
Web Framework	Flask
CI/CD	Jenkins, GitHub Actions
Containerization	Docker
Cloud	AWS EC2, AWS ECR
Testing	Pytest
Version Control	Git, GitHub

🏗 Architecture Flow

Developer Push → GitHub
              → Jenkins / GitHub Actions
              → Automated Tests (Pytest)
              → Docker Image Build
              → Push Image to AWS ECR
              → Deploy Container on AWS EC2
📂 Project Structure

ci-cd-flask-full/
├── app/
│   ├── app.py
│   └── __init__.py
├── tests/
│   └── test_app.py
├── .github/workflows/
│   └── ci-cd.yml
├── Dockerfile
├── Jenkinsfile
├── requirements.txt
├── .gitignore
└── README.md

⚙️ CI/CD Features
✔ Continuous Integration

Automated dependency installation

Unit testing using Pytest

Build validation on every GitHub push

✔ Continuous Deployment

Docker image creation

Secure image storage in AWS ECR

Automatic deployment to AWS EC2

✔ Multiple CI/CD Tools

Jenkins for traditional pipeline setup

GitHub Actions for cloud-native automation

▶️ Run Locally
pip install -r requirements.txt
python app/app.py

Open in browser:

http://localhost:5000

🐳 Run Using Docker
docker build -t flask-ci-cd-app .
docker run -p 5000:5000 flask-ci-cd-app

☁️ AWS Deployment

Docker images are pushed to AWS Elastic Container Registry (ECR)

EC2 instance pulls the latest image and runs the container

Deployment is fully automated via CI/CD pipeline

🧠 What This Project Demonstrates

End-to-end DevOps pipeline implementation

Cloud-ready Dockerized application

Secure and automated deployments

Industry-standard CI/CD practices

