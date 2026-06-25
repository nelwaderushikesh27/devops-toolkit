# 🐳 DevOps Toolkit

Docker & Kubernetes configurations for development and deployment.

## 📦 What's Included

| Tool | Description |
|------|-------------|
| **Docker Compose** | Multi-service setup |
| **Kubernetes** | K8s deployment configs |
| **CI/CD** | GitHub Actions pipelines |
| **Monitoring** | Prometheus + Grafana |
| **Logging** | ELK Stack |

## 🚀 Quick Start

```bash
git clone https://github.com/nelwaderushikesh27/devops-toolkit.git
cd devops-toolkit

# Start all services
docker-compose up -d

# Deploy to Kubernetes
kubectl apply -f k8s/
```

## 🏗️ Project Structure
```
devops-toolkit/
├── docker/
│   ├── Dockerfile
│   └── docker-compose.yml
├── k8s/
│   ├── deployment.yaml
│   ├── service.yaml
│   └── ingress.yaml
├── monitoring/
│   └── prometheus.yml
├── ci-cd/
│   └── github-actions.yml
├── scripts/
│   ├── deploy.sh
│   └── backup.sh
└── README.md
```

## 🐳 Docker Services

| Service | Port | Description |
|---------|------|-------------|
| API | 3000 | Node.js backend |
| Frontend | 5173 | React app |
| MongoDB | 27017 | Database |
| Redis | 6379 | Cache |
| Nginx | 80 | Reverse proxy |

## ☸️ Kubernetes

```bash
# Apply configurations
kubectl apply -f k8s/namespace.yaml
kubectl apply -f k8s/configmap.yaml
kubectl apply -f k8s/deployment.yaml
kubectl apply -f k8s/service.yaml

# Check status
kubectl get pods -n production
kubectl get services -n production
```

## 🔄 CI/CD Pipeline

The GitHub Actions workflow:
1. Run tests
2. Build Docker image
3. Push to Docker Hub
4. Deploy to Kubernetes

## 📊 Monitoring

- Prometheus for metrics collection
- Grafana for visualization
- ELK Stack for log management

---
*Infrastructure as Code 🚀*
