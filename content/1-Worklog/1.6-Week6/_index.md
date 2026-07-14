---
title: "Week 6: Approval Automation & Contract Generation"
date: 2026-07-10
weight: 6
chapter: false
---

## Week 6: Automating the Approval Workflow and Contract Generation

### Daily log

| Day | Work done | Start date | Completion date | Reference |
| ---- | ---- | ---- | ---- | ---- |
| Mon | Built the API allowing Admins to approve (`APPROVED`) or reject (`REJECTED`) a rental request. | 05/25/2026 | 05/25/2026 | [AWS Study Group Docs](https://cloudjourney.awsstudygroup.com/) |
| Tue | Implemented the logic: when a request is approved, the system automatically creates a new `Contract` record and updates the room status to `OCCUPIED`. | 05/26/2026 | 05/26/2026 | [AWS Study Group Docs](https://cloudjourney.awsstudygroup.com/) |
| Wed | Wrapped the whole operation in a database transaction to prevent a room from being double-approved for two different students. | 05/27/2026 | 05/27/2026 | [AWS Study Group Docs](https://cloudjourney.awsstudygroup.com/) |
| Thu | Added a simple race-condition check: re-checking the room's status within the same transaction right before approving. | 05/28/2026 | 05/28/2026 | [AWS Study Group Docs](https://cloudjourney.awsstudygroup.com/) |
| Fri | Built the `PUT /api/requests/{id}/reject` API, updating the status and storing the rejection reason entered by the Admin. | 05/29/2026 | 05/29/2026 | [AWS Study Group Docs](https://cloudjourney.awsstudygroup.com/) |
| Sat | Wrote a few integration tests simulating two simultaneous approval requests for the same room to verify the transaction logic. | 05/30/2026 | 05/31/2026 | [AWS Study Group Docs](https://cloudjourney.awsstudygroup.com/) |

### Outcomes
*   The approve → generate contract → update room status flow works correctly across all tested scenarios.
*   No more data inconsistency between `TenantRequests`, `Contracts`, and `Rooms`.
