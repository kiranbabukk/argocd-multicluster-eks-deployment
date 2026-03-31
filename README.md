# Multi-Cluster Application Deployment using ArgoCD (AWS EKS)

## Overview
This project demonstrates a complete GitOps-based multi-cluster deployment using ArgoCD on Amazon EKS. The same application is deployed across multiple Kubernetes clusters using a single Git repository.

## Infrastructure Setup
- Provisioned 3 Amazon EKS clusters using Terraform
- Each cluster contains 2 worker nodes
- Total infrastructure: 3 clusters, 6 nodes

## Tools & Technologies
- AWS EKS
- Terraform (Infrastructure as Code)
- Kubernetes
- ArgoCD (GitOps)
- GitHub

## Deployment Strategy
- Application manifests stored in GitHub repository
- ArgoCD configured for multi-cluster management
- Used ApplicationSet to automatically deploy applications across all clusters
- Continuous synchronization enabled

## Application Details
- Application: Tetris Web Application
- Docker Image: kirankalyandevops/tetrisv2:latest
- Service Type: LoadBalancer

## Deployment Outcome
- Successfully deployed application across:
  - EKS_CLUSTER_NEW1
  - EKS_CLUSTER_NEW2
  - EKS_CLUSTER_NEW3
- All applications are in:
  - Healthy
  - Synced

## Output
(Add ArgoCD UI screenshot here showing all applications in Healthy and Synced state)

## Repository
https://github.com/kiranbabukk/devsecops-Tetris-manifest
