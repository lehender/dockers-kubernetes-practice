# dockers-kubernetes-practice
Hands-on Docker and Kubernetes lab environment. Includes container deployment, scaling, service exposure, and rolling updates using Docker Desktop and kubectl.
This repository documents my personal lab work for gaining practical experience with containerization and orchestration tools.

### 🔧 Environment
- Docker Desktop (Windows, WSL2 backend)
- Built-in Kubernetes (single-node cluster)
- kubectl CLI for management and troubleshooting

### 🧠 Concepts Covered
- Running and managing Docker containers (`docker run`, `docker ps`, `docker logs`)
- Deploying applications to Kubernetes using `kubectl create deployment`
- Exposing services and scaling pods
- Performing rolling updates and rollbacks
- Observing cluster state and resource health

### 🗂️ Example Commands
```bash
kubectl create deployment nginx-deployment --image=nginx
kubectl expose deployment nginx-deployment --port=80 --type=NodePort
kubectl scale deployment nginx-deployment --replicas=3
kubectl rollout status deployment nginx-deployment
