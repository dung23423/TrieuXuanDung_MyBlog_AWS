---
title: "Week 5: Room & Rental Request APIs"
date: 2026-07-10
weight: 5
chapter: false
---

## Week 5: Building Room Management and Rental Request APIs

### Daily log

| Day | Work done | Start date | Completion date | Reference |
| ---- | ---- | ---- | ---- | ---- |
| Mon | Built the `/api/rooms` API group: add, edit, delete, and search rooms by status and price range. | 05/18/2026 | 05/18/2026 | [AWS Study Group Docs](https://cloudjourney.awsstudygroup.com/) |
| Tue | Built the `/api/requests` API for students to submit rental requests, including personal details and desired room. | 05/19/2026 | 05/19/2026 | [AWS Study Group Docs](https://cloudjourney.awsstudygroup.com/) |
| Wed | Wrote dedicated validator classes (FluentValidation) instead of manual validation inside controllers, for cleaner code. | 05/20/2026 | 05/20/2026 | [AWS Study Group Docs](https://cloudjourney.awsstudygroup.com/) |
| Thu | Applied DTOs to separate the API response shape from the database entities, avoiding exposing unnecessary sensitive fields. | 05/21/2026 | 05/21/2026 | [AWS Study Group Docs](https://cloudjourney.awsstudygroup.com/) |
| Fri | Learned to write custom validation rules with FluentValidation, e.g. validating Vietnamese phone number formats using regex. | 05/22/2026 | 05/22/2026 | [AWS Study Group Docs](https://cloudjourney.awsstudygroup.com/) |
| Sat | Manually tested the full API via Swagger across 15+ scenarios (valid and invalid data). | 05/23/2026 | 05/24/2026 | [AWS Study Group Docs](https://cloudjourney.awsstudygroup.com/) |

### Outcomes
*   The room management and request-intake APIs work reliably.
*   Learned how to write custom validation rules with FluentValidation.
