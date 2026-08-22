# Capital One (capital-one)

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

Capital One is a US money-center bank and financial services company offering credit cards, checking and savings accounts, loans, and auto financing. Through the Capital One DevExchange developer program, the bank publishes a catalog of partner-facing production APIs for account lookup, transaction authorizations, credit offers, customer transactions, credit card applications, auto financing, proactive prescreen, partner account summary, shop with rewards, and public key sharing for client authentication. Access is secured with OAuth 2.0 and a public sandbox supports pre-production integration, with production access gated behind partner approval. Developer documentation is HTML-only (the portal is a single-page app) and no downloadable OpenAPI specs are published. As an FDX member, Capital One also supports consumer-permissioned open-finance data access via aggregators (Plaid, Akoya, Finicity) in the US voluntary open-banking context.

**URL:** [Visit APIs.json URL](https://raw.githubusercontent.com/api-evangelist/capital-one/refs/heads/main/apis.yml)

## Scope

- **Type:** Index
- **x-type:** company
- **Position:** Consumer
- **Access:** 3rd-Party

## Tags

- Auto Finance
- Authorizations
- Banking
- Credit Cards
- Credit Offers
- DevExchange
- Financial Services
- OAuth 2.0
- Payments
- Rewards

## Features

- Broad public developer program (DevExchange) across consumer banking capabilities
- OAuth 2.0-based authentication and authorization
- Sandbox environment for pre-production testing
- Public key sharing for client authentication and data protection
- Coverage across account lookup, authorizations, credit offers, and transactions
- Credit card application flows at point-of-sale and pre-application orchestration
- Real-time proactive prescreen and enhanced decisioning data
- Rewards and Shop with Rewards integration for merchants

## Use Cases

- Partner and fintech integration with Capital One consumer banking
- Credit card application embedding at point-of-sale and online checkout
- Personalized credit offers and prescreen underwriting
- Reward-powered shopping and commerce experiences
- Auto financing application and approval flows
- Consumer-permissioned account summary for partner dashboards
- Real-time transaction authorization for merchants and fintechs

## APIs

- **Capital One Account Lookup API** — Account details, balances, and transaction history for lookup scenarios.
- **Capital One Authorizations API** — Real-time validation and authorization of financial transactions.
- **Capital One Credit Offers API** — Programmatic access to Capital One credit card offers, rates, and eligibility.
- **Capital One Customer Transactions** — Customer transaction processing and reconciliation.
- **Capital One Data Protection and Client Authentication Public Key Sharing API** — Public key exchange for encrypted client-server communication.
- **Capital One Digital Auto Financing Credit Application API** — Digital auto loan application and approval flow.
- **Capital One Enhanced Decisioning Data API** — Decisioning data with analytics and ML signals for risk, fraud, and customer insight.
- **Capital One In-Store Credit Card Payments API** — Credit card payment acceptance integrated with merchant POS.
- **Capital One POS Credit Card Application API** — Credit card application at the point-of-sale counter.
- **Capital One Partner Account Summary API** — Real-time account summary, balances, and pending transactions for partners.
- **Capital One Pre-Application Orchestrator API** — Orchestrates data gathering, credit checks, and eligibility for product applications.
- **Capital One Real-Time Proactive Prescreen API** — Real-time creditworthiness prescreen for targeted offers.
- **Capital One Retrieve Consumer Bank Products API** — Access consumer credit card, checking, and savings product details.
- **Capital One Shop with Rewards API** — Integration for reward redemption in online shopping experiences.

## Common Properties

- [Portal](https://developer.capitalone.com/)
- [Getting Started](https://developer.capitalone.com/documentation/getting-started)
- [OAuth 2.0](https://developer.capitalone.com/documentation/o-auth)
- [Sandbox](https://developer.capitalone.com/documentation/sandbox)
- [FAQ](https://developer.capitalone.com/help/faq)
- [Support](https://developer.capitalone.com/help/tickets)
- [GitHub Organization](https://github.com/capitalone)

## Timestamps

- **Created:** 2024-11-15
- **Modified:** 2026-04-23

## Maintainers

**FN:** Kin Lane
**Email:** info@apievangelist.com
