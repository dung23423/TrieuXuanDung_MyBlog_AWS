---
title: "Week 9: JWT Authentication & Integration Testing"
date: 2026-07-10
weight: 9
chapter: false
---

## Week 9: JWT Authentication and System Integration Testing

### Daily log

| Day | Work done | Start date | Completion date | Reference |
| ---- | ---- | ---- | ---- | ---- |
| Mon | Integrated JWT authentication into the Backend: built the `POST /api/auth/login` API, issuing an access token with `UserId` and `Role` claims. | 06/15/2026 | 06/15/2026 | [AWS Study Group Docs](https://cloudjourney.awsstudygroup.com/) |
| Tue | Configured `[Authorize(Roles = "Admin")]` on admin-only APIs (add/edit/delete rooms, approve requests). | 06/16/2026 | 06/16/2026 | [AWS Study Group Docs](https://cloudjourney.awsstudygroup.com/) |
| Wed | Wrote a sample `fetch` snippet for calling the login API to help the teammate owning the UI wire it in. | 06/17/2026 | 06/17/2026 | [AWS Study Group Docs](https://cloudjourney.awsstudygroup.com/) |
| Thu | Explained how to attach the token to the `Authorization: Bearer <token>` header for authenticated requests. | 06/18/2026 | 06/18/2026 | [AWS Study Group Docs](https://cloudjourney.awsstudygroup.com/) |
| Fri | Worked with the team to test the login → protected API call flow end-to-end. | 06/19/2026 | 06/19/2026 | [AWS Study Group Docs](https://cloudjourney.awsstudygroup.com/) |
| Sat | Tested expired/fake tokens to confirm the API correctly returns 401. | 06/20/2026 | 06/21/2026 | [AWS Study Group Docs](https://cloudjourney.awsstudygroup.com/) |

### Outcomes
*   All sensitive APIs are correctly protected by role.
*   Confirmed the login flow works reliably when integrated with the team's UI.
