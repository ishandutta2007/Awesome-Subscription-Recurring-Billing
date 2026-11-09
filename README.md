<div align="center">

<img src="./assets/banner.svg" alt="Awesome Subscription &amp; Recurring Billing Banner" width="100%" />

# 💳 Awesome Subscription &amp; Recurring Billing 🚀

<a href="https://github.com/ishandutta2007/Awesome-Awesome-Awesome"><img src="https://img.shields.io/badge/Awesome-%E2%9C%94-blueviolet?style=flat-square&logo=github" alt="Awesome"/></a>
<a href="https://discord.gg/jc4xtF58Ve"><img src="https://img.shields.io/badge/Discord-5865F2?style=for-the-badge&logo=discord&logoColor=white" alt="Discord" /></a>
[![Awesome](https://awesome.re/badge.svg)](https://github.com/ishandutta2007/Awesome-Awesome-Awesome)
[![License: CC0-1.0](https://img.shields.io/badge/License-CC0_1.0-lightgrey.svg)](LICENSE)
[![GitHub_Stars](https://img.shields.io/github/stars/ishandutta2007/Awesome-Subscription-Recurring-Billing?style=social)](https://github.com/ishandutta2007/Awesome-Subscription-Recurring-Billing/stargazers)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](#-contributing)
<a href="https://github.com/ishandutta2007"><img alt="GitHub followers" src="https://img.shields.io/github/followers/ishandutta2007?label=Follow" /></a>

<p align="center">
  <b>✨ A curated directory of top Subscription Billing platforms, Recurring Payment engines, Usage-Based Metering tools, and Invoicing software. ✨</b>
  <br />
  <i>🔥 From battle-tested cloud SaaS providers to self-hosted, developer-first open-source engines for managing plans, invoices, taxes, and revenue recognition. ⚡</i>
</p>

[📈 Sector Overview](#-sector-overview--market-dynamics) • [🟦 SaaS Platforms](#-saas--hosted-platforms) • [🟩 Open-Source Software](#-open-source-software) • [📊 Comparison Matrix](#-comparison-at-a-glance) • [⭐ Star History](#-star-history) • [🤝 Contributing](#-contributing)

</div>

---

## 📋 Table of Contents

- [📈 Sector Overview & Market Dynamics](#-sector-overview--market-dynamics)
- [🟦 SaaS / Hosted Platforms](#-saas--hosted-platforms)
- [🟩 Open-Source Software (Ranked by Stars)](#-open-source-software)
  - [1. Lago](#1-lago-)
  - [2. Invoice Ninja](#2-invoice-ninja-)
  - [3. Polar](#3-polar-)
  - [4. Crater](#4-crater-)
  - [5. FlexPrice](#5-flexprice-)
  - [6. Kill Bill](#6-kill-bill-)
  - [7. InvoicePlane](#7-invoiceplane-)
  - [8. OpenMeter](#8-openmeter-)
  - [9. Meteroid](#9-meteroid-)
  - [10. Tier](#10-tier-)
  - [11. UniBee](#11-unibee-)
  - [12. Zentla](#12-zentla-)
- [📊 Comparison at a Glance](#-comparison-at-a-glance)
- [⭐ Star History](#-star-history)
- [🤝 Contributing](#-contributing)
- [☕ Support](#-support)
- [📄 License](#-license)

---

## 📈 Sector Overview & Market Dynamics

The global subscription and billing management market is estimated at **$7.5 billion – $8.5 billion in 2024–2025** and is projected to expand to **$18 billion – $20+ billion by 2030–2031**, driven by a compound annual growth rate (CAGR) of approximately 16.5%–17% as global businesses accelerate transitions toward hybrid subscription and usage-based pricing models.

The sector exhibits **moderate concentration at the enterprise tier** alongside **high fragmentation across the middle and lower tiers**:
- **Enterprise Concentration:** Tier-1 fintech infrastructure giants and legacy enterprise software suites (e.g., Stripe, Oracle, SAP, Salesforce, and Zuora) capture over 40%–45% of total high-volume and multi-entity enterprise billing volume.
- **Mid-Market & Developer Fragmentation:** The remaining market is intensely fragmented among specialized pure-play platforms, Merchant of Record (MoR) providers (e.g., Paddle), and high-growth API-first consumption-metering platforms (e.g., Metronome, Orb). Simultaneously, open-source and self-hosted billing engines (e.g., Lago, Polar, Kill Bill, FlexPrice) have surged to deliver data sovereignty, avoid vendor lock-in, and eliminate transaction tax overhead for engineering-led teams.

---

## 🟦 SaaS / Hosted Platforms

Commercial, cloud-hosted Subscription and Recurring Billing platforms. Products are sorted in **descending order by company scale** (estimated valuation or annual revenue run-rate).

| Platform | Company Scale (Valuation / Revenue) | Starting Pricing (Specific Tier) | Free Tier / Trial Limit | Key Focus & Monetization Archetype |
|:---|:---|:---|:---|:---|
| **[Stripe Billing](https://stripe.com/billing)** | **$70 Billion Valuation** (~$14B+ total processing revenue) | **0.7%** of recurring billing volume (standard domestic processing: 2.9% + 30¢) | **No free tier limit** (0.7% fee applies from dollar one; pay-as-you-go with no setup fee) | Native billing layer on Stripe payment gateway; ideal for Stripe-standardized SaaS |
| **[Zuora](https://www.zuora.com)** | **$1.7 Billion Valuation** ($450M annual revenue; acquired by Silver Lake/GIC) | **Quote-based annual contract** (Starting tiers typically ~$50,000–$75,000/yr) | **No permanent free tier** (Evaluation sandboxes available only via enterprise sales qualification) | Enterprise subscription relationship management, complex CPQ, and ASC 606 revenue recognition (RevPro) |
| **[Paddle](https://www.paddle.com)** | **$1.4 Billion Valuation** (Series D unicorn backed by KKR) | **5% + $0.50** per successful transaction | **Pay-as-you-go with $0 fees** until first paid checkout (handles cardless and card-required trials for end-users) | Complete Merchant of Record (MoR); absorbs global VAT/sales tax registration, filing, and fraud liability |
| **[Chargebee](https://www.chargebee.com)** | **$1.4 Billion Valuation** (Series F unicorn backed by Insight Partners) | **$0/month** until $250k lifetime billing; then **0.75% overage** (Performance plan starts at **$599/month**) | **$250,000 cumulative lifetime billing** on Starter plan (up to 50,000 API calls/month) | Mature subscription management engine with automated dunning and gateway orchestration |
| **[Recurly](https://recurly.com)** | **~$500 Million+ Est. Valuation** (Majority acquisition by Accel-KKR) | **$249/month + 0.9%** on overages above included threshold | **90-day free trial** of Starter plan (includes first **$40,000/month** billing volume without extra percentage fee) | Advanced dunning recovery, churn prevention algorithms, and subscriber lifecycle management |
| **[Maxio](https://www.maxio.com)** | **~$300 Million–$400 Million Est. Valuation** (Backed by Vista Equity Partners) | **$599/month** (Grow plan for teams up to $100k monthly billings) | **30-day developer sandbox trial** ("Build" tier: $0 for dummy gateway testing; no live production billing) | B2B SaaS financial operations, complex contract billing, SaaS metrics reporting, and deferred revenue |
| **[Orb](https://www.withorb.com)** | **~$110 Million–$250 Million Valuation** ($44.1M raised; acquired by Adyen) | **Quote-based base tier** (Estimated entry deployments start at **~$720/month** base platform fee) | **No self-serve free tier** (Requires sales consultation for sandbox onboarding and custom event ingestion proof-of-concept) | Developer-first usage-based pricing, high-throughput event ingestion, and real-time metering for AI & cloud APIs |
| **[Metronome](https://metronome.com)** | **High-Growth Scale** (Acquired by Stripe; $78M+ raised prior) | **0.8% of billing volume + $0.04 per 1,000 ingested events** (Starter tier; no baseline platform monthly subscription) | **No fixed platform fee entry point** (Pay purely per-event and per-dollar processed; sandbox testing access upon developer sign-up) | High-volume consumption and token-based billing for infrastructure, LLM providers, and data platforms |

---

## 🟩 Open-Source Software

Self-hosted, community-driven Subscription, Invoicing, and Recurring Billing platforms. Sorted in **descending order by GitHub Stars_Count**.

### 1. Lago 🌊
[![Lago Stars](https://img.shields.io/github/stars/getlago/lago?style=social&color=white)](https://github.com/getlago/lago/stargazers)

- **Repository:** [getlago/lago](https://github.com/getlago/lago)
- **License:** AGPL-3.0
- **Stack:** Ruby / PostgreSQL / Redis / ClickHouse
- **Key Capabilities:** Lago is the leading open-source billing engine designed specifically for usage-based, subscription, and hybrid pricing models. It acts as an API-first metering layer that calculates complex charges, tracks consumption events, manages prepaid credits, generates invoices, and dispatches collection triggers to payment gateways like Stripe, Adyen, and GoCardless.
- **Best For:** High-growth developer teams seeking a self-hosted alternative to Chargebee and Stripe Billing with native support for real-time usage event ingestion.

### 2. Invoice Ninja 🥷
[![Invoice Ninja Stars](https://img.shields.io/github/stars/invoiceninja/invoiceninja?style=social&color=white)](https://github.com/invoiceninja/invoiceninja/stargazers)

- **Repository:** [invoiceninja/invoiceninja](https://github.com/invoiceninja/invoiceninja)
- **License:** Elastic License 2.0 (Source-Available)
- **Stack:** PHP / Laravel / Flutter / MySQL
- **Key Capabilities:** Comprehensive invoicing and payment orchestration platform supporting recurring billing schedules, client portals, quotation workflows, project time-tracking, and integration with 30+ payment gateways.
- **Best For:** Freelancers, agencies, and small businesses needing an end-to-end self-hosted invoice and recurring payment suite.

### 3. Polar ❄️
[![Polar Stars](https://img.shields.io/github/stars/polarsource/polar?style=social&color=white)](https://github.com/polarsource/polar/stargazers)

- **Repository:** [polarsource/polar](https://github.com/polarsource/polar)
- **License:** Apache-2.0
- **Stack:** Python (FastAPI) / Next.js / PostgreSQL / Redis
- **Key Capabilities:** An open-source monetization platform built for modern software and digital products. Polar supports subscription tiers, pay-what-you-want pricing, license key generation, GitHub issue funding, and automated Merchant of Record capabilities.
- **Best For:** Open-source creators, indie hackers, and SaaS founders selling digital downloads, subscriptions, and API access.

### 4. Crater 🧾
[![Crater Stars](https://img.shields.io/github/stars/crater-invoice-inc/crater?style=social&color=white)](https://github.com/crater-invoice-inc/crater/stargazers)

- **Repository:** [crater-invoice-inc/crater](https://github.com/crater-invoice-inc/crater)
- **License:** GPL-3.0
- **Stack:** PHP / Laravel / Vue.js / MySQL
- **Key Capabilities:** Clean, intuitive self-hosted invoicing software with support for automated recurring invoices, detailed expense tracking, multi-currency support, payment gateways, and custom tax rates.
- **Best For:** Small business owners and service agencies desiring a minimalist, beautiful recurring invoice solution.

### 5. FlexPrice ⚡
[![FlexPrice Stars](https://img.shields.io/github/stars/flexprice/flexprice?style=social&color=white)](https://github.com/flexprice/flexprice/stargazers)

- **Repository:** [flexprice/flexprice](https://github.com/flexprice/flexprice)
- **License:** Apache-2.0
- **Stack:** Go / PostgreSQL / ClickHouse / React
- **Key Capabilities:** Real-time usage-based pricing and billing infrastructure for developers. Features real-time usage event aggregation, no-code pricing plan configuration, prepaid wallets, credit top-ups, and feature entitlements.
- **Best For:** AI and cloud infrastructure products needing high-speed metering and credit deductions without proprietary lock-in.

### 6. Kill Bill 🗡️
[![Kill Bill Stars](https://img.shields.io/github/stars/killbill/killbill?style=social&color=white)](https://github.com/killbill/killbill/stargazers)

- **Repository:** [killbill/killbill](https://github.com/killbill/killbill)
- **License:** Apache-2.0
- **Stack:** Java / PostgreSQL / MySQL / OSGi Plugins
- **Key Capabilities:** Enterprise-grade open-source subscription billing and payments platform. Features a modular OSGi plugin architecture, state-machine subscription lifecycle management, payment gateway routing, and deep international tax integration.
- **Best For:** Large enterprises and platform engineering teams with in-house Java expertise needing full architectural control over billing pipelines.

### 7. InvoicePlane ✈️
[![InvoicePlane Stars](https://img.shields.io/github/stars/InvoicePlane/InvoicePlane?style=social&color=white)](https://github.com/InvoicePlane/InvoicePlane/stargazers)

- **Repository:** [InvoicePlane/InvoicePlane](https://github.com/InvoicePlane/InvoicePlane)
- **License:** MIT
- **Stack:** PHP / CodeIgniter / MySQL
- **Key Capabilities:** Veteran self-hosted invoicing application for managing quotes, client accounts, invoices, and automated recurring payment cycles through PayPal, Stripe, and custom processors.
- **Best For:** Simple self-hosted recurring invoicing without complex microservice orchestration overhead.

### 8. OpenMeter ⏱️
[![OpenMeter Stars](https://img.shields.io/github/stars/openmeterio/openmeter?style=social&color=white)](https://github.com/openmeterio/openmeter/stargazers)

- **Repository:** [openmeterio/openmeter](https://github.com/openmeterio/openmeter)
- **License:** Apache-2.0
- **Stack:** Go / Kafka / ClickHouse / PostgreSQL
- **Key Capabilities:** Cloud-native usage metering infrastructure built for AI, API, and developer tools. Collects and aggregates millions of events per second in real-time, enforcing quotas, calculating consumption metrics, and syncing billing data into Stripe Billing or customer portals.
- **Best For:** High-throughput streaming and AI platforms requiring low-latency token and API call metering.

### 9. Meteroid 🚀
[![Meteroid Stars](https://img.shields.io/github/stars/meteroid-oss/meteroid?style=social&color=white)](https://github.com/meteroid-oss/meteroid/stargazers)

- **Repository:** [meteroid-oss/meteroid](https://github.com/meteroid-oss/meteroid)
- **License:** Apache-2.0
- **Stack:** Rust / PostgreSQL / ClickHouse / Kafka
- **Key Capabilities:** High-performance, Rust-powered billing engine handling subscription management, hybrid usage-based pricing, cost limiting, plan grandfathering, and real-time revenue analytics.
- **Best For:** Performance-sensitive teams seeking memory-efficient, lightning-fast event processing and rating.

### 10. Tier 🎯
[![Tier Stars](https://img.shields.io/github/stars/tierrun/tier?style=social&color=white)](https://github.com/tierrun/tier/stargazers)

- **Repository:** [tierrun/tier](https://github.com/tierrun/tier)
- **License:** BSD-3-Clause
- **Stack:** Go / Stripe API
- **Key Capabilities:** Pricing-as-code SDK and CLI designed to manage SaaS pricing models directly against Stripe. Defines price plans, tiered limits, and usage reporting in a declarative JSON configuration file (`pricing.json`).
- **Best For:** Developers looking to treat SaaS pricing configurations as version-controlled code without managing separate billing databases.

### 11. UniBee 🐝
[![UniBee Stars](https://img.shields.io/github/stars/UniBee-Billing/unibee?style=social&color=white)](https://github.com/UniBee-Billing/unibee/stargazers)

- **Repository:** [UniBee-Billing/unibee](https://github.com/UniBee-Billing/unibee)
- **License:** Apache-2.0
- **Stack:** Go / MySQL / Redis / Vue.js
- **Key Capabilities:** Gateway-agnostic subscription billing and dunning engine. Enables merchants to plug into Stripe, PayPal, and regional payment providers simultaneously with automated invoice recovery, coupon support, and tax calculation.
- **Best For:** Companies targeting emerging markets requiring simultaneous multi-gateway routing and flexible currency support.

### 12. Zentla 🛡️
[![Zentla Stars](https://img.shields.io/github/stars/hexrift/zentla?style=social&color=white)](https://github.com/hexrift/zentla/stargazers)

- **Repository:** [hexrift/zentla](https://github.com/hexrift/zentla)
- **License:** MIT
- **Stack:** Node.js / TypeScript / PostgreSQL / Redis
- **Key Capabilities:** Developer-centric monetization layer decoupling billing providers from SaaS codebases. Combines entitlements, feature gating, usage counters, and multi-provider payment abstractions (Stripe, Zuora) behind a unified SDK.
- **Best For:** Engineering teams looking to avoid vendor lock-in by abstracting entitlement checks and payment processors behind an open-source API.

---

## 📊 Comparison at a Glance

| Software | Delivery | Primary License | Tech Stack | Usage Metering | Built-in Payments | Multi-Gateway | Best Suited For |
|:---|:---|:---|:---|:---|:---|:---|:---|
| **Stripe Billing** | Cloud SaaS | Proprietary | Cloud | ✅ Basic | ✅ Native | ❌ (Stripe only) | Stripe-standardized SaaS |
| **Zuora** | Cloud SaaS | Proprietary | Cloud | ✅ Advanced | Via Gateway | ✅ | Enterprise ASC 606 & CPQ |
| **Paddle** | Cloud SaaS | Proprietary | Cloud | ⚠️ Add-on | ✅ (MoR) | ✅ (MoR managed) | Global VAT & sales tax compliance |
| **Chargebee** | Cloud SaaS | Proprietary | Cloud | ✅ Add-on | Via Gateway | ✅ | Subscription-first & dunning recovery |
| **Recurly** | Cloud SaaS | Proprietary | Cloud | ✅ Add-on | Via Gateway | ✅ | Mid-market churn reduction |
| **Maxio** | Cloud SaaS | Proprietary | Cloud | ✅ Hybrid | Via Gateway | ✅ | B2B SaaS ARR & revenue recognition |
| **Orb** | Cloud SaaS | Proprietary | Cloud | ✅ Deep Real-time | Push to Gateway | ✅ | High-volume API & AI token billing |
| **Metronome** | Cloud SaaS | Proprietary | Cloud | ✅ Deep Streaming | Push to Gateway | ✅ | High-throughput consumption pricing |
| **Lago** | Self-Hosted | AGPL-3.0 | Ruby / Postgres / ClickHouse | ✅ Real-time | Push to Gateway | ✅ | Modern OSS usage & subscription engine |
| **Invoice Ninja** | Self-Hosted | Elastic-2.0 | PHP / Laravel / Flutter | ⚠️ Basic | 30+ Gateways | ✅ | Comprehensive invoicing & quotes |
| **Polar** | Self-Hosted / SaaS | Apache-2.0 | Python / Next.js | ✅ Digital products | Stripe / MoR | ✅ | Developer monetization & digital goods |
| **Crater** | Self-Hosted | GPL-3.0 | PHP / Laravel / Vue | ❌ | Via Gateway | ⚠️ | Minimalist recurring client invoicing |
| **FlexPrice** | Self-Hosted / SaaS | Apache-2.0 | Go / ClickHouse | ✅ High-speed | Push to Gateway | ✅ | Real-time AI metering & credit wallets |
| **Kill Bill** | Self-Hosted | Apache-2.0 | Java / MySQL / Postgres | ✅ Plugins | Plugin-based | ✅ | Enterprise pluggable billing architecture |
| **InvoicePlane** | Self-Hosted | MIT | PHP / MySQL | ❌ | Via Gateway | ⚠️ | Classic client invoicing & payments |
| **OpenMeter** | Self-Hosted / SaaS | Apache-2.0 | Go / Kafka / ClickHouse | ✅ High-scale | Push to Gateway | ✅ | Millions of events/sec AI & API metering |
| **Meteroid** | Self-Hosted | Apache-2.0 | Rust / ClickHouse / Kafka | ✅ High-performance | Push to Gateway | ✅ | High-throughput Rust usage rating |
| **Tier** | Self-Hosted CLI/SDK | BSD-3-Clause | Go | ✅ Stripe-synced | Via Stripe | ❌ (Stripe only) | Declarative pricing-as-code |
| **UniBee** | Self-Hosted | Apache-2.0 | Go / MySQL / Redis | ✅ Standard | Multi-Gateway | ✅ | Gateway-agnostic international billing |
| **Zentla** | Self-Hosted | MIT | Node.js / TypeScript | ✅ Entitlements | Multi-Provider | ✅ | Provider-agnostic entitlement gating |

---

##  Star History
[![Star History Chart](https://www.star-history.com/svg?repos=ishandutta2007/Awesome-Subscription-Recurring-Billing&type=date&legend=top-left)](https://www.star-history.com/#ishandutta2007/Awesome-Subscription-Recurring-Billing&type=date&legend=top-left)

---

## 🤝 Contributing

Contributions are very welcome! If you know of an open-source or notable SaaS Subscription and Recurring Billing platform that should be included:

1. 🍴 Fork this repository.
2. 🌿 Create a feature branch (`git checkout -b feature/add-new-billing-tool`).
3. 💾 Commit your changes with clear descriptions (`git commit -m 'Add tool to open-source section'`).
4. 🚀 Push to your branch (`git push origin feature/add-new-billing-tool`).
5. 📬 Open a Pull Request.

**Submission Guidelines:**
- **Product Name & URL:** Clear link to official repository or landing page.
- **Specific Pricing & Free Tier Limits:** State exact starting numbers rather than generic descriptions.
- **Tech Stack & Open-Source License:** Must specify OSI-approved license (or clarify source-available status).
- **Maintenance Health:** Open-source projects should have had active commits/releases within the past 12 months.

---

## ☕ Support

If you found this curated list insightful or helpful for designing your subscription monetization architecture:

- ⭐ **Star this repository** to help other engineers and founders discover it across GitHub.
- 📢 **Share this resource** with your engineering team, tech communities, and colleagues.
- ☕ **Sponsor the Maintainer:** If this saved you time or aided your tool evaluation, consider supporting ongoing open-source curation on the [GitHub Sponsor Dashboard](https://github.com/sponsors/ishandutta2007).

---

## 📄 License

This repository is dedicated to the public domain under the [Creative Commons Zero v1.0 Universal (CC0 1.0)](LICENSE) dedication. Listed third-party software projects and company trademarks retain their respective copyrights and licenses.

---

<div align="center">
  <sub>Built with ❤️ for developers, founders, and billing architects. Don't forget to ⭐ star this repository!</sub>
</div>
