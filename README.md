# AKS-managed Azure Active Directory integration 
## AKS Provides 3 authentication and authorization options:
### 1. Local accounts with Kubernetes RBAC - 
       Use built-in kubernetes role-based access contaol for authorization checks on the cluster.
       By default, an AKS cluster is created with local accounts using Kubernetes RBAC, with no integration between AKS and Azure AD.
          * You can use native Kubernetes options like client certificates or bearer tokens
          * "az aks get-credentials" but everyone will have full access.
### 2. Azure AD authentication with Kubernetes RBAC - 
       Use Azure AD for authentication and Kubernetes native RBAC for authorization.
       Irreversible
       OpenID Connect is used to enable authentication
       Azure  AD Premium offer conditional policies to restrict access future, e.g by location or JIT
       
### 3. Azure AD authentication with Azure RBAC - 
       Use Azure role assignments for authorization checks on the cluster.
       Irreversible
       OpenID Connect is used to enable authentication
       Azure  AD Premium offer conditional policies to restrict access future, e.g by location or JIT
       Integrating AKS cluster with azure AD allows fine-grained control over user access using Azure RBAC and Kubernetes RBAC
