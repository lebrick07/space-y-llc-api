# Space Y LLC Application

Auto-generated application managed by OpenLuffy.

## Stack
- **Language**: Python
- **Framework**: FastAPI
- **Container Registry**: GitHub Container Registry (GHCR)

## Environments
- **Development**: `space-y-llc-dev` namespace
- **Pre-production**: `space-y-llc-preprod` namespace  
- **Production**: `space-y-llc-prod` namespace

## Local Development

### ```bash
pip install -r requirements.txt
python main.py
```

Visit: http://localhost:8000

## CI/CD Pipeline
GitHub Actions automatically builds and deploys on push:
- `develop` branch → DEV + PREPROD environments
- `main` branch → PRODUCTION environment (manual approval required)

## Deployment
Managed by ArgoCD - syncs automatically when new images are pushed.

## Health Check
All environments expose `/healthz` endpoint for liveness/readiness probes.

---
*Managed by OpenLuffy* 🏴‍☠️
