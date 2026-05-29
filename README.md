# Secure-Cloud-Landing-Zones

[![CI](https://github.com/Popoo2020/Secure-Cloud-Landing-Zones/actions/workflows/ci.yml/badge.svg)](https://github.com/Popoo2020/Secure-Cloud-Landing-Zones/actions/workflows/ci.yml)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

**Secure-Cloud-Landing-Zones** provides guidance and reference artefacts for designing secure landing-zone foundations across public cloud providers.

The project focuses on high-level security architecture and governance patterns for identity, networking, logging and control objectives. It is currently a documentation-focused portfolio baseline rather than a deployable Terraform or cloud-template package.

> **Status:** documentation-focused cloud-security reference baseline.

## Features

- **Identity baseline for Azure:** `docs/azure_identity_baseline.md` describes recommended Entra ID patterns including privilege separation, privileged identity management concepts and conditional access policy ideas.
- **Control objectives:** `docs/control_objectives.md` maps landing-zone components such as identity, network, logging and key management to generic security-control objectives.
- **Governance-first design:** the repository emphasises reviewable architecture principles over unverified deployment automation.

## Current repository scope

```text
docs/
  azure_identity_baseline.md
  control_objectives.md

.github/workflows/
  ci.yml
```

## Quickstart

1. Read `docs/azure_identity_baseline.md` to understand foundational identity patterns.
2. Review `docs/control_objectives.md` to connect landing-zone design decisions to security and compliance goals.
3. Adapt the recommendations to your environment before implementation.

## Roadmap

1. Add network segmentation reference notes for Azure and AWS.
2. Add logging baseline guidance for capturing critical security events.
3. Add key-management and break-glass-account guidance.
4. Add diagrams for common landing-zone topologies.
5. Add optional validation checks for documentation consistency.

## Known limitations

- This project is documentation-focused.
- It does not currently provide deployable Terraform modules or scripts.
- The guidance is not a substitute for environment-specific cloud architecture review.
- Recommendations should be adapted to each organisation's risk profile, regulatory requirements and cloud-provider documentation.
