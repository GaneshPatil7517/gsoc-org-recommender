# gsoc-org-recommender
A MERN stack platform that recommends Google Summer of Code organizations to students based on their skills and interests, with admin management, AI-powered recommendation engine, and full DevOps deployment.


Table of Contents
Project Overview
Tech Stack
Features
Folder Structure
Installation & Setup
DevOps & Deployment
AI Recommendation Engine
Testing & Security
Future Improvements
License

Project Overview
GSoC Guide is designed to help students find the best-fit GSoC organizations by matching their skills and interests with available opportunities. Admins can manage organizations yearly, while students receive personalized recommendations based on their input skills. The project is production-ready, fully containerized, and deployable on cloud platforms with Kubernetes orchestration and CI/CD automation.


Tech Stack

Frontend:
React + Tailwind CSS
React Router DOM
Axios for API requests

Backend:
Node.js + Express
MongoDB (NoSQL database)
JWT Authentication (Students & Admins)

DevOps / Deployment:
Docker & Docker Compose
Kubernetes (Deployments, Services, Ingress, Autoscaling)
CI/CD with Jenkins
Cloud Deployment (GKE / AWS EKS / Azure AKS)
AI / Recommendation:
Initial: Tag-based skill matching
Advanced: Embeddings & semantic similarity for AI-powered recommendations

Testing & Security:
Jest for unit & integration tests
Helmet, input validation, rate limiting for security

Features
For Students:
Register/login & JWT authentication
Enter skills & interests
Receive organization recommendations
Dashboard analytics: search stats, top skills

For Admins:
CRUD operations for GSoC organizations
Yearly updates to organization list
Analytics dashboard for student trends
Prometheus + Grafana for monitoring

🔹 Folder Structure (Example)

gsoc-guide/
├─ backend/
│  ├─ controllers/
│  ├─ models/
│  ├─ routes/
│  ├─ middleware/
│  ├─ utils/
│  ├─ app.js
│  └─ server.js
├─ frontend/
│  ├─ public/
│  ├─ src/
│  │  ├─ components/
│  │  ├─ pages/
│  │  ├─ hooks/
│  │  ├─ services/
│  │  └─ App.js
├─ k8s/
│  ├─ deployment.yaml
│  ├─ service.yaml
│  └─ ingress.yaml
├─ docker/
│  ├─ Dockerfile.backend
│  ├─ Dockerfile.frontend
│  └─ docker-compose.yml
├─ tests/
├─ .gitignore
├─ README.md
└─ package.json
