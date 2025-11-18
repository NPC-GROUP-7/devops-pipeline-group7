---
name: DevOps Task
about: Track infrastructure, pipeline, or configuration tasks.
title: "[DEVOPS] "
labels: devops
assignees: ''
---

## Task Description  
Set up the *End-to-End CI/CD pipeline* for the Funny Poll System using GitHub Actions.  
Pipeline should build and test both frontend (React) and backend (Node), run PostgreSQL in Docker, and deploy to production.

## Component  
- [x] CI/CD Pipeline  
- [ ] Infrastructure  
- [ ] Configuration Management  
- [ ] Security  
- [ ] Documentation  

## Acceptance Criteria  
- Pipeline triggers on pull request & push to main  
- Runs separate frontend + backend build and test jobs  
- Launches PostgreSQL using services in GitHub Actions  
- Automatically deploys to staging when PR is merged  
- Production deployment requires manual approval  
- Stores secrets in GitHub Actions → Settings → Secrets

## Dependencies  
- Dockerfile for frontend and backend  
- docker-compose file for full stack  
- Provisioned production server (AWS/DigitalOcean/Render)  
- Environment variables stored securely

## Estimated Effort  
*Large*
