# 🚀 DevOps Capstone Project — CI/CD Pipeline using Jenkins, Docker & AWS

This project demonstrates a complete **real-world CI/CD pipeline** implementation using **Jenkins, Docker, GitHub, and AWS EC2**.  
The pipeline automatically builds, tests, and deploys a containerized Python Flask application.

---

## 🏗️ Architecture Overview

GitHub → Jenkins → Docker → AWS EC2 → Live Application

---

## 🔧 Tech Stack Used

- **Cloud:** AWS EC2
- **CI/CD Tool:** Jenkins
- **Containerization:** Docker
- **Version Control:** Git & GitHub
- **Configuration Management:** Ansible *(future enhancement)*
- **Infrastructure as Code:** Terraform *(future enhancement)*
- **Application:** Python Flask

---

devops-capstone-project/
│
├── app/
│ ├── app.py
│ ├── requirements.txt
│ └── Dockerfile
│
├── jenkins/
│ └── Jenkinsfile
│
├── ansible/
│ └── (future playbooks)
│
├── terraform/
│ └── (future IaC scripts)
│
└── README.md


---

## ⚙️ CI/CD Pipeline Workflow

1. Developer pushes code to GitHub.
2. Jenkins automatically pulls latest code.
3. Jenkins builds Docker image.
4. Stops old running container.
5. Deploys new Docker container.
6. Application becomes live instantly.

---

## 🔁 Jenkins Pipeline Stages

- Checkout Source Code
- Build Docker Image
- Stop Existing Container
- Deploy New Container

---

## 🐳 Docker Workflow

- Dockerfile builds Python Flask application image.
- Jenkins builds Docker image automatically.
- Container is deployed using port **5000**.

---

## 🌍 Application Access



http://<EC2-PUBLIC-IP>:5000


---

## 🛠️ How To Run Manually

cd app 
docker build -t devops-capstone-app .
docker run -d -p 5000:5000 devops-capstone-app



## 📈 Future Enhancements

Terraform-based Infrastructure Automation

Ansible-based Configuration Management

Kubernetes Deployment (EKS)

Monitoring using Prometheus & Grafana

Logging using ELK Stack


## 🎯 Key Learnings

Jenkins CI/CD Pipeline design

Docker container lifecycle management

Real-time production debugging

GitHub + Jenkins integration

Cloud deployment using AWS EC2

👨‍💻 Author

Babil Babu
Aspiring DevOps Engineer

---


