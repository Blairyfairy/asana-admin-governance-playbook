# Asana Admin Governance Playbook

Capstone project for the **Asana Administrator Certificate** (Path A: Professional Experience), completed by **Blair Page**, freelance Systems/Cloud Engineer (AWS, database administration, e-commerce full-stack).

The repo covers every capstone objective: investigation and planning, an ongoing admin checklist, an Asana project build, and a reflection. It also includes an incident response runbook and a comparison against the official exemplar.

## Repository structure

```
asana-admin-governance-playbook/
├── README.md
├── LICENSE
├── .gitignore
├── docs/
│   ├── 01-investigation-and-planning.md   # Step 1: three topics, plans, proactive measure
│   ├── 02-ongoing-admin-checklist.md      # Step 2: checklist with rationale
│   ├── 03-asana-project-build.md          # Step 3: project structure, tasks, timeline
│   ├── 04-reflection.md                   # Reflection answers (100-150 words)
│   ├── 05-exemplar-comparison.md          # Mapping to the official exemplar
│   └── 06-security-incident-response.md   # Breach response runbook
├── checklists/
│   └── ongoing-admin-best-practices.md    # Printable/pasteable checklist
├── data/
│   └── asana-project-import.csv           # Importable task list with dates and assignees
└── templates/
    ├── quarterly-governance-review.md     # Recurring review template
    └── guest-offboarding.md               # Engagement-close access cleanup
```

## Capstone objectives coverage

| Objective | Where it is addressed |
|---|---|
| Review the path and organizational context | `docs/01-investigation-and-planning.md` |
| Identify three topics to investigate | `docs/01-investigation-and-planning.md` |
| Plan per topic (problem, features, outcome) | `docs/01-investigation-and-planning.md` |
| One proactive measure | `docs/01-investigation-and-planning.md`, `templates/quarterly-governance-review.md` |
| "Ongoing Admin Best Practices" checklist (5-7 items) | `docs/02-ongoing-admin-checklist.md`, `checklists/` |
| Build an Asana project with dates and assignees | `docs/03-asana-project-build.md`, `data/asana-project-import.csv` |
| Reflection (2 questions, 100-150 words) | `docs/04-reflection.md` |

## Quick start: build the Asana project

1. In Asana, create a project (or start from the **Workflow gallery** operations project plan for IT teams, as the exemplar does).
2. Edit `data/asana-project-import.csv` and replace `admin@example.com` with your real Asana email.
3. Use **Add project > Import CSV** and map the columns.
4. Add the Priority and Topic custom fields, then set the quarterly review task to repeat every 3 months.

## Source material

Based on the *Asana Administrator Certificate: Admin best practices checklists* from Asana Academy. This repo is an independent study project and is not affiliated with Asana.

## Author

Blair Page, Las Vegas, NV
