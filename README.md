# 🚀 Jenkins CI/CD Pipeline Project

## 📌 Project Overview
This project demonstrates the implementation of a **CI/CD (Continuous Integration and Continuous Deployment) pipeline** using Jenkins, GitHub, and Docker. The pipeline automates source code retrieval, Docker image building, and deployment of a web application.

## 🎯 Project Objectives
- Automate application build and deployment.
- Integrate GitHub with Jenkins.
- Build Docker images automatically.
- Push Docker images to Docker Hub.
- Simplify the software delivery process.

## 🛠️ Technologies Used

| Technology | Purpose |
|---|---|
| AWS EC2 | Cloud server infrastructure |
| Linux | Operating system |
| Git & GitHub | Source code management |
| Jenkins | CI/CD automation |
| Docker | Containerization |
| Docker Hub | Docker image repository |
| Shell Script | Pipeline automation |
| HTML & CSS | Web application |

## 🏗️ Project Architecture

Developer → GitHub → Jenkins → Docker Build → Docker Hub → Deployment

## ⚙️ Project Workflow

1. **Source Code:** Store application files in a GitHub repository.
2. **Jenkins Setup:** Install and configure Jenkins on an AWS EC2 instance.
3. **GitHub Integration:** Connect the GitHub repository to Jenkins.
4. **Pipeline Execution:** Configure Jenkins to execute the build script.
5. **Docker Build:** Build a Docker image using the Dockerfile.
6. **Image Push:** Authenticate with Docker Hub and push the image.
7. **Deployment:** Run the Docker container to serve the web application.

## 📂 Project Structure

```text
MY-CICD-PROJECT/
├── index.html
├── Dockerfile
├── deploy.sh
└── README.md
```

## 🚀 How to Run the Project

### Step 1: Clone the Repository

```bash
git clone YOUR_GITHUB_REPOSITORY_URL
cd MY-CICD-PROJECT
```

Replace `YOUR_GITHUB_REPOSITORY_URL` with your actual GitHub repository URL.

### Step 2: Build the Docker Image

```bash
docker build -t cloud-messenger-netflix:latest .
```

### Step 3: Run the Docker Container

```bash
docker run -d --name cloud-messenger-web -p 8081:80 cloud-messenger-netflix:latest
```

### Step 4: Access the Application

Open your browser and visit:

```text
http://YOUR_EC2_PUBLIC_IP:8081
```

Ensure the EC2 security group allows inbound TCP traffic on port `8081`.

## 🔐 Security Best Practices

- Store Docker Hub credentials in Jenkins Credentials.
- Never commit passwords, access tokens, or AWS secret keys to GitHub.
- Restrict Jenkins access to authorized users.
- Allow only necessary inbound ports in AWS security groups.
- Use secure credential management for automated deployments.

## 📈 Project Benefits

- Reduces manual deployment effort.
- Improves consistency and repeatability.
- Enables faster application delivery.
- Demonstrates practical cloud and DevOps skills.
- Provides hands-on experience with CI/CD automation.

## 👨‍💻 Skills Demonstrated

AWS EC2 | Linux | Git | GitHub | Jenkins | Docker | Docker Hub | CI/CD | Shell Scripting

## 🏁 Conclusion

This project demonstrates how Jenkins, GitHub, Docker, and AWS EC2 can work together to automate the build and delivery of a web application. It provides practical experience with essential tools used in modern Cloud and DevOps engineering.

---
**Project Category:** Cloud & DevOps

**Author:** Mayur Chaudhari
