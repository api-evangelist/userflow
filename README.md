# Userflow (userflow)

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

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
