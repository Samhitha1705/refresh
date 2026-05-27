# DevOps CI/CD Practice Project

## Tech Used
- Git
- GitHub
- Docker
- Jenkins
- Python Flask
- Ubuntu (WSL)

---

## Project Setup

### Create Virtual Environment
python3 -m venv venv

### Activate venv
source venv/bin/activate

### Install Flask
pip install flask

---

## Docker Commands

### Build Image
docker build -t devops-app .

### Run Container
docker run -d -p 5000:5000 --name devops-container devops-app

### Check Containers
docker ps -a

### View Logs
docker logs devops-container

---

## Git Commands

### Create Branch
git checkout -b stage1

### Push Code
git push -u origin stage1

---

## Jenkins Pipeline

Stages:
1. Clone Repo
2. Build Docker Image
3. Stop Old Container
4. Run New Container

---

## Errors Faced

### Error
_name_ not defined

### Fix
Changed:
Flask(_name_)

to:
Flask(__name__)

---

## What I Learned
- Docker image creation
- Container management
- Jenkins pipelines
- GitHub integration
- CI/CD basics
