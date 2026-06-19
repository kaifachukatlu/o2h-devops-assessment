# 🚀 O2H DevOps Assessment

![Node.js](https://img.shields.io/badge/Node.js-18-green)
![Docker](https://img.shields.io/badge/Docker-Ready-blue)
![GitHub Actions](https://img.shields.io/badge/CI/CD-GitHub_Actions-orange)
![Status](https://img.shields.io/badge/Status-Completed-success)

## 📖 Overview

This repository contains my submission for the **O2H DevOps Fresher Assessment**. The assessment demonstrates fundamental knowledge of:

* Git & GitHub
* Linux Administration
* Docker
* CI/CD Concepts
* Bash Scripting
* Documentation

---

# 🛠 Technologies Used

* Git
* GitHub
* Node.js
* Express.js
* Docker
* GitHub Actions
* Linux
* Bash

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

# 🌐 Application

A simple Node.js Express application that displays:

```text
Hello from o2h DevOps Assessment
```

Run the application:

```bash
npm install
node app.js
```

Access:

```text
http://localhost:3000
```

---

# 🐳 Docker

## Dockerfile

```dockerfile
FROM node:18

WORKDIR /app

COPY package*.json ./

RUN npm install

COPY . .

EXPOSE 3000

CMD ["node", "app.js"]
```

## Docker Commands

Build Docker Image:

```bash
docker build -t o2h-app .
```

Run Docker Container:

```bash
docker run -p 3000:3000 o2h-app
```

---

# ⚙️ CI/CD Workflow

Implemented using GitHub Actions.

Pipeline Flow:

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

# 🌿 Git Workflow

* Initialized local Git repository.
* Added project files.
* Created feature branch:

```text
feature/homepage
```

* Modified README.
* Committed changes.
* Merged feature branch into master.
* Pushed code to GitHub.

---

# 🐧 Linux Commands

Current User:

```bash
whoami
```

Disk Usage:

```bash
df -h
```

Memory Usage:

```bash
free -m
```

Find Log Files:

```bash
find . -name "*.log"
```

Create Backup Folder:

```bash
mkdir backup
```

Compress Directory:

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

# 📸 Screenshots

The `screenshots/` folder contains:

* Application output
* Project structure
* Repository screenshots

---

# 👨‍💻 Author

**Kaif**

GitHub: https://github.com/kaifachukatlu

---

⭐ Thank you for reviewing my submission.
