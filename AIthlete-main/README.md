GymAI — Pose Estimation ML Service

This repository contains a lightweight pose-estimation model and an inference FastAPI service.

Quick start (local):

- Run unit tests for the ML module:

```powershell
$env:PYTHONPATH = "C:\Users\rishi\Documents\GymAI\Backend\ml\pose_estimation"
python -m pytest Backend/ml/pose_estimation/tests -q
```

- Run with Docker Compose (includes Redis for session persistence):

```powershell
docker-compose up --build
# service will be available at http://localhost:8000
```

- Build Docker image manually:

```powershell
docker build -t gymai-pose:latest Backend/ml/pose_estimation
docker run -p 8000:8000 --env REDIS_URL=redis://host:6379/0 gymai-pose:latest
```

- Deploy to Render: add `render.yaml` and set build/start commands in the Render dashboard.
- Deploy to Render: add `render.yaml` and set build/start commands in the Render dashboard.

Publish to GitHub Container Registry (GHCR):

1. A GitHub Actions workflow `publish-ghcr.yml` is included that will build and push the Docker image to GHCR when you push to `main` or manually trigger the workflow.
2. The workflow uses the repository's `GITHUB_TOKEN` by default so you don't need to add secrets for pushing to GHCR within the same repository.

Credits: This is a demo scaffold; before production use, improve model accuracy, add monitoring, and secure uploads.
