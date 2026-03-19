# Jenkins CI/CD Pipeline for Apache Webpage Deployment

## Project Overview

This project demonstrates a simple **CI/CD pipeline** using **GitHub** and **Jenkins** to automatically deploy a static webpage to an **Apache web server** running on an **AWS EC2 instance**.

Whenever changes are pushed to the GitHub repository, Jenkins detects the update and deploys the latest `index.html` file to the Apache document root. This removes manual deployment and ensures the live website always reflects the latest code.

---

## Architecture

GitHub → Jenkins → EC2 Apache Server → Live Webpage

---

## Tools Used

- **GitHub** – stores the application source code
- **Jenkins** – automates the deployment pipeline
- **AWS EC2** – hosts Jenkins and Apache
- **Apache (httpd)** – serves the webpage
- **Git** – version control system

---

## Project Files

```text
jenkins-sample/
├── index.html
└── Jenkinsfile
