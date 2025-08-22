# Terraform-Jenkins-Repo-for-Flask-App

This repository contains **Terraform configurations** to provision AWS resources required to run the Flask application.

## Contents
- `main.tf` → Infrastructure definition (VPC, subnets, EC2, Security Groups).
- `variables.tf` → Configurable variables (region, instance type, etc.).
- `outputs.tf` → Useful outputs like public IP or DNS.
- `jenkins_pipeline.tf` → Jenkins integration for automation.

## Purpose
- Automates the provisioning of AWS infrastructure.
- Provides networking, compute, and security setup for the Flask application.
- Ensures reproducible and version-controlled infrastructure.

## How It Fits in the Project
1. Jenkins triggers Terraform scripts after a successful build.
2. Terraform provisions infrastructure (EC2, networking, IAM).
3. Flask app container is deployed to the provisioned EC2.

---
