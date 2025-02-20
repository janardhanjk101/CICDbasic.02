# CICDbasic.02
This project implements a fully automated CI/CD pipeline for a Node.js web application using Jenkins, Docker, and Ansible across multiple machines. It ensures smooth and efficient deployment by automating the build, test, and deployment process.

# CI/CD Pipeline for Node.js Application

## 📌 Overview
This project implements a fully automated **CI/CD pipeline** for a **Node.js web application** using **Jenkins, Docker, and Ansible** across multiple machines. It ensures smooth and efficient deployment by automating the build, test, and deployment process.

---

## 🚀 Architecture
The pipeline operates across **three machines**:

### 1️⃣ Development Machine (PC 1 - Windows)
- Writes and maintains the **Node.js application** using **VS Code**.
- Pushes code to **GitHub** for version control.

### 2️⃣ CI/CD Server (PC 2 - Vagrant Ubuntu on VirtualBox)
- Runs **Jenkins** for continuous integration.
- Uses **Docker** for building and testing.
- Deploys using **Ansible**.

### 3️⃣ Deployment Server (PC 3 - Vagrant Ubuntu on VirtualBox)
- Hosts the **Node.js application** in a Docker container.
- Serves the application via **port 80**.

---

## 🔄 CI/CD Workflow
1️⃣ **Code Push**: Developer pushes changes to **GitHub**.
2️⃣ **Build & Test**: Jenkins pulls the code, installs dependencies, and runs tests.
3️⃣ **Dockerization**: Jenkins builds a **Docker image** and pushes it to **Docker Hub**.
4️⃣ **Deployment via Ansible**:
   - PC 3 pulls the latest **Docker image**.
   - Stops any running container and starts the new one.
5️⃣ **Application is Live!** 🚀

---

## 🔧 Technologies Used
- **Version Control**: Git & GitHub
- **CI/CD Automation**: Jenkins
- **Containerization**: Docker
- **Configuration Management**: Ansible
- **Orchestration**: Vagrant & VirtualBox
- **Programming Language**: JavaScript (Node.js)

---

## 📌 Key Features
✔️ **Automated Build & Testing** in Jenkins  
✔️ **Containerized Deployment** using Docker  
✔️ **Infrastructure as Code (IaC)** with Ansible  
✔️ **Multi-Node Architecture** for real-world DevOps practice  
✔️ **Scalable & Reproducible Deployment**  

---

## 💡 Why This Project?
✅ **Hands-on DevOps Experience**: Simulates real-world **CI/CD workflows**.  
✅ **Showcases Key Skills**: Version control, automation, containerization, and configuration management.  
✅ **Prepares for DevOps Interviews**: Demonstrates knowledge of **Jenkins, Docker, Ansible, and CI/CD best practices**.  

---

## 📄 How to Run the Pipeline
1. Clone the **GitHub repository**.
2. Set up **PC 2 & PC 3** using **Vagrant and VirtualBox**.
3. Install **Jenkins, Docker, and Ansible** on **PC 2**.
4. Add **GitHub, Docker Hub, and SSH credentials** in Jenkins.
5. Run the **Jenkins pipeline** to automate the deployment.  

---

🚀 **Now every time you push code, it will automatically deploy!** 🎯

