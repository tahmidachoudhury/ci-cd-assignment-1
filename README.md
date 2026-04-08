# Task 1 – Basic CI Pipeline

## What Was Built
A GitHub Actions CI pipeline that runs automatically on every push. The pipeline validates the code, builds a Docker image and pushes it to Docker Hub - all without any manual steps.

## Pipeline Steps
1. Checkout code from the repo
2. Login to Docker Hub using GitHub Secrets
3. Install and run flake8 linting to check code quality
4. Run unit tests to verify the app works
5. Build the Docker image
6. Push the image to Docker Hub
7. Notify on success