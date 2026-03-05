# Azure Identity Baseline

This document outlines baseline identity and access management (IAM) configurations for Microsoft Entra ID (Azure AD) in an enterprise landing zone.

## Principles

1. **Least Privilege:** Assign the minimum permissions necessary for users and applications to perform their duties.
2. **Separation of Duties:** Separate administrative roles (e.g., Global Administrator, Security Administrator) to reduce risk of misuse.
3. **Just‑In‑Time Access (JIT):** Use Privileged Identity Management (PIM) to require approval and time‑bound elevation for privileged roles.

## Conditional Access Patterns

| Scenario | Policy Description |
|---------|-------------------|
| Require MFA for all users | Enforce multifactor authentication for interactive sign‑ins. Exclude break‑glass accounts. |
| Block legacy authentication | Create a policy that blocks protocols such as POP/IMAP and Basic Auth to mitigate password spray attacks. |
| Location‑based access | Restrict access to critical applications from trusted countries or IP ranges; require MFA when outside the trusted network. |
| Device compliance | Require devices to be marked as compliant in Intune or hybrid‑joined before accessing sensitive resources. |

## Privileged Access Policies

* Enable PIM for all built‑in privileged roles.
* Require approval for role activation with a clear justification.
* Configure notifications for role assignments and activations.

These baselines serve as a starting point and should be tailored to your organization’s risk profile and regulatory requirements.