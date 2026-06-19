# O2H DevOps Assessment

Completed by **Kaif**

## 📌 Overview

This repository contains the solutions for the **O2H DevOps Fresher Assessment**. The assessment covers Git & GitHub, Linux fundamentals, Docker, CI/CD concepts, troubleshooting, and Bash scripting.

---

## 🚀 Technologies Used

* Git & GitHub
* Node.js
* Express.js
* Docker
* GitHub Actions
* Linux Commands
* Bash Scripting

---

## 📂 Project Structure

```text
o2h-devops-assessment/
│
├── README.md
├── app.js
├── package.json
├── package-lock.json
├── Dockerfile
├── Linux_Commands.md
├── script.sh
├── workflow.yml
├── .gitignore
└── screenshots/
```

---

## 🌐 Application

### app.js

The application is a simple Express server that returns:

```text
Hello from o2h DevOps Assessment
```

The application runs on:

```text
http://localhost:3000
```

---

## 🐳 Docker

### Dockerfile

```dockerfile
FROM node:18

WORKDIR /app

COPY package*.json ./

RUN npm install

COPY . .

EXPOSE 3000

CMD ["node", "app.js"]
```

### Docker Commands

Build Docker image:

```bash
docker build -t o2h-app .
```

Run Docker container:

```bash
docker run -p 3000:3000 o2h-app
```

---

## ⚙️ CI/CD Pipeline

A basic GitHub Actions workflow has been created.

Pipeline flow:

```text
Developer Push
       ↓
GitHub
       ↓
Build
       ↓
Install Dependencies
       ↓
Run Tests
       ↓
Docker Build
```

---

## 🌿 Git Branching Strategy

### Branch Created

```text
feature/homepage
```

Workflow followed:

1. Created local repository.
2. Added project files.
3. Created feature branch.
4. Modified README.
5. Committed changes.
6. Merged into master branch.
7. Pushed to GitHub.

---

## 🐧 Linux Commands

Display current user:

```bash
whoami
```

Show disk usage:

```bash
df -h
```

Show memory usage:

```bash
free -m
```

Find log files:

```bash
find . -name "*.log"
```

Create backup folder:

```bash
mkdir backup
```

Compress directory:

```bash
tar -czvf backup.tar.gz project/
```

---

## 📜 Bash Script

```bash
#!/bin/bash

mkdir -p backup

cp *.txt backup/

echo "Backup completed successfully"
```

---

# Troubleshooting

## Scenario 1: Docker Container Exits Immediately

### Possible Reasons

* Application crashes during startup.
* Incorrect CMD instruction.
* Missing dependencies.
* Port configuration issue.

### Debug Commands

```bash
docker ps -a
docker logs <container_id>
docker exec -it <container_id> sh
```

---

## Scenario 2: Application Works Locally but Not on Server

### Things to Check

* Firewall rules.
* Port accessibility.
* Environment variables.
* Dependencies installed.
* Application logs.

### Commands

```bash
netstat -tulpn
docker logs <container_id>
curl localhost:3000
```

---

# Interview Questions

## Difference between Docker Image and Container

* Docker Image is a blueprint or template.
* Docker Container is a running instance of an image.

---

## What is CI/CD?

**CI (Continuous Integration):**

Automates code integration and testing.

**CD (Continuous Deployment):**

Automates deployment and delivery processes.

---

## What Happens During docker build?

Docker reads instructions from the Dockerfile and creates image layers step by step.

---

## Difference Between CMD and ENTRYPOINT

* CMD provides default commands.
* ENTRYPOINT makes the container behave like an executable.

---

## What is Infrastructure as Code (IaC)?

Infrastructure as Code is the practice of managing and provisioning infrastructure using code and automation tools such as Terraform and Ansible.

---

## How GitHub Actions Work

GitHub Actions automatically run workflows whenever code is pushed to the repository. It helps automate build, test, and deployment tasks.

---

## What Would You Automate First in a Software Project?

I would automate:

* Build process
* Testing process
* Deployment process
* Backup and monitoring tasks

---

## 👨‍💻 Author

**Kaif**

GitHub: https://github.com/kaifachukatlu

---
