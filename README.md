# University of Edinburgh (university-of-edinburgh)

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

The University of Edinburgh is a public research university in Scotland, United Kingdom, founded in 1582 and ranked #20 in the QS World University Rankings 2025. This repository catalogs its public developer/API footprint as an APIs.json provider profile for the API Evangelist network. The footprint centres on open research infrastructure — the Edinburgh DataShare research-data repository and the Pure / Edinburgh Research Explorer research information system — alongside an internal, SSO-gated Enterprise APIs programme.

- APIs.json: https://raw.githubusercontent.com/api-evangelist/university-of-edinburgh/refs/heads/main/apis.yml
- Run with Naftiko: https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=university-of-edinburgh-api-evangelist&utm_content=repo

## Type

- Index / Consumer / 3rd-Party

## Tags

Education, Higher Education, University, Research Data, Open Data, Repository, OAI-PMH, United Kingdom, Scotland

## APIs

- **Edinburgh DataShare REST API** — DSpace REST API for the open-access research-data repository (JSON). Docs: https://libraryblogs.is.ed.ac.uk/datablog/2021/12/17/new-feature-in-edinburgh-datashare-the-rest-api/ — Base: https://datashare.ed.ac.uk/rest
- **Edinburgh DataShare OAI-PMH** — Metadata harvesting endpoint for the research-data repository. Docs: https://datashare.ed.ac.uk/oai/request?verb=Identify — Base: https://datashare.ed.ac.uk/oai/request
- **Edinburgh Research Explorer (Pure) OAI-PMH** — Public OAI-PMH endpoint for the Pure research information system. Docs: https://www.pure.ed.ac.uk/ws/oai?verb=Identify — Base: https://www.pure.ed.ac.uk/ws/oai
- **Enterprise APIs Programme (gated)** — Internal Student Records / Timetabling / Staff APIs, documented behind University SSO; not publicly accessible. Docs: https://digital-strategy.ed.ac.uk/current-programmes-projects/enterprise-apis

## Plans / Rate Limits / FinOps

- Plans: [plans/university-of-edinburgh-plans-pricing.yml](plans/university-of-edinburgh-plans-pricing.yml)
- Rate Limits: [rate-limits/university-of-edinburgh-rate-limits.yml](rate-limits/university-of-edinburgh-rate-limits.yml)
- FinOps: [finops/university-of-edinburgh-finops.yml](finops/university-of-edinburgh-finops.yml)

## Timestamps

- Created: 2026-06-03
- Modified: 2026-06-03

## Common Properties

- Website: https://www.ed.ac.uk/
- GitHub: https://github.com/uoe-is-apps
- LinkedIn: https://www.linkedin.com/school/university-of-edinburgh/
- Authentication: https://idp.ed.ac.uk/
- Plans, Rate Limits, FinOps, Review (see files above and review.yml)

## Notes

- All endpoints were probed live on 2026-06-03. DataShare REST/OAI and Pure OAI returned 200 with valid payloads. The Enterprise APIs documentation redirects to SAML SSO (idp.ed.ac.uk) and is gated/internal.
- Pure also exposes SOAP and REST web services, but developer access to those is granted case by case and is not publicly documented; only the OAI-PMH endpoint is cataloged as public.
- The verified official GitHub org with public repositories is `uoe-is-apps` (IS Applications Directorate). The `university-of-edinburgh` org exists but exposes no public repositories.
- No endpoints were fabricated. See review.yml for per-URL status.

## Maintainers

- Kin Lane — kin@apievangelist.com
