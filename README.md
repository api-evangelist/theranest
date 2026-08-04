# TheraNest (theranest)

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
