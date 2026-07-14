---
title: "Week 7: Utility Billing Module"
date: 2026-07-10
weight: 7
chapter: false
---

## Week 7: Building the Utility Billing Calculation Module

### Daily log

| Day | Work done | Start date | Completion date | Reference |
| ---- | ---- | ---- | ---- | ---- |
| Mon | Designed the `UtilityUsage` table to store starting and ending electricity/water meter readings per room, per month. | 06/01/2026 | 06/01/2026 | [AWS Study Group Docs](https://cloudjourney.awsstudygroup.com/) |
| Tue | Wrote the billing service: electricity and water charges based on configured unit rates, plus room rent and service fees for the total invoice. | 06/02/2026 | 06/02/2026 | [AWS Study Group Docs](https://cloudjourney.awsstudygroup.com/) |
| Wed | Built the `POST /api/invoices/generate` batch API, automatically generating invoices for all occupied rooms for the current month. | 06/03/2026 | 06/03/2026 | [AWS Study Group Docs](https://cloudjourney.awsstudygroup.com/) |
| Thu | Found a bug: forgot to handle the case where the ending reading is lower than the starting reading, producing a negative charge; added validation to block this case. | 06/04/2026 | 06/04/2026 | [AWS Study Group Docs](https://cloudjourney.awsstudygroup.com/) |
| Fri | Wrote dedicated unit tests for the calculation logic, covering multiple data sets to make sure the formulas stay correct if rates change. | 06/05/2026 | 06/05/2026 | [AWS Study Group Docs](https://cloudjourney.awsstudygroup.com/) |
| Sat | Ran the invoicing API against a test data set of 10 rooms with varying consumption levels. | 06/06/2026 | 06/07/2026 | [AWS Study Group Docs](https://cloudjourney.awsstudygroup.com/) |

### Outcomes
*   The auto-invoicing API works correctly against the test data set.
*   The calculation unit test suite passes 100%.
