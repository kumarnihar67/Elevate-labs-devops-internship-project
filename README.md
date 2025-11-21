🚀 Local CI/CD Pipeline with GitHub Actions, Docker & Minikube

💻 No cloud required — full CI/CD pipeline running locally.

This project demonstrates a complete CI/CD pipeline that builds a Docker image 🐳, runs automated tests 🧪, pushes the image to Docker Hub, and deploys the application to a local Kubernetes cluster using Minikube ☸️.

📌 Project Overview

The goal of this project is to simulate a full cloud-like CI/CD workflow entirely on your local machine.

🔥 Features included:

🐳 Dockerfile for containerization

📦 docker-compose for local dev

🤖 GitHub Actions workflow for CI/CD

🧪 Automated tests on every push

📤 Push Docker image to Docker Hub

☸️ Kubernetes deployment on Minikube

🌐 Running app inside Minikube

🧱 Architecture & Workflow
┌──────────────┐       ┌──────────────────┐       ┌─────────────────────┐
│  GitHub Repo │──────▶│ GitHub Actions CI│──────▶│ Docker Hub Registry │
└──────────────┘       └──────────────────┘       └───────────┬─────────┘
                                                               │
                                                               ▼
                                                    ┌────────────────────┐
                                                    │ Minikube Kubernetes │
                                                    │ (Local Deployment)  │
                                                    └────────────────────┘
                                                    

🛠 Tech Stack🔧 Component	🛠 Tool

CI/CD	GitHub Actions 🤖
Containerization	Docker 🐳
Container Registry	Docker Hub 📦
Local Deployment	Minikube ☸️
Orchestration	Kubernetes ⚙️
Dev Setup	docker-compose 🧩

🏁 Getting Started

1️⃣ Clone the Repository
🐳 Docker Setup Build & Run Locally

<img width="1920" height="1080" alt="P-1-minikube1" src="https://github.com/user-attachments/assets/9e7ba587-2509-401f-9817-60acce3eefc9" />


🤖 CI/CD with GitHub Actions
 Runs tests

<img width="1920" height="1080" alt="P1-workflow1" src="https://github.com/user-attachments/assets/8538b91b-89a1-4cba-bbc8-0a01c902b0b7" />

 
 Builds the Docker image

<img width="1920" height="1080" alt="P1-workflow2" src="https://github.com/user-attachments/assets/070a9841-d7f0-4c68-b395-20659fc757e7" />

 
 Logs in to Docker Hub

<img width="1920" height="1080" alt="P1-workflow3" src="https://github.com/user-attachments/assets/c955d1aa-b962-4596-840c-bb51a276b8e3" />

 
 Pushes the image 

 <img width="1920" height="1080" alt="P-1-repo" src="https://github.com/user-attachments/assets/7fd6465c-625a-4cf0-abd3-f7e385d1710c" />

 

☸️ Deploying to Minikube Start Minikube
   Apply Kubernetes manifests
   Stored in:deployment.yaml , service.yaml

   <img width="1920" height="1080" alt="P-1-minikube1" src="https://github.com/user-attachments/assets/7f6cef59-5ba8-4759-b3ae-247c56b74326" />


5️⃣ Verify Deployment
   kubectl get pods
   kubectl get svc

   <img width="1920" height="1080" alt="P-1-minikube2" src="https://github.com/user-attachments/assets/bd1f7201-bccf-49af-b50d-aa5271b0aad3" />


6️⃣ Access the App 🌐
   minikube service my-local-app-service

   <img width="1920" height="1080" alt="deployment-screenshot" src="https://github.com/user-attachments/assets/f581ae73-0c55-4909-9531-29f0485f56e3" />


📦 Docker Hub Image
    https://hub.docker.com/u/kumarnihar67

  <img width="1920" height="1080" alt="P1-dockerhub-image" src="https://github.com/user-attachments/assets/47767773-aab0-4bb2-a163-35bc14857691" />


    
