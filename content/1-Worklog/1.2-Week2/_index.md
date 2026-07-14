---
title: "Week 2: VPC & S3 Storage"
date: 2026-07-10
weight: 2
chapter: false
---

## Week 2: Hands-on with Virtual Private Cloud (VPC) and S3 Object Storage

### Goals
* Understand how to design a secure virtual private network on AWS.
* Get familiar with the S3 object storage service and access control via IAM.

### Daily log

| Day | Work done | Start date | Completion date | Reference |
| ---- | ---- | ---- | ---- | ---- |
| Mon | Studied CIDR blocks, public/private subnets, Internet Gateway, NAT Gateway, and Route Tables within a VPC. | 04/27/2026 | 04/27/2026 | [AWS Study Group Docs](https://cloudjourney.awsstudygroup.com/) |
| Tue | Built a VPC by hand with one public and one private subnet, verified that instances in the private subnet cannot reach the Internet directly. | 04/28/2026 | 04/28/2026 | [AWS Study Group Docs](https://cloudjourney.awsstudygroup.com/) |
| Wed | Learned about S3 concepts: Buckets, Objects, Storage Classes, Versioning. Created a test bucket, uploaded/deleted objects via Console and CLI. | 04/29/2026 | 04/29/2026 | [AWS Study Group Docs](https://cloudjourney.awsstudygroup.com/) |
| Thu | Read about IAM JSON policies, wrote a custom policy allowing only read access (GetObject) on a specific bucket. | 04/30/2026 | 04/30/2026 | [AWS Study Group Docs](https://cloudjourney.awsstudygroup.com/) |
| Fri | Attached the policy to a test IAM user and confirmed the restricted permissions worked as expected (no delete/upload allowed). | 05/01/2026 | 05/01/2026 | [AWS Study Group Docs](https://cloudjourney.awsstudygroup.com/) |
| Sat | Consolidated the first two weeks' learnings and sketched an initial idea for the personal project to start in week 3. | 05/02/2026 | 05/03/2026 | [AWS Study Group Docs](https://cloudjourney.awsstudygroup.com/) |

### Outcomes
* Successfully built a basic VPC model with separate public and private subnets.
* Comfortable working with S3: creating buckets, uploading objects, managing permissions, and understanding the difference between Bucket Policy and IAM Policy.
* Wrote a custom IAM policy following the principle of least privilege.
