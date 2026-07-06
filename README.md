# Secure-Cloud-Landing-Zones

[![CI](https://github.com/Popoo2020/Secure-Cloud-Landing-Zones/actions/workflows/ci.yml/badge.svg)](https://github.com/Popoo2020/Secure-Cloud-Landing-Zones/actions/workflows/ci.yml)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

**Secure-Cloud-Landing-Zones** provides guidance and reference artefacts for designing secure landing-zone foundations across public cloud providers.

The project focuses on high-level security architecture and governance patterns for identity, networking, logging and control objectives. It is currently a documentation-focused portfolio baseline rather than a deployable Terraform or cloud-template package.

> **Status:** documentation-focused cloud-security reference baseline.

## Features

- **Identity baseline for Azure:** `docs/azure_identity_baseline.md` describes recommended Entra ID patterns including privilege separation, privileged identity management concepts and conditional access policy ideas.
- **Governance-first design:** the repository emphasises reviewable architecture principles over unverified deployment automation.
- **Future control objectives:** broader landing-zone control objectives are listed in the roadmap and should be added as the documentation set expands.

## Current repository scope

```text
docs/
  azure_identity_baseline.md

.github/workflows/
  ci.yml
```

## Quickstart

1. Read `docs/azure_identity_baseline.md` to understand foundational identity patterns.
2. Adapt the recommendations to your environment before implementation.
3. Use the roadmap below to guide future documentation expansion.

## Roadmap

1. Add broader control-objective notes for identity, network, logging and key-management themes.
2. Add network segmentation reference notes for Azure and AWS.
3. Add logging baseline guidance for capturing critical security events.
4. Add key-management and break-glass-account guidance.
5. Add diagrams for common landing-zone topologies.
6. Add optional validation checks for documentation consistency.

## Known limitations

- This project is documentation-focused.
- It does not currently provide deployable Terraform modules or scripts.
- The guidance is not a substitute for environment-specific cloud architecture review.
- Recommendations should be adapted to each organisation's risk profile, regulatory requirements and cloud-provider documentation.
