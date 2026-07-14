---
title: "Week 4: ASP.NET Core Backend Setup"
date: 2026-07-10
weight: 4
chapter: false
---

## Week 4: Setting up the Backend with ASP.NET Core and PostgreSQL

### Daily log

| Day | Work done | Start date | Completion date | Reference |
| ---- | ---- | ---- | ---- | ---- |
| Mon | Scaffolded a new Web API project with ASP.NET Core (.NET 10) using `dotnet new webapi`. | 05/11/2026 | 05/11/2026 | [AWS Study Group Docs](https://cloudjourney.awsstudygroup.com/) |
| Tue | Reorganized the folder structure into layers: `Controllers`, `Entities`, `DTOs`, `Services`, `Repositories`, to keep the codebase maintainable as the project grows. | 05/12/2026 | 05/12/2026 | [AWS Study Group Docs](https://cloudjourney.awsstudygroup.com/) |
| Wed | Set up PostgreSQL locally via Docker Compose instead of installing it directly on my machine. | 05/13/2026 | 05/13/2026 | [AWS Study Group Docs](https://cloudjourney.awsstudygroup.com/) |
| Thu | Ran into a connection error because the PostgreSQL Docker container wasn't exposing the port correctly, fixed by reviewing `docker-compose.yml` and the `5432:5432` port mapping. | 05/14/2026 | 05/14/2026 | [AWS Study Group Docs](https://cloudjourney.awsstudygroup.com/) |
| Fri | Installed `Npgsql.EntityFrameworkCore.PostgreSQL` and wrote a `DbContext` mapping the 6 entities designed in week 3. | 05/15/2026 | 05/15/2026 | [AWS Study Group Docs](https://cloudjourney.awsstudygroup.com/) |
| Sat | Ran the first migration, verified tables in PostgreSQL using DBeaver, and enabled Swagger UI for quick API testing. | 05/16/2026 | 05/17/2026 | [AWS Study Group Docs](https://cloudjourney.awsstudygroup.com/) |

### Outcomes
*   The Backend runs and connects reliably to the local PostgreSQL instance via Docker.
*   All 6 tables were migrated successfully, matching the ERD.
*   Enabled Swagger UI for quick API testing during development, without needing an external tool like Postman yet.
