# Azure Portal Deployment Steps

1. Created Resource Group in Norway East
2. Deployed Virtual Network and subnets
3. Configured Network Security Groups
4. Created Azure App Service
5. Enabled Managed Identity
6. Created Azure Key Vault
7. Configured access policies for secrets
   
## ⚠️ RBAC Propagation Challenge & Design Decision

During deployment, the system-assigned managed identity for the App Service was successfully created (validated via Azure CLI), but did not immediately appear in the Azure Portal role assignment picker.

This behavior is a known Azure RBAC propagation delay, especially common in student subscriptions.

### Solution
Instead of relying on manual access assignment, Azure Policy was used to enforce security and governance rules at the platform level.

### Outcome
- Eliminated dependency on UI-based RBAC propagation
- Improved security consistency
- Demonstrated enterprise-grade governance approach
