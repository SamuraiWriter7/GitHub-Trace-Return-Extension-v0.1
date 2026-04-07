# Security Policy

## Scope

This repository is a specification and reference design repository for the **GitHub Trace Return Extension v0.1**.

It does not provide a production service, hosted API, or deployed runtime system.
However, it includes:

- machine-readable schemas
- sample configuration files
- GitHub Actions workflow definitions
- governance-oriented specification documents

Because of that, security concerns in this repository mainly involve:

- workflow misuse
- malicious or misleading schema/example changes
- supply-chain style manipulation of validation logic
- confusing or deceptive policy modifications presented as legitimate specification updates

---

## Supported Versions

At this stage, security review is focused on the latest version on the default branch.

| Version | Supported |
|---------|-----------|
| v0.1.x  | Yes       |
| earlier drafts | No |

---

## What to Report

Please report issues such as:

- malicious workflow changes
- unauthorized or suspicious changes to schema validation logic
- deceptive example files designed to bypass validation intent
- misleading documentation changes that alter governance meaning in a harmful way
- security risks introduced through repository automation
- abuse vectors that could enable score manipulation, trace farming, or anti-gaming bypass in future implementations

You may also report broader specification-level concerns if they relate to:

- integrity
- trust
- provenance
- misuse resistance
- governance abuse

---

## What Not to Report

Please do not report:

- general feature requests
- editorial preferences
- conceptual disagreements that are not security-relevant
- speculative production vulnerabilities in systems that are not implemented in this repository
- issues already documented as non-goals in the specification

---

## Reporting a Vulnerability

If you discover a security issue, please report it privately first.

Recommended report contents:

- short summary
- affected file(s)
- description of the issue
- reproduction steps, if applicable
- potential impact
- suggested fix, if available

At this stage, the preferred reporting path is:

- open a private communication channel if available
- otherwise open a GitHub issue only if the report does **not** create additional risk by being public

If the issue could enable abuse, workflow compromise, or deceptive governance manipulation, please avoid public disclosure before review.

---

## Response Goals

Best-effort response goals:

- initial acknowledgment: within 7 days
- triage decision: within 14 days
- fix or documented resolution: as reasonably possible depending on severity and scope

These are goals, not guarantees.

---

## Disclosure Policy

This repository prefers **responsible disclosure**.

Please do not publicly disclose high-risk issues before there has been a reasonable opportunity to review and respond.

When a confirmed issue is resolved, the resolution may be documented through one or more of the following:

- commit history
- release notes
- changelog entry
- repository documentation update

---

## Security Priorities for This Repository

The main security priorities are:

1. **Workflow integrity**  
   Prevent unsafe or misleading changes to GitHub Actions workflows.

2. **Schema integrity**  
   Preserve trust in machine-readable validation files.

3. **Example integrity**  
   Ensure examples reflect intended usage and are not silently replaced with deceptive content.

4. **Governance integrity**  
   Prevent harmful redefinition of core concepts under the appearance of minor edits.

5. **Anti-gaming awareness**  
   Keep future abuse surfaces visible, especially around attribution manipulation and trace-score inflation.

---

## Safe Contribution Guidance

When contributing changes, extra care should be taken with:

- `.github/workflows/**`
- `schema/**`
- `examples/**`
- governance-related documentation

Large or subtle changes in these areas should be reviewed carefully before merge.

---

## Out of Scope

The following are outside the direct security scope of this repository:

- production infrastructure vulnerabilities
- payment processor vulnerabilities
- vulnerabilities in third-party platforms not controlled by this repository
- legal disputes about attribution or ownership by themselves
- hypothetical runtime exploits in systems not implemented here

---

## Contact Note

This repository is currently maintained as a specification-first project.
Security handling is therefore centered on **integrity, trust, and misuse resistance**, not only traditional software exploits.

If you report an issue in good faith, that effort is appreciated.
