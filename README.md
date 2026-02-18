# Secure-Cloud-Landing-Zones

## Overview
This repository provides secure landing zones for Azure and AWS environments. It includes opinionated baselines for identity management, network segmentation, logging, monitoring, and compliance controls. The goal is to help organisations deploy scalable, secure-by-default cloud foundations aligned to ISO 27001 and other frameworks.

## Features
- **Identity baselines**: sample configurations for Azure Entra ID and AWS IAM, including role-based access control, conditional access policies, MFA enforcement and privileged identity management.
- **Network segmentation**: reference network topologies with hub/spoke patterns, network security groups (NSGs), route tables, and VPC/VNet peering guidelines.
- **Logging & monitoring**: templates for enabling platform logging (Azure Activity Log, AWS CloudTrail), threat detection services (Microsoft Sentinel, AWS GuardDuty), and centralised log analytics.
- **Compliance controls**: mapping of landing zone components to ISO/IEC 27001 controls, with evidence suggestions and audit checklists.
- **Documentation & diagrams**: architecture diagrams and design decision records to accelerate implementation.

## Repository Structure
- `azure/` – baseline configurations and scripts for Azure landing zones.
- `aws/` – baseline configurations and scripts for AWS landing zones.
- `docs/` – high-level architecture diagrams, threat models and design documents.
- `.github/workflows/` – CI workflows for linting and validating templates.

## Getting Started
1. Review the architecture and design decisions in `docs/`.
2. For Azure: customise the parameters in `azure/` before deploying via ARM/Bicep/Terraform.
3. For AWS: review the IAM and VPC templates in `aws/` and adjust to your organisation’s naming standards.
4. Use the compliance matrix in `docs/compliance-mapping.md` to map each component to the relevant control.

## Contributing
Contributions are welcome! Please open issues or pull requests for improvements. See `SECURITY.md` for vulnerability reporting procedures and `LICENSE` for terms.

## License
Licensed under the Apache 2.0 License.


