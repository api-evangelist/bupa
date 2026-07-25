# Bupa (bupa)

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
