# AWS Infrastructure Terraform Repository

This repository contains the Terraform modules and configurations for deploying and managing the infrastructure of an app.LegisTrader hosted on Amazon Web Services (AWS). The purpose of this repository is to centralize and version control the infrastructure as code, making it easier to maintain, collaborate, and deploy the necessary resources.

## Repository Structure

The repository is structured as follows:
├── modules/
│   ├── vpc/
│   ├── eks/
│   ├── iam/
│   ├── secrets-manager/
│   ├── rds/
│   └── ...
├── environments/
│   ├── production/
│   └── dev/
└── README.md

- `modules/`: This directory contains reusable Terraform modules for different AWS services and resources. Each module is self-contained and can be used independently or composed together to create complete infrastructures.
  - `vpc/`: Module for creating and configuring a Virtual Private Cloud (VPC).
  - `eks/`: Module for provisioning an Amazon Elastic Kubernetes Service (EKS) cluster.
  - `iam/`: Module for managing AWS Identity and Access Management (IAM) resources, such as roles and policies.
  - `secrets-manager/`: Module for setting up and managing secrets using AWS Secrets Manager.
  - `rds/`: Module for provisioning and configuring Amazon Relational Database Service (RDS) instances.
  - ...

- `environments/`: This directory contains Terraform configurations for different environments (e.g., production, development). Each environment directory includes the necessary Terraform files and variable definitions specific to that environment.
