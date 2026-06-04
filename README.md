# University of Edinburgh (university-of-edinburgh)

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
