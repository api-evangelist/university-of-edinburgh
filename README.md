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

The University of Edinburgh is a public research university in Scotland, United Kingdom, founded in 1582 and ranked #20 in the QS World University Rankings 2025. This repository catalogs its public developer/API footprint as an APIs.json provider profile for the API Evangelist network. The footprint centres on open research infrastructure — the Edinburgh DataShare research-data repository and the Pure / Edinburgh Research Explorer research information system — alongside an internal, SSO-gated Enterprise APIs programme.

- APIs.json: https://raw.githubusercontent.com/api-evangelist/university-of-edinburgh/refs/heads/main/apis.yml
- Run with Naftiko: https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=university-of-edinburgh-api-evangelist&utm_content=repo

## Type

- university / Public Research University / Index / Provider / Public

## Tags

University, Higher Education, Education, United Kingdom, Scotland, Russell Group, Research Repository, Open Data, Identity Federation, Research Computing, OAI-PMH, Artificial Intelligence

## APIs

Every surface carries an `x-operator` recording **who runs the thing the contract describes**.
Re-profiled 2026-08-19 against the operator axis.

### Institution-operated

- **Edinburgh DataShare REST API** — DSpace 8.3 REST API for the open-access research-data repository. Base: `https://datashare.ed.ac.uk/server/api`. Communities/collections/discovery readable anonymously; items and bitstreams return 401.
- **Edinburgh DataShare OAI-PMH** — OAI-PMH 2.0, fully anonymous, 12 metadata prefixes including rioxx and uketd_dc. DataCite DOIs under 10.7488/ds. Base: `https://datashare.ed.ac.uk/server/oai`
- **Edinburgh Research Archive (ERA) REST API** — a second DSpace 8.3 repository, for theses and publications. Base: `https://era.ed.ac.uk/server/api`
- **Edinburgh Research Archive (ERA) OAI-PMH** — OAI-PMH 2.0, 13 prefixes including etdms. DOIs under 10.7488/era. Base: `https://era.ed.ac.uk/server/oai`
- **EIDF Data Catalogue API** — CKAN 2.11.3 Action API for the Edinburgh International Data Facility, run by EPCC. Base: `https://catalogue.eidf.ac.uk/api/3/action`
- **ELM — Edinburgh Language Models API** — OpenAI-compatible generative-AI gateway built by EDINA for UK tertiary education. Bearer auth, no public signup. Base: `https://elm.edina.ac.uk/api/v1`
- **Shibboleth Identity Provider** — SAML 2.0 entity metadata published unauthenticated. entityID `https://idp.ed.ac.uk/shibboleth`
- **Enterprise API Gateway (gated)** — WSO2 Choreo gateway at `https://api.ed.ac.uk`. Live, Edinburgh-operated, no public route or developer portal.

### Tenant (institution's data, vendor's contract — not saved here)

- **Edinburgh Research Explorer (Elsevier Pure)** — `https://www.research.ed.ac.uk/`. Pure's API contract belongs to Elsevier. Its OAI-PMH endpoint returned HTTP 500 on 2026-08-19.
- **DiscoverEd Library Discovery (Ex Libris Primo)** — `https://discovered.ed.ac.uk/`

### Retired

- **Edinburgh DataShare DSpace 6 legacy `/rest` API** — now returns 404. Seven OpenAPI documents describing this endpoint were removed from this repository on 2026-08-19. The University library blog post documenting it is still live and still points at the dead API.

## Plans / Rate Limits / FinOps

- Plans: [plans/university-of-edinburgh-plans-pricing.yml](plans/university-of-edinburgh-plans-pricing.yml)
- Rate Limits: [rate-limits/university-of-edinburgh-rate-limits.yml](rate-limits/university-of-edinburgh-rate-limits.yml)
- FinOps: [finops/university-of-edinburgh-finops.yml](finops/university-of-edinburgh-finops.yml)

## Timestamps

- Created: 2026-06-03
- Modified: 2026-08-19

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
