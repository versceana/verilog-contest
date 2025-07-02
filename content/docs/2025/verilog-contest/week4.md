---
title: "Week #4"
---

# **Week #4**

## Testing and QA

*Summary of testing strategy and types of tests implemented.*
We have implemented a combination of unit tests and Postman-based integration tests for API endpoints. All tests are automatically executed in the CI pipeline on every pull request and push to dev.

### Evidence of test execution

- Link to Postman collection: https://www.postman.com/collections/f38f971d0b2e5a4c65bb
- CI logs: https://github.com/IU-Capstone-Project-2025/verilog-contest/actions/runs/16031851882/job/45234142892

## CI/CD

The CI/CD pipeline is built with GitHub Actions, triggered by PRs to main, pushes to dev/devops, and manual dispatch. It includes four stages:

**1. Backend checks:** staticcheck, gofmt, go test

**2. Frontend checks:** npm ci, Prettier formatting, ESLint linting

**3. Compose tests:** Docker Compose up, container health checks, HTTP response validation

**4. Push images:** Authenticate to GHCR, build & push Docker images for all services

Challenges faced: intermittent port conflicts in compose tests and occasional flakiness in Postman collection runs, both mitigated by pre-test cleanup scripts.



### Links to CI/CD configuration files

- CI/CD file: https://github.com/IU-Capstone-Project-2025/verilog-contest/blob/main/.github/workflows/ci.yaml

## Deployment

### Staging

We deploy to staging using Docker Compose orchestrated by Coolify + Nixpacks, exposing services through a Cloudflare tunnel. ICD club servers host the environment; secrets and .env are managed securely.

### Production

Currently, our production environment is hosted on a single VPS (ICD club server) using docker-compose. The deployment steps are:

 - **Image build & push:** On merge to main, GitHub Actions builds Docker images and pushes them to GHCR.

- **Compose deployment:** The server pulls images from GHCR and runs docker-compose to update services.

 - **DNS & SSL:** The domain is **https://platform.innochipdesign.ru/**.

## Vibe Check

*Facilitate a team health check. Discuss progress, roadblocks, and team dynamics. Ensure everyone feels heard.*

# Weekly commitments

## Individual contribution of each participant

| Team Member            | Week #2 Contributions                                                                      |
| ---------------------- | ------------------------------------------------------------------------------------------ |
| **Mikhail Panteleev**  | Social communication for finding server (+ domen + ssl), initial service and bugs fix in backend, hard thinking about jadger parser, deploy.                       |
| **Vladislav Merkulov** | Runner integration into system, testing.                       |
| **Aleksei Fominykh**   | Developing Judger parser, staging, kuber.                                         |
| **Sofia Kulagina**     | CI/CD using docker-compose instead of build and pushing in GitHub container, initial service in CI/CD.             |
| **Diana Yakupova**     | Meeting organization, report, backend api in contest components, configure api in api client with auth.|


## Plan for Next Week

In Week #5, our goal is to finilize testing, provide more backend API in frontend, bug fixing and finilizing judger-parser in backend. We will also work on deploying the application to production.

## Confirmation of the code's operability

We confirm that the code in the main branch:
- [✔] In working condition.
- [✔] Run via docker-compose (or another alternative described in the `README.md`).