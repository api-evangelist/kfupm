# King Fahd University of Petroleum & Minerals

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

King Fahd University of Petroleum & Minerals (KFUPM) is a public research university in Dhahran, Saudi Arabia. Its programmable footprint is small, and most of what previously appeared in this profile was not its own: 37 OpenAPI definitions attributed to KFUPM here were the Elsevier Pure Web Services contract (info.title "Pure API", contact pure-support@elsevier.com, version 5.35.3-4) served from the university's Pure tenant at pure.kfupm.edu.sa. That contract is Elsevier's and has been removed; the tenant relationship is recorded instead. What KFUPM genuinely operates is three surfaces on its own infrastructure. Its identity provider at sts.kfupm.edu.sa publishes signed SAML 2.0 federation metadata and an OpenID Connect discovery document, and is registered in eduGAIN through MAEEN, the Saudi identity federation, with scope kfupm.edu.sa — an institution-operated machine-readable surface by definition. The KFUPM ePrints repository (EPrints 3.4.1) serves a live, unauthenticated OAI-PMH 2.0 harvesting interface with six working verbs and six metadata formats, plus record-level and search-level JSON export whose record model carries a KFUPM-local `arabic_abstract` field. The registrar publishes a live course offering system, but it answers only an HTML form POST and returns no machine-readable format. There is no central developer portal, no API documentation, no changelog, no status page, no robots.txt, no sitemap and no llms.txt on the university's own domain. The library discovery surface sits behind a Cloudflare bot challenge. KFUPM does not publish an OpenAPI for anything it operates; the three descriptions in this repo were derived by probing the live endpoints.

**Areas:** University · Higher Education · Education · Research · Saudi Arabia · Middle East · Identity Federation · Research Repository · Open Access · OAI-PMH · Theses · Course Catalog

## King Fahd University of Petroleum & Minerals on APIs.io

Everything profiled for King Fahd University of Petroleum & Minerals is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/kfupm/](https://apis.io/providers/kfupm/)** — or go straight to one of the APIs or properties below.

### APIs (6)

- [KFUPM Elsevier Pure Web Services (tenant deployment)](https://apis.io/apis/kfupm/pure-tenant/) — KFUPM runs an Elsevier Pure research information system at pure.kfupm.edu.sa and its Pure Web Services REST API is reachable at /ws/api, authenticated with…
- [King Fahd University of Petroleum & Minerals Discovery API](https://apis.io/apis/kfupm/kfupm-discovery-api/) — Unauthenticated metadata endpoints. All three fetched live 2026-08-30.
- [King Fahd University of Petroleum & Minerals Export API](https://apis.io/apis/kfupm/kfupm-export-api/) — Record-level export in a named format.
- [King Fahd University of Petroleum & Minerals Oai Pmh API](https://apis.io/apis/kfupm/kfupm-oai-pmh-api/) — OAI-PMH 2.0 protocol requests. All six verbs verified live 2026-08-30.
- [King Fahd University of Petroleum & Minerals Search API](https://apis.io/apis/kfupm/kfupm-search-api/) — Free-text search with a machine-readable output format.
- [King Fahd University of Petroleum & Minerals Oauth2 API](https://apis.io/apis/kfupm/kfupm-oauth2-api/) — OAuth 2.0 / OpenID Connect endpoints as declared by KFUPM's own discovery document.

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### JSON Schema (1)

The data models the API reads and writes.

- [KFUPM ePrints Record](https://apis.io/schemas/kfupm/kfupm-eprints-record/)

#### Vocabulary (1)

The provider's domain terms, defined.

- [KFUPM Pure Web Services Vocabulary](https://apis.io/vocabularies/kfupm/kfupm-vocabulary/)

#### Examples (1)

Example requests and responses.

- [Kfupm Sts Openid Configuration](https://apis.io/examples/kfupm/kfupm-sts-openid-configuration/)

#### Security (2)

Authentication, trust centre, and vulnerability disclosure.

- [Kfupm Authentication](https://apis.io/security/kfupm/kfupm-authentication/)
- [Kfupm Domain Security](https://apis.io/security/kfupm/kfupm-domain-security/)

#### OAuth scopes (1)

The permissions the API asks for.

- [Kfupm Scopes](https://apis.io/scopes/kfupm/kfupm-scopes/)

#### Plans and pricing (1)

Published plans, tiers and prices.

- [Kfupm Plans Pricing](https://apis.io/plans/kfupm/kfupm-plans-pricing/)

#### Rate limits (1)

Published request limits.

- [Kfupm Rate Limits](https://apis.io/rate-limits/kfupm/kfupm-rate-limits/)

#### FinOps (1)

What the API costs to run, by operation.

- [Kfupm Finops](https://apis.io/finops/kfupm/kfupm-finops/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://www.kfupm.edu.sa/)
- [Blog](https://news.kfupm.edu.sa/)
- [Terms of service](https://www.kfupm.edu.sa/terms-of-use)
- [Privacy policy](https://www.kfupm.edu.sa/privacy-policy)
- [GitHub](https://github.com/KFUPM-OSC)

## API Evangelist rating

**Kin Score 32.4** — thin · rubric 0.24.0 · scored 2026-10-17

| Facet | Score |
|---|---|
| Discoverability | 71.4 |
| Contract quality | 48.5 |
| Contract governance | 3.8 |
| Operational transparency | 7.9 |
| Developer ergonomics | 23.8 |
| Access clarity | 26.3 |

**Agent readiness 22.4** — agent-aware

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | — |
| Reversibility Documented | — |
| MCP Server | — |
| Auth Clarity | negotiable (partial credit) |
| Idempotency | — |
| Error Semantics | — |
| OpenAPI Examples | documented (partial credit) |
| Rate Limit Signal | derived (partial credit) |
| Event Surface Described | — |
| Agent Skills | — |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | documented (partial credit) |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |

**Regulatory alignment 34.3** — Education & Research

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/kfupm/](https://apis.io/providers/kfupm/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for King Fahd University of Petroleum & Minerals: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/kfupm/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
