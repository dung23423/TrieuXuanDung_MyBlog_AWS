---
title: "Week 10: Terraform & RDS PostgreSQL"
date: 2026-07-10
weight: 10
chapter: false
---

## Week 10: Infrastructure as Code with Terraform and RDS

### Daily log

| Day | Work done | Start date | Completion date | Reference |
| ---- | ---- | ---- | ---- | ---- |
| Mon | Learned and practiced core Terraform concepts: `provider`, `resource`, `variable`, `output`, and the state file. | 06/22/2026 | 06/22/2026 | [AWS Study Group Docs](https://cloudjourney.awsstudygroup.com/) |
| Tue | Wrote Terraform code defining a dedicated VPC, subnets, Internet Gateway, Route Table, and Security Group for the deployment environment. | 06/23/2026 | 06/23/2026 | [AWS Study Group Docs](https://cloudjourney.awsstudygroup.com/) |
| Wed | Provisioned Amazon RDS PostgreSQL via Terraform, choosing a `db.t4g.micro` instance to take advantage of the Free Tier. | 06/24/2026 | 06/24/2026 | [AWS Study Group Docs](https://cloudjourney.awsstudygroup.com/) |
| Thu | Hit a missing IAM permissions error running `terraform apply`, temporarily added `AmazonRDSFullAccess` and `AmazonVPCFullAccess` policies. | 06/25/2026 | 06/25/2026 | [AWS Study Group Docs](https://cloudjourney.awsstudygroup.com/) |
| Fri | Added a Security Group rule allowing my own IP to connect to RDS after discovering the local Backend couldn't connect. | 06/26/2026 | 06/26/2026 | [AWS Study Group Docs](https://cloudjourney.awsstudygroup.com/) |
| Sat | Reorganized the Terraform code into modules (`network`, `database`) for easier reuse with other resources in later weeks. | 06/27/2026 | 06/28/2026 | [AWS Study Group Docs](https://cloudjourney.awsstudygroup.com/) |

### Outcomes
*   RDS PostgreSQL runs reliably on AWS, and the local Backend connects successfully.
*   The entire infrastructure can be recreated with a single `terraform apply` and cleanly torn down with `terraform destroy`.
