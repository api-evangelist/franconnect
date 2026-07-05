# FranConnect (franconnect)

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
