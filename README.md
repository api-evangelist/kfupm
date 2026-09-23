# King Fahd University of Petroleum & Minerals (kfupm)

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

King Fahd University of Petroleum & Minerals (KFUPM) is a public research university in Dhahran, Saudi Arabia. Its programmable footprint is small and, until this re-profile, largely misattributed: 37 OpenAPI definitions catalogued here as KFUPM's were the Elsevier Pure Web Services contract (`info.title: Pure API`, `contact: pure-support@elsevier.com`, version 5.35.3-4) served from the university's Pure tenant at `pure.kfupm.edu.sa`. That contract is Elsevier's. It has been removed and the tenant relationship recorded once instead.

What KFUPM genuinely operates is three surfaces on its own infrastructure, all verified live on 2026-08-30 and none of them previously in this profile.

- APIs.json: https://raw.githubusercontent.com/api-evangelist/kfupm/refs/heads/main/apis.yml
- Run with Naftiko: https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=kfupm-api-evangelist&utm_content=repo

## Type

- University / Public Research University / Index / Consumer / Public

## Tags

University, Higher Education, Education, Research, Saudi Arabia, Middle East, Identity Federation, Research Repository, Open Access, OAI-PMH, Theses, Course Catalog

## APIs

Every entry carries an operator. `institution` means KFUPM runs the thing the contract describes; `tenant` means KFUPM runs a deployment of somebody else's product and the contract belongs to that vendor.

- **KFUPM Identity Federation (SAML 2.0 + OpenID Connect)** — `x-operator: institution`. KFUPM's own AD FS identity provider. Signed SAML 2.0 federation metadata (80 KB, entityID `http://sts.kfupm.edu.sa/adfs/services/trust`) and an OpenID Connect discovery document for issuer `https://sts.kfupm.edu.sa/adfs`, with a two-key RS256 JWKS. Registered in eduGAIN as entity 671205 by MAEEN (SA-MIF), scope `kfupm.edu.sa`. Base: https://sts.kfupm.edu.sa
- **KFUPM ePrints OAI-PMH Repository Interface** — `x-operator: institution`. Live OAI-PMH 2.0 on a self-hosted EPrints 3.4.1 repository. All six verbs verified; six metadata formats (didl, mets, oai_bibl, oai_dc, rdf, uketd_dc). No authentication. Base: https://eprints.kfupm.edu.sa/cgi/oai2
- **KFUPM ePrints Export & Search (JSON)** — `x-operator: institution`. Unauthenticated record-level and search-level JSON from the same repository. The record model carries a KFUPM-local `arabic_abstract` field. Base: https://eprints.kfupm.edu.sa/cgi
- **KFUPM Elsevier Pure Web Services (tenant deployment)** — `x-operator: tenant`, vendor Elsevier. Recorded as a relationship; the contract is deliberately not saved here. Base: https://pure.kfupm.edu.sa/ws/api

## Artifacts

- OpenAPI (all three derived by probe — KFUPM publishes none): [openapi/](openapi/)
- Conformance (education regime: `oai-pmh`, `saml`): [conformance/kfupm-conformance.yml](conformance/kfupm-conformance.yml)
- Authentication: [authentication/kfupm-authentication.yml](authentication/kfupm-authentication.yml)
- Scopes: [scopes/kfupm-scopes.yml](scopes/kfupm-scopes.yml)
- Errors: [errors/kfupm-errors.yml](errors/kfupm-errors.yml)
- Lifecycle: [lifecycle/kfupm-lifecycle.yml](lifecycle/kfupm-lifecycle.yml)
- Vocabulary: [vocabulary/kfupm-vocabulary.yml](vocabulary/kfupm-vocabulary.yml)
- JSON Schema: [json-schema/kfupm-eprints-record-schema.json](json-schema/kfupm-eprints-record-schema.json)
- Examples (probed responses): [examples/](examples/)

## Plans / Rate Limits / FinOps

- Plans & Pricing: [plans/kfupm-plans-pricing.yml](plans/kfupm-plans-pricing.yml)
- Rate Limits: [rate-limits/kfupm-rate-limits.yml](rate-limits/kfupm-rate-limits.yml)
- FinOps: [finops/kfupm-finops.yml](finops/kfupm-finops.yml)

## Timestamps

- Created: 2026-06-03
- Modified: 2026-08-30

## Common Properties

- Website: https://www.kfupm.edu.sa/
- Terms of Service: https://www.kfupm.edu.sa/terms-of-use
- Privacy Policy: https://www.kfupm.edu.sa/privacy-policy
- Blog: https://news.kfupm.edu.sa/
- LinkedIn: https://www.linkedin.com/school/kfupm/
- Identity Federation: https://sts.kfupm.edu.sa/FederationMetadata/2007-06/FederationMetadata.xml
- Research Repository (ePrints): https://eprints.kfupm.edu.sa/
- Research Portal (Elsevier Pure tenant): https://pure.kfupm.edu.sa/
- Course Catalog: https://registrar.kfupm.edu.sa/courses-classes/course-offering1/
- Library Catalog: https://library.kfupm.edu.sa/
- AI Tooling (AI+X): https://www.kfupm.edu.sa/about-us/discover/ai-x
- GitHub Organization (student Open Source Club): https://github.com/KFUPM-OSC

## Notes

- KFUPM publishes no developer portal, no API documentation, no OpenAPI, no changelog, no status page, no `robots.txt`, no `sitemap.xml` and no `llms.txt` on its own domain.
- The identity federation surface is the significant find: an institution-operated SAML 2.0 IdP with published metadata and an OIDC discovery document, registered in eduGAIN via the Saudi federation MAEEN. It had never been catalogued.
- The ePrints OAI-PMH `Identify` response declares no metadata, data or submission policy — it still carries the EPrints defaults, so reuse rights for harvested metadata are undeclared.
- OAI-PMH protocol errors are returned with HTTP 200 and an `<error code>` element; a harvester reading only the HTTP status will treat a failed request as a success.
- The registrar course offering system is institution-operated but answers only an HTML form POST — no JSON, no machine-readable format.
- `library.kfupm.edu.sa` is live behind a Cloudflare bot challenge (403 to non-browser clients). Live, not dead; machine-unreadable.
- The `github.com/kfupm` organization has zero public repositories, no description and has not been touched since 2019. Ownership by the university is unevidenced, so it was dropped as a pointer.
- The LinkedIn school page returns HTTP 999 to automated probes (bot-block); the page exists in a browser.
- The ePrints JSON export exposes personal data — depositor `contact_email`, advisor and committee names — and internal EPrints fields (`dir`, `userid`). No live personal values are stored in this repo.
- No endpoints were fabricated. The three OpenAPI descriptions here are marked `method: derived` and every path, parameter and error code in them was observed in a live response.

## Maintainers

- Kin Lane — kin@apievangelist.com
