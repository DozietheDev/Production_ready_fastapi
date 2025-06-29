```markdown
# Production-Ready FastAPI Service

## Overview
This project makes a simple FastAPI service production-ready using Docker, Kubernetes, CI/CD, monitoring, and security best practices.

## Features
- Multi-stage Docker build
- Kubernetes manifests with probes and resource limits
- CI/CD with GitHub Actions
- Prometheus/Grafana monitoring
- Network policies and RBAC
- Terraform for infrastructure

## Usage
### Build & Run Locally
```bash
docker build -t fastapi .
docker run -p 8000:8000 fastapi
```

### Deploy to Kubernetes
```bash
scripts/deploy.sh
```

### Health Check
```bash
scripts/health-check.sh
```

### Rollback
```bash
scripts/rollback.sh
```

### View App
Visit http://localhost:8000/health or configured ingress hostname.
```