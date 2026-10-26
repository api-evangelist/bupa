# Bupa (bupa)

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

Bupa is a United Kingdom headquartered international healthcare group that writes private medical insurance and also runs the clinics, dental practices, hospitals and aged-care homes that deliver the care it funds. It has no shareholders, is owned by the British United Provident Association Limited and reinvests its profits, and operates market units across the UK, Australia and New Zealand, Spain and Latin America (Sanitas, Bupa Chile), Türkiye, Poland, Hong Kong SAR, India and the Middle East, plus the Bupa Global international private medical insurance business.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/bupa/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/bupa/refs/heads/main/apis.yml)

## Tags

- Insurance
- United Kingdom
- Health Insurance
- Life and Health
- Carrier
- Healthcare
- Aged Care
- Claims
- Policy Administration
- Partner Gated

## Timestamps

- **Created:** 2026-07-25
- **Modified:** 2026-07-25

## APIs

None listed.

Bupa publishes no public, self-serve API. This is an honest and expected finding for a life-and-health carrier in a market with no open-insurance obligation — the UK has the FCA and PRA but no open-insurance rule, the FCA's Open Finance work is still consultation, and the London Market's Blueprint Two modernization programme is aimed at brokers and syndicates in the subscription P&C market rather than at a health carrier or at outside developers.

What exists instead:

- **Group level (bupa.com) — nothing.** `developer.bupa.com`, `developers.bupa.com`, `docs.bupa.com` and `api.bupa.com` do not resolve. `/developers`, `/api`, `/developer` and `/integrations` all return HTTP 404. `/partners` redirects off-domain to a Saba learning-cloud partner training site.
- **Bupa Australia — a real portal, but gated.** [portal.api.bupa.com.au](https://portal.api.bupa.com.au/) returns HTTP 200 and is a genuine Azure API Management developer portal, but it lists no APIs to anonymous visitors and its [Get Started](https://portal.api.bupa.com.au/get-started) page routes every step through the Bupa Integration Fabric Team: *"Contact the Bupa Integration Fabric Team with your interest to get access to our API specifications."* The portal's own `config.json` points at an internal-only APIM management host, so the catalog cannot be read from outside.
- **Bupa Chile — a login wall.** [apidoc.bupa.cl](https://apidoc.bupa.cl/) is an Angular single-page app fronted by Microsoft Entra ID; its backend `https://api.bupa.cl/portal/ms-controller` returns HTTP 401 to every anonymous request.
- **Bupa Global — decommissioned.** `api-portal.bupaglobal.com` is indexed by third parties but no longer resolves.
- **UK intermediaries — a broker portal, not an API.** The UK channel for brokers and intermediaries is the login-gated Bupa Connect web portal for quotes and cover.

## Sector signals

- **ACORD posture:** no ACORD reference found. No mention of ACORD, AL3, ACORD XML, NGDS or ACORD certification appears anywhere on Bupa's public estate — consistent with a private medical insurance and healthcare provision book rather than P&C or life.
- **Quote / bind / issue / FNOL:** none publicly exposed. Claims run through the myBupa member app and gated provider channels.
- **Auth model:** OAuth2 authorization code via Microsoft Entra ID guards the Chile portal; Azure APIM subscription keys are implied by the Australian portal's copy but are not publicly documented.
- **Webhooks / events / Postman / GraphQL / gRPC:** none found.
- **OpenAPI harvested:** 0 specifications. Candidate spec paths were probed against `api.bupa.com.au` (all HTTP 502) and `api.bupa.cl` (all HTTP 401). No `openapi/` directory is included, because nothing real was available to save.

Full probe log, HTTP statuses and provenance are in [review.yml](review.yml).

## Links

- [Website](https://www.bupa.com/)
- [News](https://www.bupa.com/news)
- [LinkedIn](https://www.linkedin.com/company/bupa)
- [Bupa Developer Portal (Australia)](https://portal.api.bupa.com.au/)
- [Get Started (Australia)](https://portal.api.bupa.com.au/get-started)
- [Portal de APIs Bupa (Chile)](https://apidoc.bupa.cl/)
