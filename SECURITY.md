# Security Policy

This document defines the security posture, support boundaries, and responsible disclosure process for this project. It is written to establish clear expectations for users, contributors, researchers, and maintainers, and to ensure that security-related communication is handled with rigor, discretion, and accountability.

Security is treated here not as an afterthought or a compliance checkbox, but as a first-order design constraint. The policies below are intended to scale with the project over time and to remain valid even as implementations evolve.

---

## Supported Versions

Security updates are provided **only** for the versions explicitly listed as supported below. Versions not listed as supported should be considered **end-of-life (EOL)** and may contain unpatched vulnerabilities.

| Version | Supported |
| ------- | --------- |
| 5.1.x   | ✅ Yes    |
| 5.0.x   | ❌ No     |
| 4.0.x   | ✅ Yes    |
| < 4.0   | ❌ No     |

### Interpretation of Support Status

- **Supported versions** receive security patches for vulnerabilities that meet the project’s severity threshold.
- **Unsupported versions** do not receive security fixes, regardless of severity.
- Users running unsupported versions are strongly advised to upgrade to a supported release before reporting security issues.

Support status applies **only** to security updates. Functional bugs, performance issues, or feature requests may follow a different lifecycle.

---

## Security Scope

This security policy applies to:
- The core codebase maintained in this repository
- Official build artifacts and release distributions
- Configuration defaults shipped with supported versions
- Documented and intended usage patterns

This policy does **not** apply to:
- Forks or downstream derivatives not maintained by this project
- Custom modifications or patches applied by third parties
- Deployment environments outside the project’s control
- Vulnerabilities introduced through misuse, misconfiguration, or unsupported integrations

Reports that fall outside this scope may be acknowledged but are not guaranteed remediation.

---

## Reporting a Vulnerability

If you believe you have discovered a security vulnerability, **do not open a public issue** and **do not disclose details publicly** before coordination with the maintainers.

Responsible disclosure protects users, maintainers, and downstream projects.

### How to Report

To report a vulnerability:

1. Use GitHub’s **private security advisory** feature for this repository, if available  
   **or**
2. Contact the maintainers via the designated private security contact listed in the repository metadata

Your report should include, as applicable:
- A clear description of the vulnerability
- Affected versions and components
- Steps to reproduce the issue
- Proof-of-concept code or examples (if safe to share)
- Impact assessment (confidentiality, integrity, availability)
- Any known mitigations or workarounds

Incomplete reports may delay triage.

---

## What Happens After You Report

### Acknowledgment

- You can expect an acknowledgment of receipt **within 7 business days**.
- This acknowledgment confirms that the report has been received and queued for review.
- It does not imply validation or acceptance of the report.

### Triage and Assessment

The maintainers will:
- Verify whether the issue is reproducible
- Determine whether it falls within scope
- Assess severity using internal risk criteria
- Identify affected versions and components

During this phase, you may be contacted for clarification or additional information.

---

## Disclosure and Remediation Process

If a vulnerability is **accepted**:

- A fix will be developed for supported versions
- A coordinated disclosure timeline will be established
- A security advisory will be published once remediation is available
- Credit may be given to the reporter unless anonymity is requested

If a vulnerability is **declined**:

- You will be informed of the decision and the rationale
- Common reasons for decline include:
  - Issue is not reproducible
  - Issue falls outside defined scope
  - Issue does not represent a security risk
  - Issue affects only unsupported versions

Declined reports are not an indictment of the reporter’s intent; they reflect scope and risk assessment decisions.

---

## Severity Classification

While exact scoring may vary, vulnerabilities are generally evaluated along these dimensions:

- **Impact**: Degree of harm if exploited
- **Exploitability**: Practical difficulty of exploitation
- **Exposure**: Likelihood of real-world use
- **Blast radius**: Scope of affected systems or data

Not all vulnerabilities warrant immediate public disclosure. Some may be handled silently if risk is negligible and no user action is required.

---

## Expectations for Reporters

We ask security researchers and reporters to:
- Act in good faith
- Avoid exploiting vulnerabilities beyond what is necessary for proof
- Avoid accessing or modifying data that does not belong to you
- Allow reasonable time for remediation before disclosure

Reports that involve extortion, coercion, or public disclosure without coordination may be disregarded.

---

## Communication and Updates

- Status updates are provided **as appropriate**, not on a fixed schedule
- Complex issues may take time to investigate and remediate
- Silence does not imply inaction; it often reflects ongoing work

We value responsible research and aim to maintain respectful, professional communication throughout the process.

---

## Security Is a Shared Responsibility

No system is perfectly secure. Security emerges from:
- Thoughtful design
- Conservative defaults
- Clear documentation
- Responsible disclosure
- Continuous review

By reporting vulnerabilities responsibly and adhering to this policy, you contribute to the resilience and trustworthiness of the project.

This document may evolve over time, but its core principle remains constant:  
**Security decisions are made deliberately, transparently, and with long-term impact in mind.**
