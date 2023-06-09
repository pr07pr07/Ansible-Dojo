# AKS-managed Azure Active Directory integration 
## AKS Provides 3 authentication and authorization options:
### 1. Local accounts with Kubernetes RBAC - 
       Use built-in kubernetes role-based access contaol for authorization checks on the cluster
       
       By default, an AKS cluster is created with local accounts using Kubernetes RBAC, with no integration between AKS and Azure AD 
### 2. Azure AD authentication with Kubernetes RBAC - 
       Use Azure AD for authentication and Kubernetes native RBAC for authorization.
### 3. Azure AD authentication with Azure RBAC - 
       Use Azure role assignments for authorization checks on the cluster.
