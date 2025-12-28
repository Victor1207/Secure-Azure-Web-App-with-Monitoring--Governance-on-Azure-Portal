# Secure Enterprise Azure Network (Azure Portal)

## Overview
This project demonstrates a secure, enterprise-style Azure network
designed and deployed manually using the Azure Portal.

The goal is to understand Azure networking, identity, and security
concepts before automating the architecture using Bicep.

## Architecture
- Virtual Network with segmented subnets
- Network Security Groups (NSGs)
- Azure App Service
- Azure Key Vault
- Managed Identity

## Security Design
- Secrets stored in Azure Key Vault
- System-assigned Managed Identity
- No credentials in application code

## Deployment Method
- Azure Portal (Manual)
- Azure CLI used for validation

## Subscription Notes
This project was deployed using an Azure Student subscription.
RBAC limitations required the use of Key Vault access policies.

## Author
**Victor Olasehinde**  

