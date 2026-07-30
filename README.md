# LiquidTrust

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
