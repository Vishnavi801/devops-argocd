# ArgoCD GitOps Deployment Project

## Project Overview

This project demonstrates how to deploy and manage applications in a Kubernetes cluster using ArgoCD and GitOps principles.

The goal of this project is to automate application deployment by connecting a GitHub repository with ArgoCD. Any changes made to the Kubernetes manifest files in GitHub can be automatically synchronized and deployed to the Kubernetes cluster through ArgoCD.

## Tools Used

* GitHub
* Kubernetes
* ArgoCD
* Docker
* Git

## Project Architecture

Developer
→ GitHub Repository
→ ArgoCD
→ Kubernetes Cluster
→ Application Deployment

## Kubernetes Resources Used

* Deployment
* Service

## Deployment Process

1. Created Kubernetes Deployment and Service manifest files.
2. Stored the manifest files in a GitHub repository.
3. Connected the GitHub repository to ArgoCD.
4. Created an ArgoCD application to monitor the repository.
5. Synced the application from ArgoCD to the Kubernetes cluster.
6. Verified successful deployment and application status.

## Commands Used

```bash
kubectl apply -f deployment.yml
kubectl apply -f svc.yml

kubectl get pods
kubectl get svc

argocd app create
argocd app sync
argocd app get
```

## Key Learnings

* Understanding GitOps concepts.
* Managing Kubernetes deployments through Git repositories.
* Using ArgoCD for continuous deployment.
* Automating application synchronization between GitHub and Kubernetes.
* Monitoring deployment status using the ArgoCD dashboard.

## Benefits of Using ArgoCD

* Automated deployments
* Version-controlled infrastructure
* Easy rollback capability
* Reduced manual intervention
* Improved deployment consistency

## Conclusion

This project helped me gain hands-on experience with GitOps practices using ArgoCD and Kubernetes. It provided a practical understanding of how modern DevOps teams manage and automate application deployments using Git as the single source of truth.
