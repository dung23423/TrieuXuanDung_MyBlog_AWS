---
title: "Week 3: SmartDorm Kickoff & Data Modeling"
date: 2026-07-10
weight: 3
chapter: false
---

## Week 3: SmartDorm Project Kickoff and Data Modeling

### Daily log

| Day | Work done | Start date | Completion date | Reference |
| ---- | ---- | ---- | ---- | ---- |
| Mon | Proposed my personal project, **SmartDorm** — a system to help dormitory management staff track rooms, tenant records, rental contracts, and monthly utility costs. | 05/04/2026 | 05/04/2026 | [AWS Study Group Docs](https://cloudjourney.awsstudygroup.com/) |
| Tue | Discussed scope with my mentor to fit a 12-week timeline, prioritizing a solid Backend first, with the UI kept to a minimal demo. | 05/05/2026 | 05/05/2026 | [AWS Study Group Docs](https://cloudjourney.awsstudygroup.com/) |
| Wed | Drew an Entity-Relationship Diagram (ERD) in draw.io, identifying 6 core entities: `Room`, `Tenant`, `Contract`, `Invoice`, `UtilityUsage`, `Maintenance`. | 05/06/2026 | 05/07/2026 | [AWS Study Group Docs](https://cloudjourney.awsstudygroup.com/) |
| Thu | Designed each table in detail: `Room` (code, capacity, price, status), `Tenant` (personal info, national ID), `Contract` (Room-Tenant link, start/end dates). | 05/07/2026 | 05/08/2026 | [AWS Study Group Docs](https://cloudjourney.awsstudygroup.com/) |
| Fri | Split `Invoice` and `UtilityUsage` into separate tables for easier extension; reserved the `Maintenance` entity in the ERD for later detailed implementation. | 05/08/2026 | 05/08/2026 | [AWS Study Group Docs](https://cloudjourney.awsstudygroup.com/) |
| Sat | Created the GitHub repository, agreed on branch naming conventions (`feature/`, `fix/`) and folder structure, and set up the local dev environment (VS Code, .NET SDK, Docker). | 05/09/2026 | 05/10/2026 | [AWS Study Group Docs](https://cloudjourney.awsstudygroup.com/) |

### Outcomes
*   Completed the ERD, reviewed by my mentor with feedback on adjusting the foreign key relationship between `Contract` and `Invoice`.
*   Project repository is ready, local dev environment is set up to start coding from week 4.
