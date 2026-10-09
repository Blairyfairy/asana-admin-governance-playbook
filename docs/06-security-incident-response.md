# Security Incident Response Runbook

Based on the Asana admin best practices "Respond to a security breach" checklist: containment, investigation, remediation and hardening, communication.

## 1. Containment

- [ ] Identify affected accounts, projects, and integrations.
- [ ] Remove or deactivate compromised members (Admin console > Members > three-dot menu > Remove).
- [ ] Block suspicious apps and revoke affected Personal Access Tokens.
- [ ] Switch sensitive projects to private-to-members and confirm work access mode.

## 2. Investigation

- [ ] Review recent member, guest, and app activity.
- [ ] Determine what data was exposed, to whom, and for how long.
- [ ] Record a timeline of events while details are fresh.

## 3. Remediation and hardening

- [ ] Reset credentials and enforce SSO or two-factor authentication.
- [ ] Tighten guest invite settings, trusted domains, and app approvals.
- [ ] Review RAC roles for excess privilege.
- [ ] Move automations to service accounts.

## 4. Communication

- [ ] Notify the security contact and affected clients promptly.
- [ ] State what happened, what data was involved, and what has been fixed.
- [ ] Follow any contractual or legal notification requirements.
- [ ] Hold a short post-incident review and update this runbook.

## Roles

| Role | Person |
|---|---|
| Incident lead and super admin | Blair Page |
| Backup admin | (assign) |
| Client contact | (per engagement) |
