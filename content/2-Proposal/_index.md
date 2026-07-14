---
title: "Project Proposal"
date: 2026-07-10
weight: 3
chapter: false
pre: " <b> 2. </b> "
---

## SmartDorm — A Proposal for a Dormitory Management System

### Background & motivation
While exploring the problem space, I noticed that dormitory and rental room management in many places still relies on paper records or scattered spreadsheets: utility readings recorded by hand, contracts kept as printouts, payment reminders sent through personal messages. This approach loses data easily, wastes time reconciling numbers, and doesn't scale as the number of rooms grows. That's why I proposed **SmartDorm**, focused on solving this with a solid Backend running on AWS, while I only contributed basic support on the UI side alongside a teammate.

### My scope in the project
*   Designing and building the entire **Backend API** with ASP.NET Core: room management, rental applications, contracts, and utility billing.
*   Designing the relational database schema in PostgreSQL and deploying it to Amazon RDS.
*   Writing the infrastructure as code with Terraform and deploying the Backend in a serverless setup on AWS Lambda.
*   Providing basic support on the frontend side: API documentation, sample request snippets, and joint testing of business flows once the UI was ready.

### Problems to solve
*   Manual utility meter readings are error-prone and hard to reconcile at month-end.
*   No centralized place to store tenant records and rental contracts.
*   Keeping a server running 24/7 to serve just a few dozen requests a day is an unnecessary cost.

### Technical approach (AWS)
I chose a serverless architecture to keep operating costs minimal during the pilot phase:
*   **AWS Lambda** runs the ASP.NET Core Backend, billed only for actual invocations rather than a fixed server-hour cost.
*   **Amazon API Gateway (HTTP API)** serves as the entry point for all client requests.
*   **Amazon RDS PostgreSQL** stores relational data, using a cost-optimized instance eligible for the Free Tier.
*   **Amazon S3** stores user-uploaded avatar and ID card images, and also hosts the static assets for the demo UI.

### Implementation plan — 3 phases
*   **Phase 1 (Weeks 1-4):** Review AWS fundamentals, design the ERD, scaffold the Backend, and connect to a local database.
*   **Phase 2 (Weeks 5-9):** Build out the core business APIs (rooms, applications, contracts, invoices), add JWT authentication, and work with the teammate on the UI to get a basic demo running.
*   **Phase 3 (Weeks 10-12):** Write the Terraform infrastructure, deploy the Backend to a real serverless environment, migrate file storage to S3, and finalize handoff documentation.

### Anticipated risks
*   **Lambda can't write to local disk:** since its filesystem is read-only, I planned from the start to move file storage to S3 rather than local disk.
*   **CORS errors between frontend and backend on different domains:** configured CORS policy clearly at both the application layer and API Gateway to avoid issues mid-project.
