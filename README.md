# 🚀 CI/CD Pipeline using GitHub Actions & Docker

This project demonstrates how to set up a complete CI/CD pipeline using **GitHub Actions** and **Docker** to build and run a simple **Flask** application — completely on your **local machine**, with no cloud services involved.

---

## ✨ Project Features

- 🐍 Simple Python Flask web app
- 🐳 Dockerized with a custom `Dockerfile`
- 🔁 CI/CD pipeline using GitHub Actions
- 🖥️ Runs entirely on local machine (`localhost:5000`)

---

## 📁 Project Structure
my-app/
├── app.py
├── requirements.txt
├── Dockerfile
└── .github/
└── workflows/
└── ci-cd.yml

---

## 🛠️ Setup Instructions

### 🔹 Step 1: Clone the Repo

Copy this👇
git clone https://github.com/<your-username>/my-app.git
cd my-app
### 🔹 Step 2: Build Docker Image Locally
Copy this👇
docker build -t my-local-app .
### 🔹 Step 3: Run Docker Container
Copy this👇
docker run -d -p 5000:5000 my-local-app
### 🔹 Step 4: Open in Browser
Visit:http://localhost:5000
### ✅ You should see:

### "Hello beautiful people have a nice day"

⚙️ CI/CD with GitHub Actions
This project uses a GitHub Actions workflow file:

.github/workflows/ci-cd.yml

It automatically builds the Docker image when code is pushed to the main branch.

