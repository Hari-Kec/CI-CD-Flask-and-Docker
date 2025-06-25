# CI/CD for Flask Docker Application 🚀

![GitHub](https://img.shields.io/github/license/Hari-Kec/CI-CD-Flask-and-Docker?style=flat-square)
![Docker](https://img.shields.io/badge/Docker-✔-blue?style=flat-square&logo=docker)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-✔-2088FF?style=flat-square&logo=github-actions)
![Python](https://img.shields.io/badge/Python-3.9-3776AB?style=flat-square&logo=python)
![Flask](https://img.shields.io/badge/Flask-2.0-000000?style=flat-square&logo=flask)

A simple Flask application with Docker containerization and CI/CD pipeline using GitHub Actions.

## Features ✨

- 🐳 Docker containerization
- ⚙️ Automated CI/CD pipeline with GitHub Actions
- 🧪 Automated testing with pytest
- 🔄 Automatic build and push to Docker Hub
- 📦 Easy deployment with Docker

## Prerequisites 📋

- Docker installed
- Python 3.9+
- GitHub account
- Docker Hub account (for image publishing)

## Project Structure 📂
CI-CD-Flask-and-Docker/
├── app.py # Main Flask application
├── DockerFile # Docker configuration
├── .github/
│ └── workflows/
│ └── cicd.yml # GitHub Actions workflow
├── requirements.txt # Python dependencies
└── README.md # Project documentation


## Setup and Installation 🛠️

### Local Development

1. Clone the repository:
   ```bash
   git clone https://github.com/Hari-Kec/CI-CD-Flask-and-Docker.git
   cd CI-CD-Flask-and-Docker
### Build and Run
   docker build -t flask-app .

   docker run -p 5000:5000 flask-app

CI/CD Pipeline
The GitHub Actions workflow performs the following steps automatically on push to main branch:

🏗️ Builds Docker image

🧪 Runs tests

🐳 Builds and pushes image to Docker Hub

Configuration ⚙️
GitHub Secrets
Set these secrets in your GitHub repository settings:

DOCKER_USERNAME - Your Docker Hub username

DOCKER_PASSWORD - Your Docker Hub password or access token
