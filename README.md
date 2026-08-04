# LiquidTrust

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
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

LiquidTrust, operated by Liquid Global, Inc., is a B2B payments platform that embeds trust and
conditionality directly into the payment flow. Its core product, Micro Escrow(R), holds funds and
releases them against defined conditions such as milestones, approvals, and deliveries, giving buyers
and sellers recourse without a traditional escrow agent. KYC/KYB, AML and sanctions screening are
built into the payment rails, which settle to 200+ countries with J.P. Morgan named as a payment-rails
partner. Pricing is 1% all-in per protected transaction, with a flat $10 Simple Pay option for
lower-risk transfers.

Backed by: Anthemis, Resolute, Motivate, Mucker

## API status

LiquidTrust sells three integration models — referral, white-label, and a direct API integration that
embeds conditional payment logic into a partner platform. **The API is access-gated.** The host
`https://api.liquidtrust.io` is live, but there is no public developer portal, API reference, OpenAPI
description, SDK, CLI, or sandbox; onboarding runs through sales.

What could be observed on the wire: the API exposes `Deprecation` and `Sunset` (RFC 8594), `Link`
(RFC 8288), and W3C Trace Context `traceparent`/`tracestate` headers, over TLS 1.3 with HSTS preload
and a hardened CSP.

## Artifacts

| Artifact | File |
|---|---|
| Conventions | `conventions/liquidtrust-conventions.yml` |
| Lifecycle / status / deprecation | `lifecycle/liquidtrust-lifecycle.yml` |
| Conformance | `conformance/liquidtrust-conformance.yml` |
| Domain security | `security/liquidtrust-domain-security.yml` |
| Vulnerability disclosure | `security/liquidtrust-vulnerability-disclosure.yml` |
| Trust center | `security/liquidtrust-trust-center.yml` |
| Well-known probe record | `well-known/liquidtrust-well-known.yml` |
| llms.txt | `llms/liquidtrust-llms.txt` |

Compliance is genuinely published: SOC 2 Type II (audited annually), ISO 27001, PCI DSS Level 1,
GDPR, and CCPA, with a Vanta-hosted trust center at <https://trust.liquidtrust.io/> and an Instatus
status page at <https://status.liquidtrust.io/>.

Not published by the provider, so deliberately absent here (no fabrication): OpenAPI, AsyncAPI or
webhook catalog, SDKs/packages, CLI, MCP server, agent skills, OAuth scopes, error catalog, decline
codes, sandbox/test data, changelog, embedded components, data model, and `/.well-known/` documents.
