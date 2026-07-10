# TheraNest (theranest)

TheraNest - now marketed as **Ensora Mental Health**, from **Ensora Health** (formerly **Therapy Brands**) - is a behavioral and mental health practice management and EHR platform for therapists, counselors, psychologists, and social workers. It covers client intake, scheduling, telehealth, clinical documentation and notes, treatment plans, client portals, insurance billing and claims, and reporting.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/theranest/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/theranest/refs/heads/main/apis.yml)

## API Access Model - Gated / No Public Developer API

This entry is documented honestly as a **gated provider**. As of this review (July 2026), TheraNest does **not** publish a documented, self-serve public developer API:

- There is **no developer portal**, no public API reference, no published base URL, and no self-serve authentication.
- Multiple software directories explicitly state TheraNest does not offer an API.
- The one "TheraNest API" that circulates is an **unofficial third-party layer** (Supergood) that reverse-engineers authenticated browser flows - it is not an official TheraNest product, and it exists precisely because TheraNest has "limited public APIs."
- Ensora marketing references "interoperable APIs" for integrating external data sources, but this is HIPAA-gated interoperability and partner integration - arranged via contact-sales and a business-associate agreement - not an open API.

Because TheraNest handles protected health information (PHI) under HIPAA, any programmatic access is partner- and BAA-gated by design.

### Modeled APIs

The API entries in `apis.yml` are **logical resource groupings modeled from the product surface** (`endpointsModeled: true`). They are **not** documented public endpoints, and no endpoints were fabricated:

- **TheraNest Clients API** - client demographics, insurance policies, diagnoses, portal status.
- **TheraNest Appointments API** - scheduling, recurring sessions, telehealth settings, service codes, reminders.
- **TheraNest Clinical Notes API** - progress notes, treatment plans, templates, sign-off / locking.
- **TheraNest Billing and Claims API** - invoices, payments, eligibility/authorizations, CMS-1500 / 837P claims, clearinghouse routing.

## Tags

- Behavioral Health
- Mental Health
- EHR
- Practice Management
- Healthcare
- HIPAA
- Telehealth
- Ensora Health
- Therapy Brands

## Timestamps

- **Created:** 2026-07-10
- **Modified:** 2026-07-10

## Pricing

TheraNest is sold as a **per-therapist SaaS subscription**, not as an API product. Published tiers (grounded July 2026; verify on the current pricing page):

- **Essentials** - from **$29 / therapist / month**; telehealth is an add-on.
- **Advanced** - mid tier; per-therapist price varies and is not consistently published.
- **Premier** - **$89 / therapist / month**, telehealth included.
- **AMA CPT license fee** - about **$19.50 / therapist / year**, billed each December.
- **Additional admin users** - $19/mo (Essentials/Advanced), $29/mo (Premier).

There is no metered API tier or developer pricing; partner/interoperability access is negotiated directly (contact sales). See [`plans/theranest-plans-pricing.yml`](plans/theranest-plans-pricing.yml) and [`finops/theranest-finops.yml`](finops/theranest-finops.yml).

## In-Product Integrations

Google Calendar, iCloud Calendar, Zoom (telehealth), QuickBooks, Square, and DocuSign (e-signature on notes) - all delivered as in-product integrations and partnerships, not via an open API.

## Common Properties

- [LinkedIn](https://www.linkedin.com/company/ensora-health)
- [Website](https://theranest.com)
- [Documentation / Knowledge Base](https://theranest.zendesk.com/hc/en-us)
- [Plans](plans/theranest-plans-pricing.yml)
- [Fin Ops](finops/theranest-finops.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
