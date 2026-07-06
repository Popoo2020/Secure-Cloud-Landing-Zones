# Azure Identity Baseline

## Purpose

This document outlines a conservative identity baseline for secure Azure landing-zone design. It is intended as architecture guidance for portfolio review and early governance planning, not as a deployable policy package.

## Baseline principles

- Use Microsoft Entra ID as the central identity plane.
- Separate human administrator accounts from daily-use accounts.
- Require multifactor authentication for privileged access.
- Prefer role-based access control with least privilege.
- Use privileged identity management concepts for standing administrative access.
- Maintain emergency access accounts with strict monitoring and review.
- Review external guest access and service principals regularly.

## Recommended control areas

| Area | Baseline expectation |
|---|---|
| Privileged access | Use dedicated admin accounts and time-bound elevation where possible. |
| Conditional access | Apply strong authentication and location/device-aware access rules. |
| Break-glass access | Maintain emergency accounts with strong controls and alerting. |
| Service principals | Assign least privilege and rotate credentials or prefer managed identities. |
| Guest users | Review access periodically and remove stale accounts. |
| Logging | Capture sign-in, audit and privileged-role events for monitoring. |

## Validation questions

1. Are administrator roles assigned only to dedicated accounts?
2. Is MFA required for all privileged access?
3. Are emergency access accounts documented, protected and monitored?
4. Are service principals reviewed for excessive privileges?
5. Are identity logs forwarded to a monitoring or SIEM workflow?

## Known limitations

This baseline is intentionally generic. Real environments should align implementation with Microsoft guidance, organisational policy, legal requirements and risk appetite.
