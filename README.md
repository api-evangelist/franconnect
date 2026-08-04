# FranConnect (franconnect)

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
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

FranConnect is a franchise and multi-location management platform used by 1,500+ brands across roughly one million locations, covering franchise development and sales, franchisee/unit information management, field operations and audits, financials and royalties, and CRM. Its FranConnect Sky product exposes a RESTful API - organized by module (Franchise Sales "fs", CRM "cm", Info Manager "fim", Finance "manage-finance", and Admin "admin") - that lets customers import and export data between FranConnect Sky and third-party applications. All API calls are made over HTTPS and authenticated with an Authorization-Token header.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/franconnect/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/franconnect/refs/heads/main/apis.yml)

## Access Model (Important)

FranConnect's API is **real and documented, but not open or self-serve**. It is a customer/partner-gated interface:

- You must be a **FranConnect Sky customer or integration partner** to use it.
- API credentials (the `Authorization-Token`) are **provisioned by FranConnect** for your tenant, following a REST API account creation process in the FranConnect help center.
- The detailed API reference portal at **docs.franconnect.net** requires a **signed-in account**; the public marketplace listing ([marketplace.franconnect.net/api-detail.html](https://marketplace.franconnect.net/api-detail.html)) describes the API at a high level.
- FranConnect Sky is multi-tenant SaaS, so the base URL is **tenant-specific** (modeled here as `https://{tenant}.franconnect.net`).

Because the reference documentation is gated, the per-module APIs in `apis.yml` are described from FranConnect's **publicly stated module structure**, and the exact endpoint paths are **modeled, not fabricated from a public OpenAPI**. No OpenAPI definition, Postman collection, or endpoint-level surface is asserted here beyond what FranConnect states publicly. This entry is an honest catalog of a gated enterprise API.

## Tags

- Franchise Management
- Franchise Development
- Franchise Operations
- Field Operations
- Multi-Location
- CRM
- Franchise Sales
- SaaS

## Timestamps

- **Created:** 2026-07-04
- **Modified:** 2026-07-04

## APIs

The FranConnect Sky API is organized by product module. Each logical API below maps to a documented module path segment.

### FranConnect Franchise Sales API

Franchise Sales / Development module (path segment `fs`). Import and export franchise development leads, prospects, and the franchise sales pipeline used to recruit and qualify new franchisees.

- **Human URL:** [https://docs.franconnect.net/](https://docs.franconnect.net/)
- **Base URL:** `https://{tenant}.franconnect.net`

### FranConnect CRM API

CRM module (path segment `cm`). Read and write contacts and relationship/communication records supporting franchise and consumer engagement.

- **Human URL:** [https://docs.franconnect.net/](https://docs.franconnect.net/)
- **Base URL:** `https://{tenant}.franconnect.net`

### FranConnect Info Manager API

Info Manager module (path segment `fim`). The system of record for franchisee and unit/location profiles, plus document retrieval - recent releases added dedicated REST endpoints for programmatic access to stored files and their metadata.

- **Human URL:** [https://docs.franconnect.net/](https://docs.franconnect.net/)
- **Base URL:** `https://{tenant}.franconnect.net`

### FranConnect Finance API

Finance module (path segment `manage-finance`). Import and export financial data - unit sales reporting, royalties, fees, and invoicing used to calculate and reconcile franchisee obligations.

- **Human URL:** [https://docs.franconnect.net/](https://docs.franconnect.net/)
- **Base URL:** `https://{tenant}.franconnect.net`

### FranConnect Admin API

Admin module (path segment `admin`). Administrative entities such as users, roles, and configuration that govern the FranConnect Sky tenant.

- **Human URL:** [https://docs.franconnect.net/](https://docs.franconnect.net/)
- **Base URL:** `https://{tenant}.franconnect.net`

## Common Properties

- [LinkedIn](https://www.linkedin.com/company/franconnect)
- [Website](https://www.franconnect.com/en/)
- [Documentation](https://docs.franconnect.net/)
- [API Marketplace Listing](https://marketplace.franconnect.net/api-detail.html)
- [Plans](plans/franconnect-plans-pricing.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
