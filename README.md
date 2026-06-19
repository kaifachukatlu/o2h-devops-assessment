# 🚀 O2H DevOps Assessment

![Node.js](https://img.shields.io/badge/Node.js-18-green)
![Docker](https://img.shields.io/badge/Docker-Ready-blue)
![GitHub Actions](https://img.shields.io/badge/CI/CD-GitHub_Actions-orange)
![Status](https://img.shields.io/badge/Status-Completed-success)

---

# 📖 Overview

This repository contains my submission for the **O2H DevOps Fresher Assessment**. The assessment focuses on:

* Git & GitHub
* Linux Administration
* Docker
* CI/CD Concepts
* Bash Scripting
* Documentation

---

# 📂 Project Structure

```text
o2h-devops-assessment/
│
├── README.md
├── Dockerfile
├── Linux_Commands.md
├── script.sh
├── workflow.yml
├── app.js
├── package.json
├── package-lock.json
├── .gitignore
└── screenshots/
```

---

# 1️⃣ Task 1: Git & GitHub

## Git Workflow

* Initialized a local Git repository.
* Added project files.
* Created feature branch:

```text
feature/homepage
```

* Updated README.
* Committed changes.
* Merged feature branch into master.
* Pushed code to GitHub.

### Repository

```text
https://github.com/kaifachukatlu/o2h-devops-assessment
```

---

# 2️⃣ Task 2: Linux Administration

### Display Current User

```bash
whoami
```

### Show Disk Usage

```bash
df -h
```

### Show Memory Usage

```bash
free -m
```

### Find All .log Files

```bash
find . -name "*.log"
```

### Create Backup Folder

```bash
mkdir backup
```

### Compress Directory

```bash
tar -czvf backup.tar.gz project/
```

---

# 3️⃣ Task 3: Dockerization

## Application

A simple Node.js Express application that displays:

```text
Hello from o2h DevOps Assessment
```

### Run Application

```bash
npm install
node app.js
```

Access:

```text
http://localhost:3000
```

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

Build image:

```bash
docker build -t o2h-app .
```

Run container:

```bash
docker run -p 3000:3000 o2h-app
```

---

# 4️⃣ Task 4: CI/CD Pipeline

Implemented using GitHub Actions.

### Workflow

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

# 🎁 Bonus Task: Bash Script

```bash
#!/bin/bash

mkdir -p backup

cp *.txt backup/

echo "Backup completed successfully"
```

---

# 📸 Screenshots

The screenshots folder contains:

* Application Output
* Project Structure
* Repository Screenshots

---

# 🛠 Technologies Used

* Git
* GitHub
* Linux
* Node.js
* Express.js
* Docker
* GitHub Actions
* Bash

---

# 👨‍💻 Author

### Kaif

GitHub: https://github.com/kaifachukatlu

---

⭐ Thank you for reviewing my submission.
