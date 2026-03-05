# Control Objectives Mapping

This document maps high-level security control objectives to specific landing zone design elements and configurations.

| Control Objective | Implementation in Landing Zone |
|------------------|-------------------------------|
| **Identity and Access Management** | Implement Azure Entra baseline policies (see `azure_identity_baseline.md`), including MFA, conditional access, PIM and role separation. |
| **Network Segmentation** | Use Virtual Network (VNet) peering and Network Security Groups (NSGs) to separate workloads and enforce least-privilege access between tiers. |
| **Logging and Monitoring** | Enable diagnostic logs for all resources; forward logs to a central Log Analytics workspace; integrate with Sentinel for SIEM capabilities. |
| **Key Management** | Use Azure Key Vault or Managed HSM for key storage; enforce soft-delete and purge protection; rotate keys regularly. |
| **Resiliency and Disaster Recovery** | Deploy workloads across multiple availability zones; implement backup policies and test restoration procedures. |

These mappings align with common frameworks such as ISO 27001 and NIST SP 800‑53. Adjust control objectives based on compliance requirements and business context.