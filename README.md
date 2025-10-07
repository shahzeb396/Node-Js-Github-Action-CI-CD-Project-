# 🚀 Node.js CI/CD Pipeline with GitHub Actions, Docker & AWS EC2

## 📌 Project Overview
This project demonstrates a **complete CI/CD pipeline** for a Node.js + Express app using **GitHub Actions**, **Docker**, and **AWS EC2**.  
The workflow automates build, test, Docker image creation, push to Docker Hub, and deployment to an EC2 instance.

---

## 🧩 Tech Stack
- **Node.js + Express** – Application backend  
- **Docker** – Containerization  
- **GitHub Actions** – CI/CD pipeline automation  
- **AWS EC2** – Hosting environment  
- **Slack Notifications** – Real-time pipeline alerts  

---

## ⚙️ Pipeline Stages
1. **Build & Test**
   - Installs dependencies and runs basic tests.
   - Uses caching for faster npm installs.
2. **Dockerize & Push**
   - Builds Docker image and pushes to Docker Hub.
3. **Deploy to AWS EC2**
   - Pulls the latest image on EC2 and runs container.
4. **Notify**
   - Sends Slack notifications on success or failure.
5. **Concurrency**
   - Cancels old runs if a new one is triggered.

---

## 🧠 GitHub Actions Concepts Used
- **Caching** → Speeds up builds by reusing npm packages.  
- **Artifacts** → Optional: store build logs or reports.  
- **Secrets** → Stores AWS, Docker, and Slack credentials securely.  
- **Concurrency** → Prevents duplicate job runs.  
- **Slack Notifications** → Real-time success/failure updates.  

