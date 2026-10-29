# healthcare-azure-capstone
# Real-World Healthcare Management System on Azure

This repository contains the containerized microservices and Kubernetes manifests for a highly secure, HIPAA-compliant Healthcare Management System deployed on Microsoft Azure.

## Architecture Highlights
* **Compute:** Azure Kubernetes Service (AKS) & Azure Container Registry (ACR).
* **Networking:** Azure Virtual Network, Application Gateway with Web Application Firewall (WAF).
* **Data:** Azure SQL Database (Geo-replicated, TDE enabled) & Azure Redis Cache.
* **Security:** Azure Active Directory (OAuth 2.0/MFA) & Azure Key Vault.

## Deployment Instructions
1. Authenticate to your Azure CLI: `az login`
2. Get AKS credentials: `az aks get-credentials --resource-group <RG-Name> --name <AKS-Cluster-Name>`
3. Apply the manifests: `kubectl apply -f k8s-manifests/`
