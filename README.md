# King Fahd University of Petroleum & Minerals (kfupm)

King Fahd University of Petroleum & Minerals (KFUPM) is a public research university in Dhahran, Saudi Arabia, ranked #101 in the QS World University Rankings 2025. KFUPM does not run a centralized public developer portal, but several institutional systems expose machine-readable interfaces — the KFUPM ePrints repository (OAI-PMH 2.0 + EPrints REST/search URLs) and the Elsevier Pure research portal (Pure Web Services REST API, authentication-gated).

- APIs.json: https://raw.githubusercontent.com/api-evangelist/kfupm/refs/heads/main/apis.yml
- Run with Naftiko: https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=kfupm-api-evangelist&utm_content=repo

## Type

- Index / Consumer / 3rd-Party

## Tags

Education, Higher Education, University, Research, Open Access, Repository, Saudi Arabia, Middle East

## APIs

- **KFUPM ePrints OAI-PMH** — OAI-PMH 2.0 harvesting for the theses and dissertations repository. Docs: https://eprints.kfupm.edu.sa/ · Base: https://eprints.kfupm.edu.sa/cgi/oai2
- **KFUPM ePrints REST / Search** — Addressable EPrints records and public search. Docs: https://eprints.kfupm.edu.sa/ · Base: https://eprints.kfupm.edu.sa/id/eprint/
- **KFUPM Pure Web Services API** — Elsevier Pure REST API (OpenAPI 3), authentication-gated. Docs: https://pure.kfupm.edu.sa/ · Base: https://pure.kfupm.edu.sa/ws/api/

## Plans / Rate Limits / FinOps

- Plans & Pricing: [plans/kfupm-plans-pricing.yml](plans/kfupm-plans-pricing.yml)
- Rate Limits: [rate-limits/kfupm-rate-limits.yml](rate-limits/kfupm-rate-limits.yml)
- FinOps: [finops/kfupm-finops.yml](finops/kfupm-finops.yml)

## Timestamps

- Created: 2026-06-03
- Modified: 2026-06-03

## Common Properties

- Website: https://www.kfupm.edu.sa/
- GitHub: https://github.com/kfupm
- Source Code (Open Source Club): https://github.com/KFUPM-OSC
- LinkedIn: https://www.linkedin.com/school/kfupm/
- Repository (ePrints): https://eprints.kfupm.edu.sa/
- Research Portal (Pure): https://pure.kfupm.edu.sa/

## Notes

- No centralized public developer portal was found for KFUPM.
- ePrints OAI-PMH was verified live (Identify returns repositoryName "KFUPM ePrints", protocol 2.0).
- The Pure Web Services API exists but is authentication-gated (versioned endpoint returns HTTP 401); it is not an open public API.
- The github.com/kfupm organization exists but currently has no public repositories.
- The LinkedIn school page returns HTTP 999 to automated probes (bot-block); the page exists in a browser.
- No endpoints were fabricated; only confirmed URLs are cataloged.

## Maintainers

- Kin Lane — kin@apievangelist.com
