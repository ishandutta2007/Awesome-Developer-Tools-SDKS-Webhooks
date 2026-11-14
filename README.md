# Awesome-Developer-Tools-SDKS-Webhooks

## Top Developer Tools, SDKs & Webhooks Ecosystem

**Curated List of SaaS Platforms & Open-Source GitHub Projects**  
*Focused on API Infrastructure, SDK Generation & Event-Driven Webhook Delivery*  
**Last updated: March 2026**

This repository tracks notable **SaaS platforms** and **open-source projects** for **Developer Tools, SDKs & Webhooks**. These platforms provide the foundational infrastructure for building, testing, and distributing APIs and client libraries—covering API gateways, SDK generators, webhook delivery engines, and developer documentation that reduce integration friction for third-party developers.

**Examples** include Chargebee, Stripe, Twilio, GitHub, Shopify, Plaid, Brex, Square, AWS Developer Tools, and Postman (the category leaders).

**Open-source emphasis**: This section highlights every major active project for self-hosted SDK generation, open-source webhook infrastructure, and community-driven API tooling—ideal for organizations seeking transparency and predictable costs over per-seat or per-event SaaS billing. The open-source landscape is genuinely functional: **Fern** generates SDKs and docs from OpenAPI specs , **OpenAPI Generator** supports 50+ languages , and **Hook0** provides full-feature-parity self-hosted webhook delivery .

Contributions welcome! Open an PR to add/update entries. Keep descriptions factual and link to official sites.

