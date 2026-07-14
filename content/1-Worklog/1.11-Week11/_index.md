---
title: "Week 11: Serverless Deployment with Lambda"
date: 2026-07-10
weight: 11
chapter: false
---

## Week 11: Serverless Deployment with AWS Lambda

### Daily log

| Day | Work done | Start date | Completion date | Reference |
| ---- | ---- | ---- | ---- | ---- |
| Mon | Learned the `Amazon.Lambda.AspNetCoreServer` package to run the ASP.NET Core app on AWS Lambda. | 06/29/2026 | 06/29/2026 | [AWS Study Group Docs](https://cloudjourney.awsstudygroup.com/) |
| Tue | Packaged the Backend into a zip file matching AWS Lambda's required structure, uploaded it to S3. | 06/30/2026 | 06/30/2026 | [AWS Study Group Docs](https://cloudjourney.awsstudygroup.com/) |
| Wed | Created the Lambda function from the zip, connected it to API Gateway (HTTP API v2). | 07/01/2026 | 07/01/2026 | [AWS Study Group Docs](https://cloudjourney.awsstudygroup.com/) |
| Thu | Hit a CORS error calling the API from the demo UI, configured `AddCors` in `Program.cs` to address it. | 07/02/2026 | 07/02/2026 | [AWS Study Group Docs](https://cloudjourney.awsstudygroup.com/) |
| Fri | Set a matching CORS policy on API Gateway to fully resolve the cross-origin issue. | 07/03/2026 | 07/03/2026 | [AWS Study Group Docs](https://cloudjourney.awsstudygroup.com/) |
| Sat | Updated the Terraform code from week 10 to automate creating the Lambda function and API Gateway. | 07/04/2026 | 07/05/2026 | [AWS Study Group Docs](https://cloudjourney.awsstudygroup.com/) |

### Outcomes
*   The Backend runs reliably in a serverless environment, no longer requiring EC2 running 24/7.
*   The CORS issue is fully resolved.
