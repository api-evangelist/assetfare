# AssetFare

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

A non-custodial routing API for AI agents that returns fee-inclusive cross-chain and same-chain quotes and bounded unsigned actions; the caller's own wallet verifies, signs and submits every transaction, and AssetFare never holds keys, signs or submits. Its live v2 capabilities document (checked 2026-10-03) lists 16 chains, 20 asset endpoints and 54 active directed routes (a further 44 measured routes are inactive), with a USD 1 minimum, no business maximum and an exact 1 bp service fee on top of provider and network fees. The v2 REST contract covers capabilities, quote, prepare, a receipt-driven session lifecycle and status; the same surface is offered over MCP and A2A, and a legacy v1 compatibility API remains live.

**Areas:** AI Agents · Asset Transfer · Bridge · Cross-Chain · Non-Custodial · Cryptocurrency · Solana · Base · Arbitrum · Robinhood Chain · Optimism · Ethereum

## AssetFare on APIs.io

Everything profiled for AssetFare is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/assetfare/](https://apis.io/providers/assetfare/)** — or go straight to one of the APIs or properties below.

### APIs (6)

- [AssetFare Capabilities API](https://apis.io/apis/assetfare/assetfare-capabilities-api/) — Reads the live v2 capability document: chains, asset endpoints, active and inactive directed routes, fee policy, amount policy and execution availability.
- [AssetFare Prepare API](https://apis.io/apis/assetfare/assetfare-prepare-api/) — Returns a validated, bounded unsigned action bundle for a quote the caller has explicitly approved; the caller signs and submits.
- [AssetFare Quote API](https://apis.io/apis/assetfare/assetfare-quote-api/) — Quotes a live route with expected and minimum receive, total token-path cost, provider fees, ETA and the ordered direct-protocol provider path.
- [AssetFare Session API](https://apis.io/apis/assetfare/assetfare-session-api/) — Quote-bound, idempotent, receipt-driven sessions for multistep routes: create, read, observe source and output receipts, and refresh an expired unsubmitted…
- [AssetFare Status API](https://apis.io/apis/assetfare/assetfare-status-api/) — Reads route and provider health without creating a quote.
- [AssetFare Legacy v1 Compatibility API](https://apis.io/apis/assetfare/assetfare-legacy-v1-api/) — The earlier v1 route API (wallet auth, quote, session and status), still served for compatibility and listed in the provider's API catalog as a legacy…

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### Arazzo workflows (1)

Multi-step workflows that chain operations into a business task.

- [AssetFare read-only route evaluation](https://apis.io/arazzos/assetfare/assetfare-route-evaluation-arazzo/)

#### MCP servers (1)

Model Context Protocol servers that expose the API to agents.

- [mcp](https://apis.io/servers/assetfare/mcp/)

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Assetfare Agentic Access](https://apis.io/agentic-access/assetfare/assetfare-agentic-access/)

#### JSON-LD (1)

Linked-data contexts for the provider's vocabulary.

- [Moved to /providers/assetfare/](https://apis.io/jsonld/assetfare/assetfare-context/)

#### Overlays (2)

OpenAPI overlays, including conversational phrasing for each operation.

- [Assetfare Agent Native Route Api Overlay](https://apis.io/overlays/assetfare/assetfare-agent-native-route-api-overlay/)
- [Assetfare Openapi Overlay](https://apis.io/overlays/assetfare/assetfare-openapi-overlay/)

#### Governance rules (1)

Spectral rulesets for the provider's contracts.

- [Moved to /providers/assetfare/](https://apis.io/rules/assetfare/assetfare-rules/)

#### Security (3)

Authentication, trust centre, and vulnerability disclosure.

- [Assetfare Authentication](https://apis.io/security/assetfare/assetfare-authentication/)
- [Assetfare Domain Security](https://apis.io/security/assetfare/assetfare-domain-security/)
- [Assetfare Vulnerability Disclosure](https://apis.io/security/assetfare/assetfare-vulnerability-disclosure/)

#### Plans and pricing (1)

Published plans, tiers and prices.

- [Assetfare Plans Pricing](https://apis.io/plans/assetfare/assetfare-plans-pricing/)

#### Rate limits (1)

Published request limits.

- [Assetfare Rate Limits](https://apis.io/rate-limits/assetfare/assetfare-rate-limits/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://assetfare.dev/)
- [Documentation](https://assetfare.dev/llms-full.txt)
- [Getting started](https://assetfare.dev/pilot/)
- [Pricing](https://assetfare.dev/pricing/)
- [Terms of service](https://assetfare.dev/terms/)
- [Privacy policy](https://assetfare.dev/privacy/)
- [Status](https://api.assetfare.dev/v2/status)

## API Evangelist rating

**Kin Score 59.3** — strong · rubric 0.25.0 · scored 2026-10-23

| Facet | Score |
|---|---|
| Discoverability | 86.7 |
| Contract quality | 55.0 |
| Contract governance | 31.8 |
| Operational transparency | 63.2 |
| Developer ergonomics | 50.0 |
| Access clarity | 52.6 |

**Agent readiness 51.3** — agent-native

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | derived (partial credit) |
| Reversibility Documented | — |
| MCP Server | documented (partial credit) |
| Auth Clarity | bearer (partial credit) |
| Idempotency | verified |
| Error Semantics | verified |
| OpenAPI Examples | partial |
| Rate Limit Signal | documented (partial credit) |
| Event Surface Described | — |
| Agent Skills | yes |
| Well Known Catalog | yes |
| Consent Identity | — |
| Agent Card | conformant |
| Dry Run Mode | — |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |
| Pagination Ratio | na |
| Operation Distinctiveness | distinct |

**Regulatory alignment 30.4** — Horizontal (data, software, accessibility, platform)

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/assetfare/](https://apis.io/providers/assetfare/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for AssetFare: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/assetfare/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
