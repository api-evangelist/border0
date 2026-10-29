# Border0

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

Border0 is an identity-aware Zero Trust network access platform for securing access to infrastructure — SSH and RDP servers, PostgreSQL/MySQL/MSSQL/MongoDB/Elasticsearch databases, Kubernetes clusters, AWS consoles and S3 buckets, and any internal HTTP or TCP service. Instead of VPNs and shared credentials, Border0 publishes each resource as a policy-gated "socket," authenticates users through their existing SSO/identity provider, and records every session for audit. Its REST admin API (api.border0.com/api/v1) manages sockets, access policies, connectors, organizations, identity providers, service accounts, tokens, sessions, and audit logs, and is complemented by an official Go SDK, a Terraform provider, a CLI, and GitHub Actions. Border0 was acquired by Tailscale in March 2026.

**Areas:** Zero Trust · Network Access · Security · Identity and Access Management · Infrastructure · VPN · SSH · Database · Kubernetes · Company

## Border0 on APIs.io

Everything profiled for Border0 is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/border0/](https://apis.io/providers/border0/)** — or go straight to one of the APIs or properties below.

### APIs (15)

- [Border0 Audit Actions API](https://apis.io/apis/border0/border0-audit-actions-api/) — The Audit Actions API from Border0 — 2 operation(s) for audit actions.
- [Border0 Client API](https://apis.io/apis/border0/border0-client-api/) — The Client API from Border0 — 6 operation(s) for client.
- [Border0 Connect API](https://apis.io/apis/border0/border0-connect-api/) — The Connect API from Border0 — 1 operation(s) for connect.
- [Border0 Login API](https://apis.io/apis/border0/border0-login-api/) — The Login API from Border0 — 2 operation(s) for login.
- [Border0 Mtls-Ca API](https://apis.io/apis/border0/border0-mtls-ca-api/) — The Mtls-Ca API from Border0 — 3 operation(s) for mtls-ca.
- [Border0 Organization API](https://apis.io/apis/border0/border0-organization-api/) — The Organization API from Border0 — 4 operation(s) for organization.
- [Border0 Organizations API](https://apis.io/apis/border0/border0-organizations-api/) — The Organizations API from Border0 — 15 operation(s) for organizations.
- [Border0 Policies API](https://apis.io/apis/border0/border0-policies-api/) — The Policies API from Border0 — 2 operation(s) for policies.
- [Border0 Policy API](https://apis.io/apis/border0/border0-policy-api/) — The Policy API from Border0 — 1 operation(s) for policy.
- [Border0 Session API](https://apis.io/apis/border0/border0-session-api/) — The Session API from Border0 — 3 operation(s) for session.
- [Border0 Sessions API](https://apis.io/apis/border0/border0-sessions-api/) — The Sessions API from Border0 — 2 operation(s) for sessions.
- [Border0 Socket API](https://apis.io/apis/border0/border0-socket-api/) — The Socket API from Border0 — 10 operation(s) for socket.
- [Border0 Stats API](https://apis.io/apis/border0/border0-stats-api/) — The Stats API from Border0 — 2 operation(s) for stats.
- [Border0 User API](https://apis.io/apis/border0/border0-user-api/) — The User API from Border0 — 4 operation(s) for user.
- [Border0 Users API](https://apis.io/apis/border0/border0-users-api/) — The Users API from Border0 — 5 operation(s) for users.

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### MCP servers (1)

Model Context Protocol servers that expose the API to agents.

- [border0](https://apis.io/servers/border0/border0/)

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Border0 Agentic Access](https://apis.io/agentic-access/border0/border0-agentic-access/)

#### Collections (15)

Postman and Open Collection request collections.

- [Border0 Audit Actions API](https://apis.io/collections/border0/open-border0-audit-actions-api/)
- [Border0 Audit Actions Client API](https://apis.io/collections/border0/open-border0-client-api/)
- [Border0 Audit Actions Connect API](https://apis.io/collections/border0/open-border0-connect-api/)
- [Border0 Audit Actions Login API](https://apis.io/collections/border0/open-border0-login-api/)
- [Border0 Audit Actions Mtls-Ca API](https://apis.io/collections/border0/open-border0-mtls-ca-api/)
- [Border0 Audit Actions Organization API](https://apis.io/collections/border0/open-border0-organization-api/)
- [Border0 Audit Actions Organizations API](https://apis.io/collections/border0/open-border0-organizations-api/)
- [Border0 Audit Actions Policies API](https://apis.io/collections/border0/open-border0-policies-api/)
- [Border0 Audit Actions Policy API](https://apis.io/collections/border0/open-border0-policy-api/)
- [Border0 Audit Actions Session API](https://apis.io/collections/border0/open-border0-session-api/)
- [Border0 Audit Actions Sessions API](https://apis.io/collections/border0/open-border0-sessions-api/)
- [Border0 Audit Actions Socket API](https://apis.io/collections/border0/open-border0-socket-api/)
- [Border0 Audit Actions Stats API](https://apis.io/collections/border0/open-border0-stats-api/)
- [Border0 Audit Actions User API](https://apis.io/collections/border0/open-border0-user-api/)
- [Border0 Audit Actions Users API](https://apis.io/collections/border0/open-border0-users-api/)

#### Overlays (1)

OpenAPI overlays, including conversational phrasing for each operation.

- [Border0 Openapi Overlay](https://apis.io/overlays/border0/border0-openapi-overlay/)

#### Security (3)

Authentication, trust centre, and vulnerability disclosure.

- [Border0 Authentication](https://apis.io/security/border0/border0-authentication/)
- [Border0 Domain Security](https://apis.io/security/border0/border0-domain-security/)
- [Border0 Vulnerability Disclosure](https://apis.io/security/border0/border0-vulnerability-disclosure/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://www.border0.com)
- [Documentation](https://docs.border0.com)
- [Getting started](https://docs.border0.com/docs/quick-start-copy)
- [API reference](https://docs.border0.com/reference)
- [Sign up](https://portal.border0.com/register)
- [Support](https://docs.border0.com/docs/getting-help)
- [Blog](https://www.border0.com/blog)
- [Security](https://docs.border0.com/docs/security-policy)
- [Terms of service](https://www.border0.com/terms-of-service)
- [Privacy policy](https://www.border0.com/privacy-policy)
- [GitHub](https://github.com/borderzero)
- [Status](https://status.border0.com)

## API Evangelist rating

**Kin Score 46.0** — developing · rubric 0.25.0 · scored 2026-10-23

| Facet | Score |
|---|---|
| Discoverability | 73.2 |
| Contract quality | 49.4 |
| Contract governance | 4.5 |
| Operational transparency | 39.5 |
| Developer ergonomics | 47.0 |
| Access clarity | 34.2 |

**Agent readiness 23.6** — agent-aware

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | derived (partial credit) |
| Reversibility Documented | — |
| MCP Server | — |
| Auth Clarity | bearer (partial credit) |
| Idempotency | — |
| Error Semantics | verified |
| OpenAPI Examples | — |
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
| Pagination Ratio | — |
| Operation Distinctiveness | mostly |

**Regulatory alignment 30.4** — Horizontal (data, software, accessibility, platform)

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/border0/](https://apis.io/providers/border0/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Border0: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/border0/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
