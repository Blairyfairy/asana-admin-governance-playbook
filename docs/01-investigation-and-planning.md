# Step 1: Investigation and Planning

## Path selected

**Path A: Professional experience path**, based on my admin role.

## Organizational context

I run a small consulting practice with a rotating mix of internal members and external client guests. Teams map to client engagements: e-commerce builds, AWS/cloud migrations, hosting and infrastructure (Plesk/SolusVM), and database administration. Work is tracked in per-engagement projects with recurring maintenance tasks.

The main admin risks are:

- paying for licenses that are no longer needed,
- guests keeping access after an engagement ends, and
- third-party tools touching client data.

## Topic 1: License usage and cost control

**Problem.** Client engagements start and end, but licenses and memberships tend to stay assigned. I am likely paying for full licenses on people who only need to view status, and for inactive accounts.

**Admin features and best practices**

- Pull membership reports from the Admin console.
- Run a **license audit**: check current teams, identify inactive and non-contributing users, and review team projects before deleting a team.
- Move status-only stakeholders to **view only licenses**.
- Respond to license change requests using a defined approval rule.

**Desired outcome.** Every paid license maps to an active contributor, view-only licenses cover stakeholders, and costs stay predictable as billing owner-admin.

## Topic 2: User access, guests, and role control

**Problem.** Client guests and contractors can retain access to projects after an engagement ends. Broad default permissions risk exposing one client's work to another's.

**Admin features and best practices**

- Configure **guest invite settings** and **trusted guest domains**.
- Define **project privacy defaults** and **team privacy settings**.
- Use **role-based access controls (RAC)** and create custom roles where defaults do not fit.
- Enable **work access mode (WAM)** for sensitive client work.
- Follow the **deprovisioning steps**: remove the member, then reassign their tasks through a private-to-members project.
- Review guest accounts on a schedule.

**Desired outcome.** Least-privilege access, no orphaned guest accounts, and clear separation between client workspaces.

## Topic 3: Integrations, AI settings, and data security

**Problem.** My workflows connect Asana to code repositories, cloud tooling, and communication apps. Unreviewed integrations, personal access tokens, and AI features could expose client data. I also lack a written process for responding to a security incident.

**Admin features and best practices**

- Review current integrations and set **app approval requirements**.
- Maintain **blocked/allowed app lists**.
- Configure **service accounts** for automations instead of personal accounts.
- Set **Personal Access Token security policies**.
- Review **Asana AI settings and providers** and decide on web access.
- Run a **security checkup**: access review, authentication and login security, configuration review, data protection, update and patching, documentation and awareness.
- Maintain a **breach response plan** (see `06-security-incident-response.md`): containment, investigation, remediation and hardening, communication.

**Desired outcome.** Only vetted apps touch client data, automations run on service accounts, AI use is deliberate, and a documented response plan exists.

## Proactive measure

Run a **quarterly governance and security review** as a recurring Asana task. It covers:

- the license audit,
- the guest and access review,
- the integration and token review,
- a check of the Insights tab for anomalies (teams created, invites sent, projects shared), and
- a pass over data retention and policy documentation.

Each review ends with updating the governance checklist, so settings do not drift between audits. The template is in `templates/quarterly-governance-review.md`.
