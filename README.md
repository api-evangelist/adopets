# Adopets

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

Adopets is an Adoption Management System (AMS) for animal shelters and rescues that streamlines the entire pet adoption process — online and in-person applications, approval and team collaboration workflows, digital kennel cards with QR codes, secure payment processing for adoption fees, licenses, products and donations, daily reporting and dashboards, and post-adoption communication. Backed by Techstars. Adopets exposes an External API (documented as a public Postman collection) that lets partner systems connect staff users and create, retrieve, change, cancel, and refund adoption payment requests and transactions on behalf of an organization, authenticated with an organization API key plus a per-session JWT bearer token.

**Areas:** Pet Adoption · Animal Welfare · Shelters and Rescues · Adoption Management · Payments · Nonprofit Technology · Software-as-a-Service · Company

## Adopets on APIs.io

Everything profiled for Adopets is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/adopets/](https://apis.io/providers/adopets/)** — or go straight to one of the APIs or properties below.

### APIs (3)

- [Adopets Payment Request API](https://apis.io/apis/adopets/adopets-payment-request-api/) — Create and manage adoption payment requests
- [Adopets Payment Transaction API](https://apis.io/apis/adopets/adopets-payment-transaction-api/) — Retrieve and refund payment transactions
- [Adopets System Auth API](https://apis.io/apis/adopets/adopets-system-auth-api/) — Connect/disconnect an external system user and obtain a session token

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### Arazzo workflows (2)

Multi-step workflows that chain operations into a business task.

- [Create and collect an adoption payment (Adopets External API)](https://apis.io/arazzos/adopets/adopets-create-adoption-payment/)
- [Refund an adoption payment transaction (Adopets External API)](https://apis.io/arazzos/adopets/adopets-refund-transaction/)

#### MCP servers (1)

Model Context Protocol servers that expose the API to agents.

- [adopets-external](https://apis.io/servers/adopets/adopets-external/)

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Adopets Agentic Access](https://apis.io/agentic-access/adopets/adopets-agentic-access/)

#### Collections (3)

Postman and Open Collection request collections.

- [Adopets External payment-request API](https://apis.io/collections/adopets/open-adopets-payment-request-api/)
- [Adopets External payment-request payment-transaction API](https://apis.io/collections/adopets/open-adopets-payment-transaction-api/)
- [Adopets External payment-request system-auth API](https://apis.io/collections/adopets/open-adopets-system-auth-api/)

#### Overlays (1)

OpenAPI overlays, including conversational phrasing for each operation.

- [Adopets External Overlay](https://apis.io/overlays/adopets/adopets-external-overlay/)

#### Security (2)

Authentication, trust centre, and vulnerability disclosure.

- [Adopets Authentication](https://apis.io/security/adopets/adopets-authentication/)
- [Adopets Domain Security](https://apis.io/security/adopets/adopets-domain-security/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://adopets.com/)
- [Documentation](https://developers.adopets.com/)
- [API reference](https://developers.adopets.com/)
- [Blog](https://www.adopets.com/blog/)
- [GitHub](https://github.com/adopets)

## API Evangelist rating

**Kin Score 21.0** — emerging · rubric 0.24.0 · scored 2026-10-17

| Facet | Score |
|---|---|
| Discoverability | 71.4 |
| Contract quality | 14.0 |
| Contract governance | 4.5 |
| Operational transparency | 2.6 |
| Developer ergonomics | 54.2 |
| Access clarity | 0.0 |

**Agent readiness 23.1** — agent-aware

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | derived (partial credit) |
| Reversibility Documented | documented (partial credit) |
| MCP Server | — |
| Auth Clarity | bearer (partial credit) |
| Idempotency | — |
| Error Semantics | derived (partial credit) |
| OpenAPI Examples | partial |
| Rate Limit Signal | — |
| Event Surface Described | — |
| Agent Skills | derived (partial credit) |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |

**Regulatory alignment 15.2** — Payments

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/adopets/](https://apis.io/providers/adopets/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Adopets: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/adopets/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
