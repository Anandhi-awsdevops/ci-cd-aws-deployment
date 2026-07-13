# ci-cd-aws-deployment
# CI/CD Pipeline for Web App Deployment on AWS

## About This Project
Built a complete CI/CD Pipeline using GitHub Actions
that automatically deploys code to AWS EC2
on every push to main branch.

## Tools Used
- GitHub Actions (CI/CD)
- AWS EC2 (Ubuntu 22.04)
- Apache Web Server
- SSH Deployment
- YAML Configuration
- GitHub Secrets

## Architecture
Developer → GitHub Push → GitHub Actions → SSH → EC2 → Apache → Website

## Pipeline Flow
Code Push
    ↓
GitHub Actions Triggered
    ↓
Checkout Code
    ↓
SSH to EC2
    ↓
Deploy Files
    ↓
Website Updated!

## Steps Followed

### Step 1 - EC2 Setup
- Launched Ubuntu EC2 instance
- Installed Apache web server
- Configured permissions

### Step 2 - GitHub Repository Setup
- Created repository
- Added index.html
- Configured GitHub Secrets
  - EC2_HOST (Public IP)
  - EC2_USER (ubuntu)
  - EC2_KEY (PEM file content)

### Step 3 - GitHub Actions Workflow
- Created .github/workflows/deploy.yml
- Configured SSH deployment
- Tested pipeline

### Step 4 - Testing CI/CD
- Pushed code change
- Pipeline triggered automatically
- Website updated without manual work!

## What I Learned
- How to build CI/CD pipelines
- GitHub Actions workflow writing
- Automated deployment to AWS EC2
- Managing GitHub Secrets securely
- Real DevOps workflow experience



## Author
Anandhi Kandhan
AWS and DevOps Fresher
GitHub: github.com/yourusername
LinkedIn: linkedin.com/in/yourusername
