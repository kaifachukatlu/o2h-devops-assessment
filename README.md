# 🚀 O2H DevOps Assessment

![Node.js](https://img.shields.io/badge/Node.js-18-green)
![Docker](https://img.shields.io/badge/Docker-Ready-blue)
![GitHub Actions](https://img.shields.io/badge/CI/CD-GitHub_Actions-orange)
![License](https://img.shields.io/badge/Status-Completed-success)

## 📖 Overview

This repository contains my submission for the **O2H DevOps Fresher Assessment**. The assessment demonstrates fundamental knowledge of:

* Git & GitHub
* Linux Administration
* Docker
* CI/CD concepts
* Bash Scripting
* Troubleshooting

---

# 📂 Project Structure

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

# 🛠 Technologies Used

* Git & GitHub
* Node.js
* Express.js
* Docker
* GitHub Actions
* Linux Commands
* Bash

---

# 🌐 Application

Simple Node.js Express server:

```javascript
const express = require('express');
const app = express();

app.get('/', (req, res) => {
    res.send('Hello from o2h DevOps Assessment');
});

app.listen(3000);
```

Application runs at:

```text
http://localhost:3000
```

---

# 🐳 Docker

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

### Commands

Build image:

```bash
docker build -t o2h-app .
```

Run container:

```bash
docker run -p 3000:3000 o2h-app
```

---

# ⚙ CI/CD Workflow

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

Implemented using **GitHub Actions**.

---

# 🌿 Git Workflow

* Created local repository.
* Added project files.
* Created branch:

```text
feature/homepage
```

* Updated README.
* Committed changes.
* Merged branch into master.
* Pushed code to GitHub.

---

# 🐧 Linux Commands

Current user:

```bash
whoami
```

Disk usage:

```bash
df -h
```

Memory usage:

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

# 📜 Bash Script

```bash
#!/bin/bash

mkdir -p backup

cp *.txt backup/

echo "Backup completed successfully"
```

---

# 🔧 Troubleshooting

## Scenario 1: Docker Container Exits Immediately

### Possible Reasons

* Application crash
* Incorrect CMD instruction
* Missing dependencies
* Port conflicts

### Debug Commands

```bash
docker ps -a
docker logs <container_id>
docker exec -it <container_id> sh
```

---

## Scenario 2: Application Works Locally but Not on Server

### Things to Check

* Firewall rules
* Port accessibility
* Environment variables
* Dependencies
* Logs

### Commands

```bash
netstat -tulpn
docker logs <container_id>
curl localhost:3000
```

---

# 📚 Interview Questions

### Docker Image vs Container

* Image → Blueprint.
* Container → Running instance.

### What is CI/CD?

* Continuous Integration
* Continuous Deployment

### What Happens During Docker Build?

Docker reads the Dockerfile and creates image layers.

### CMD vs ENTRYPOINT

* CMD provides default commands.
* ENTRYPOINT makes containers executable.

### Infrastructure as Code

Managing infrastructure through code and automation tools.

### GitHub Actions

Automates build, test, and deployment workflows.

### What Would You Automate First?

* Build process
* Testing process
* Deployment process
* Monitoring

---

# 👨‍💻 Author

### Kaif

GitHub: https://github.com/kaifachukatlu

---

⭐ Thank you for reviewing my submission.
