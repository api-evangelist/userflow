# Userflow (userflow)

Userflow is a product onboarding and adoption platform that enables product teams to build in-app guided flows, checklists, announcements, and NPS surveys without requiring engineering resources. The platform provides a REST API for managing users, tracking events, and organizing users into groups or companies from a back-end application. Userflow supports data synchronization via API keys with Bearer token authentication, allowing real-time user attribute updates and event tracking to power personalized onboarding experiences. The platform targets SaaS companies seeking to improve activation rates, feature adoption, and overall user retention through guided in-app engagement.

**APIs.json:** https://raw.githubusercontent.com/api-evangelist/userflow/refs/heads/main/apis.yml

**Naftiko:** https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=userflow-api-evangelist&utm_content=repo

---

## Tags

- User Onboarding
- Product Adoption
- In-App Guides
- Checklists
- Announcements
- NPS Surveys
- User Flows
- SaaS
- Product-Led Growth

---

## APIs

### Userflow REST API

The Userflow REST API allows back-end applications to synchronize user data, track events, and manage groups or companies within the Userflow platform. It provides endpoints for creating, updating, and deleting users; listing and querying users with cursor-based pagination; posting custom events that trigger flow conditions; and managing group memberships. Authentication uses Bearer token API keys scoped per environment.

- **Base URL:** https://api.userflow.com
- **Documentation:** https://docs.userflow.com/docs/api
- **Authentication:** Bearer token (API key from Settings -> API)

**Key Resources:**
- `POST /users/{user_id}` — Create or update (upsert) a user
- `GET /users/{user_id}` — Retrieve a specific user
- `GET /users` — List users (cursor-based pagination)
- `DELETE /users/{user_id}` — Remove a user
- `POST /events` — Track custom product events
- `POST /groups/{group_id}` — Create or update a company/group
- `GET /groups` — List groups
- `POST /group_memberships` — Add user to a group

---

## Plans / Rate Limits / FinOps

| Resource | File |
|----------|------|
| Plans & Pricing | [plans/userflow-plans-pricing.yml](plans/userflow-plans-pricing.yml) |
| Rate Limits | [rate-limits/userflow-rate-limits.yml](rate-limits/userflow-rate-limits.yml) |
| FinOps | [finops/userflow-finops.yml](finops/userflow-finops.yml) |

**Pricing Summary:**

| Plan | Monthly | Annual (per mo) | Included MAUs |
|------|---------|-----------------|---------------|
| Startup | $300 | $240 | 3,000 |
| Pro | $850 | $680 | 10,000 |
| Enterprise | Custom | Custom | Custom |

---

## Timestamps

- **Created:** 2026-06-13
- **Modified:** 2026-06-13

---

## Common

| Type | URL |
|------|-----|
| Website | https://www.userflow.com |
| Documentation | https://docs.userflow.com/docs/dev |
| GitHub Org | https://github.com/userflow |
| LinkedIn | https://www.linkedin.com/company/userflow |
| Blog | https://www.userflow.com/blog |
| Pricing | https://www.userflow.com/pricing |
| Status Page | https://status.userflow.com |
| X (Twitter) | https://twitter.com/getuserflow |

---

## Maintainers

- **Kin Lane** — kin@apievangelist.com
