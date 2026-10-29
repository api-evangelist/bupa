# Bupa

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

Bupa is a United Kingdom headquartered international healthcare group that writes private medical insurance and also runs the clinics, dental practices, hospitals and aged-care homes that deliver the care it funds. It has no shareholders, is owned by the British United Provident Association Limited and reinvests its profits, and operates market units across the UK, Australia and New Zealand, Spain and Latin America (Sanitas, Bupa Chile), Turkiye, Poland, Hong Kong SAR, India and the Middle East, plus the Bupa Global international private medical insurance business. Its lines of business are health insurance, health provision and aged care rather than property and casualty or life, so the ACORD data standards that shape the rest of the insurance sector are absent from its published surface. Bupa's API posture is partner-gated: the group site bupa.com publishes no developer portal at all (developer, developers, docs and api subdomains do not resolve, and /developers, /api and /developer return 404), and the only first-party developer surfaces belong to market units. Bupa Australia runs a real Azure API Management developer portal at portal.api.bupa.com.au that returns HTTP 200 but lists no APIs publicly, instructing prospective consumers to contact the Bupa Integration Fabric Team to get access to API specifications; Bupa Chile runs apidoc.bupa.cl behind a Microsoft Entra ID login wall whose backend returns HTTP 401 to anonymous callers; and the Bupa Global portal host api-portal.bupaglobal.com no longer resolves. No public OpenAPI or Swagger definition, no Postman collection, no GraphQL or gRPC surface, and no event or webhook catalog could be confirmed anywhere on Bupa's public web estate as of 2026-07-25, and none of the four insurance API verbs — quote, bind, issue or FNOL — is exposed to unauthenticated developers.

**Areas:** Insurance · United Kingdom · Health Insurance · Life and Health · Carrier · Healthcare · Aged Care · Claims · Policy Administration

## Bupa on APIs.io

Everything profiled for Bupa is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/bupa/](https://apis.io/providers/bupa/)** — or go straight to one of the APIs or properties below.

### APIs (2)

- [Bupa Australia APIs (Integration Fabric)](https://apis.io/apis/bupa/bupa-australia-apis-integration-fabric/) — The Bupa Australia API estate, published through an Azure API Management managed developer portal at portal.api.bupa.com.au and served from the…
- [Portal de APIs Bupa (Bupa Chile)](https://apis.io/apis/bupa/portal-de-apis-bupa-bupa-chile/) — The Bupa Chile API portal at apidoc.bupa.cl — an Angular single-page application that ships Swagger UI and renders API definitions fetched from the backend…

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### Security (3)

Authentication, trust centre, and vulnerability disclosure.

- [Bupa Authentication](https://apis.io/security/bupa/bupa-authentication/)
- [Bupa Domain Security](https://apis.io/security/bupa/bupa-domain-security/)
- [Bupa Vulnerability Disclosure](https://apis.io/security/bupa/bupa-vulnerability-disclosure/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://www.bupa.com/)
- [Documentation](https://portal.api.bupa.com.au/apis)
- [Getting started](https://portal.api.bupa.com.au/get-started)
- [API reference](https://portal.api.bupa.com.au/api-details)
- [Sign up](https://portal.api.bupa.com.au/signin)
- [Support](https://www.bupa.com/contacts)
- [Blog](https://www.bupa.com/news-and-press/news-and-stories)
- [Security](https://bugcrowd.com/engagements/bupa-aus-vdp-pro)
- [Terms of service](https://www.bupa.com.au/terms-and-conditions)
- [Privacy policy](https://www.bupa.com/important-notices/privacy-notices)
- [GitHub](https://github.com/bupa-digital)

## API Evangelist rating

**Kin Score 30.5** — thin · rubric 0.24.0 · scored 2026-10-17

| Facet | Score |
|---|---|
| Discoverability | 73.2 |
| Contract quality | 0.0 |
| Contract governance | 18.2 |
| Operational transparency | 28.9 |
| Developer ergonomics | 57.1 |
| Access clarity | 23.7 |

**Agent readiness 2.5** — human-only

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | — |
| Agentic Access | — |
| Reversibility Documented | — |
| MCP Server | — |
| Auth Clarity | bearer (partial credit) |
| Idempotency | — |
| Error Semantics | — |
| OpenAPI Examples | — |
| Rate Limit Signal | — |
| Event Surface Described | — |
| Agent Skills | — |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |

**Regulatory alignment 23.7** — Insurance

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/bupa/](https://apis.io/providers/bupa/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Bupa: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/bupa/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