## Table of Contents
- [SaaS/Hosted Platforms](#saas-products)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## SaaS/Hosted Platforms

| Product | Description | Pricing (Starting Tier) | Free Tier / Trial Limits |
|---|---|---|---|
| **[Chargebee](https://www.chargebee.com/)** | Subscription billing platform with **REST API v2** for subscriptions, customers, invoices, payments, and usage metering. HTTP Basic Auth with site-scoped API keys. Ships **SDKs for 7 languages** (Node.js, Python, PHP, Java, Ruby, Go, .NET), webhooks, sandbox/test mode, and an **MCP server** for AI agents. Rate limits: Starter 150 calls/min, Performance 1,000/min, Enterprise 3,500/min. | Starter: **$0/month** (free up to $250K cumulative billing volume, then 0.75% overage fee); Performance: **$599/month** ($7,188/year) | **Free forever (Starter)**: full access up to $250,000 cumulative billing volume; unlimited sandbox/test account |
| **[Stripe](https://stripe.com/)** | Payments platform with **REST API** organized around predictable resource-oriented URLs. **OpenAPI published on GitHub** with frequent releases. **11 first-party SDKs** (Node, Python, Ruby, Go, Java, .NET, PHP, iOS, Android, React Native, React). **200+ signed webhook event types**; delivery is at-least-once and can re-order—handlers must be idempotent. | Standard: **2.9% + $0.30** per successful card charge (no monthly account fee or setup fee) | **Free forever**: 100% free unlimited sandbox/test mode access with test API keys; production charges strictly per transaction |
| **[Twilio](https://www.twilio.com/)** | Communications platform with **1,500+ API endpoints** across SMS, Voice, Video, Email, Verify, and Flex. **AsyncAPI specification** published, SDKs for all major languages, and MCP Server for AI coding agents. | Pay-as-you-go: SMS starts at **$0.0083/message**, Voice starts at **$0.0140/min outbound** ($0.0085/min inbound), local phone numbers from **$1.15/month** | **30-day free trial**: no credit card required; includes product trial units (~100 SMS, 75 voice mins, 3,000 emails) restricted to verified caller IDs and 1 active trial number |
| **[GitHub](https://github.com/features/integrations)** | **REST API** and **GraphQL API** for repositories, issues, pull requests, Actions, and more. **GitHub Apps** with granular API permissions and **built-in webhooks**. **Octokit SDK** for TypeScript/Node.js. OpenAPI specification available for code generation. | Free plan: **$0/month**; Team plan: **$4/user/month** (billed annually) or $4.40/user/month; Enterprise: **$21/user/month** | **Free forever**: unlimited public/private repositories, 5,000 API requests/hour (authenticated), 2,000 GitHub Actions minutes/month |
| **[Shopify](https://shopify.dev/)** | Commerce platform with **GraphQL-First architecture** (Admin API and Storefront API). **Webhooks** for orders/create, inventory_levels/update, refunds/create, plus mandatory compliance webhooks (customers/data_request, customers/redact, shop/redact). Cost-based rate limiting with leaky bucket. | Developer / Partner: **$0/month**; Merchant Starter plan: **$5/month**; Basic plan: **$39/month** | **Free forever (Shopify Partner)**: unlimited development stores with full GraphQL/REST API access and test webhooks; Merchant store offers **3-day free trial** |
| **[Plaid](https://plaid.com/)** | Financial data platform with REST API for bank account linking, transactions, balance, identity, and investments. **Webhooks** for SYNC_UPDATES_AVAILABLE, ITEM: LOGIN_REQUIRED, and ITEM: ERROR with JWT signature verification. Rate limits per-Item per-endpoint. | Sandbox & Development: **$0/month**; Production Pay-as-you-go: Auth starts at **~$1.50 per linked account**, Transactions at **~$0.30/Item/month** | **Free forever**: unlimited Sandbox testing environment + Development environment free for up to **100 live Items** (connected institutions) |
| **[Brex](https://developer.brex.com/)** | Financial spend platform with **Webhooks API** for real-time event notifications, multi-destination webhook subscriptions, token rotation, and staging environment. | Essentials plan: **$0/user/month**; Premium plan: **$12/user/month** | **Free forever (Essentials)**: includes corporate cards, spend tracking, and full Brex REST & Webhooks API access; no credit card required for cardless signup |
| **[Square](https://developer.squareup.com/)** | Payments platform with REST API for payments, catalog, customers, and invoices. Official SDKs and developer dashboard sandbox environment. Charges per processed payment with idempotency key support. | Standard processing: **2.6% + 10¢** (in-person) or **2.9% + 30¢** (online payments); no monthly platform API fee | **Free forever**: unlimited sandbox developer environment with simulated bank/card endpoints; production charges strictly per transaction |
| **[AWS Developer Tools](https://aws.amazon.com/products/developer-tools/)** | Cloud CI/CD and developer suite including CodeBuild, CodePipeline, CodeDeploy, and CodeCommit. | CodeBuild: **$0.005/build minute** (general1.small); CodePipeline: **$1.00/active pipeline/month**; CodeDeploy: **$0.00** for EC2/Lambda/ECS | **Free forever (AWS Free Tier)**: CodeBuild includes **100 build minutes/month** (general1.small); CodePipeline includes **1 free active pipeline/month**; CodeDeploy is free for all AWS cloud compute targets |
| **[Postman](https://www.postman.com/)** | API development, mock server, testing, and collaboration platform with Postman Collections, Monitors, and Postman CLI. | Free plan: **$0/month**; Solo plan: **$9/month** (billed annually); Team plan: **$19/user/month** (billed annually) | **Free forever**: 1 user seat, unlimited local/cloud mock servers, unlimited collection runs, 1,000 API monitoring calls/month, 50 AI credits/month |

## Open-Source GitHub Projects

| Project | Star Badge | Description |
|---------|------------|-------------|
| **[Fern](https://github.com/fern-api/fern)** | [![Stars](https://img.shields.io/github/stars/fern-api/fern?style=social&color=white)](https://github.com/fern-api/fern/stargazers) | **Input OpenAPI. Output SDKs and Docs.** TypeScript-based SDK generator with ~2,947 stars, actively pushed daily . Generates idiomatic SDKs from OpenAPI specs with built-in auth, pagination, retries, and error handling. Stripe uses Fern configurations for their own SDK generation . **Best for teams wanting automated SDK + documentation pipelines from a single spec.** |
| **[Hook0](https://github.com/hook0/hook0)** | [![Stars](https://img.shields.io/github/stars/hook0/hook0?style=social&color=white)](https://github.com/hook0/hook0/stargazers) | **The most complete open-source webhook delivery platform with full-feature-parity self-hosting.** SSPL-1.0 licensed, no closed tier. **Outbound webhooks** with multi-tenant label-based filtering, HMAC signatures, escalating backoff retries, **dead letter queue**, dot-notation event hierarchy, delivery logs and replay, REST API, and **SDKs for 12+ languages**. Authentication via Biscuit tokens + service tokens . |
| **[Outpost (Hookdeck)](https://github.com/hookdeck/outpost)** | [![Stars](https://img.shields.io/github/stars/hookdeck/outpost?style=social&color=white)](https://github.com/hookdeck/outpost/stargazers) | **Production-ready self-hosted outbound webhook and event destinations infrastructure.** Apache-2.0, Go binary/Docker. Supports **Webhooks, Amazon EventBridge, AWS SQS, AWS SNS, GCP Pub/Sub, RabbitMQ, and Kafka** as destinations. At-least-once delivery, event fanout, automatic and manual retries, multi-tenant support, **user portal** (white-label React) for customers to view metrics and debug deliveries, OpenTelemetry traces/metrics/logs, and webhook best practices (idempotency headers, timestamp, signature rotation) opt-out. Ships with MCP server . |
| **[OpenAPI Generator](https://github.com/OpenAPITools/openapi-generator)** | [![Stars](https://img.shields.io/github/stars/OpenAPITools/openapi-generator?style=social&color=white)](https://github.com/OpenAPITools/openapi-generator/stargazers) | **The most widely used open-source SDK generator.** Generates client libraries, server stubs, documentation, and configuration from OpenAPI 2.0/3.x specifications. Supports **50+ languages and frameworks** including Java, Python, TypeScript, Go, Rust, C#, PHP, Ruby, and Swift. Apache 2.0 licensed. The standard tool for organizations building their own SDKs from API specs. |

### Additional Strong Open-Source Options

| Project | Star Badge | Description |
|---------|------------|-------------|
| **[good-webhooks](https://github.com/pplytas/good-webhooks)** | [![Stars](https://img.shields.io/github/stars/pplytas/good-webhooks?style=social&color=white)](https://github.com/pplytas/good-webhooks/stargazers) | **Outbox-pattern webhook library** (MIT). `publish()` joins your database transaction—no separate outbox table. Standard Webhooks signing (HMAC-SHA256), 8 retries over ~28 hours with `Retry-After` on 429/503, automatic pause after 5 days of failures or 410, replay (single delivery or page), PostgreSQL storage. **Library, not a service**—you integrate it into your application . |
| **[Speakeasy](https://github.com/speakeasy-api/speakeasy)** | [![Stars](https://img.shields.io/github/stars/speakeasy-api/speakeasy?style=social&color=white)](https://github.com/speakeasy-api/speakeasy/stargazers) | Open-source SDK generator focused on developer experience. Generates idiomatic, type-safe SDKs from OpenAPI specs with built-in auth, pagination, retries, and error handling. CLI and GitHub Actions integration for CI/CD SDK generation. |

**Frameworks for building custom systems**: Combine **Fern** or **OpenAPI Generator** for SDK generation from your API specs, **Hook0** or **Outpost** for webhook delivery infrastructure, and **good-webhooks** for an outbox-pattern library if you want to own delivery logic in your application—creating a fully open-source developer platform stack without per-seat or per-event SaaS fees.

## How to Contribute

1. Fork the repo.
2. Add/edit entries in `README.md` (follow existing format).
3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.
4. Submit PR with a short explanation.

Star the repo if you find it useful!

## Disclaimer

- This is a **community-curated** list — not exhaustive and not an endorsement.
- Developer platforms handle API credentials and potentially sensitive application data; enforce least-privilege scopes, token rotation, and audit logging.
- **Webhook delivery is at-least-once, not exactly-once.** Stripe explicitly states delivery can re-order and replay—handlers **must be idempotent** . Shopify mandates **three compliance webhooks** (data request, customer redact, shop redact) in addition to business events . Plaid requires **JWT signature verification** on every webhook . **Open-source webhook infrastructure is genuinely viable**: Hook0 offers full-feature-parity self-hosting with no closed tier , Outpost provides production-ready delivery to multiple destination types , and good-webhooks offers an outbox-pattern library for teams wanting to own delivery logic . **SDK generation is also mature**: Fern powers Stripe's own SDK pipeline , and OpenAPI Generator supports 50+ languages . Validate licensing compatibility (Hook0 is SSPL-1.0, Outpost is Apache-2.0) with your organization's policies before committing.

---

**Made for API engineers, platform teams, and developers building developer-facing infrastructure.**  
Let's make developer tools, SDKs, and webhooks more open, reliable, and developer-friendly.
