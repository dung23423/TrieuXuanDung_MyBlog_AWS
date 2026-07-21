---
title: "Week 12: S3 Storage & Project Wrap-up"
date: 2026-07-10
weight: 12
chapter: false
---

## Week 12: S3 File Storage Integration and Project Wrap-up

### Daily log

| Day | Work done | Start date | Completion date | Reference |
| ---- | ---- | ---- | ---- | ---- |
| Mon | Discovered AWS Lambda has a read-only filesystem (aside from `/tmp`), so the local file storage from week 8 no longer worked serverless. | 07/06/2026 | 07/06/2026 | [AWS Study Group Docs](https://cloudjourney.awsstudygroup.com/) |
| Tue | Migrated all upload logic to use the AWS SDK for S3, pushing images directly to an S3 bucket. | 07/07/2026 | 07/07/2026 | [AWS Study Group Docs](https://cloudjourney.awsstudygroup.com/) |
| Wed | Configured an IAM policy granting Lambda write access to the specific bucket, defined via Terraform. | 07/08/2026 | 07/08/2026 | [AWS Study Group Docs](https://cloudjourney.awsstudygroup.com/) |
| Thu | Re-tested the full core business flow end-to-end on the deployed environment. | 07/09/2026 | 07/09/2026 | [AWS Study Group Docs](https://cloudjourney.awsstudygroup.com/) |
| Fri | Helped the team finish deploying the demo UI to Vercel hosting, confirmed the UI correctly calls the Backend API on Lambda. | 07/10/2026 | 07/10/2026 | [AWS Study Group Docs](https://cloudjourney.awsstudygroup.com/) |
| Sat | Rewrote the Swagger/README documentation covering every endpoint built over the 12 weeks. | 07/11/2026 | 07/12/2026 | [AWS Study Group Docs](https://cloudjourney.awsstudygroup.com/) |

### Outcomes
*   Image upload works reliably in the serverless + S3 setup.
*   The entire core SmartDorm business flow runs smoothly on the real deployed environment.
*   A complete set of API documentation is ready, making it easy to hand off or extend the project later.

### Looking back on 12 weeks
After 12 weeks, I feel much more confident designing and building a complete Backend with ASP.NET Core, managing AWS infrastructure with Terraform, and running an application in a serverless setup. My involvement on the frontend side was limited to basic support, but it also gave me a clearer understanding of how Backend and Frontend need to coordinate on data formats and authentication.
