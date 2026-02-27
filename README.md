## 🔁 DevOps Workflow Overview

### 1️⃣ Repository Setup
- Created a new GitHub repository.
- Pushed complete MEAN stack source code.
- Maintained separate `backend` and `frontend` directories.

---

### 2️⃣ Containerization
- Created Dockerfiles for:
  - Backend (Node.js + Express)
  - Frontend (Angular build served via Nginx)
- Used official MongoDB Docker image.
- Defined all services in `docker-compose.yml`.

Run locally:
```bash
docker compose up -d
3️⃣ Cloud Deployment (AWS EC2)

Launched Ubuntu EC2 instance.

Installed Docker & Docker Compose.

Opened ports 22 and 80.

Deployed application using Docker Compose.

Application accessible via:

http://<EC2-Public-IP>
4️⃣ CI/CD Pipeline (GitHub Actions)

Trigger: Push to main branch

Pipeline steps:

Checkout code

Login to Docker Hub

Build backend & frontend images

Push images to Docker Hub

SSH into EC2

Pull latest images

Restart containers

Result:
Any code push automatically updates the live application.

5️⃣ Nginx Reverse Proxy

Configured Nginx container.

All traffic routed through port 80.

Backend not exposed publicly.

✅ Assignment Coverage

✔ Dockerized frontend & backend
✔ MongoDB containerized
✔ EC2 deployment via Docker Compose
✔ CI/CD automation
✔ Automatic image build & deployment
✔ Nginx reverse proxy on port 80
