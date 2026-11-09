# Awesome-Subscription-Recurring-Billing

# Awesome Subscription & Recurring Billing

> A curated list of top Subscription and Recurring Billing platforms — both SaaS/Hosted commercial solutions and open-source alternatives for managing plans, invoices, payments, and revenue.
> 🌟 Star this repo if you find it useful! 🌟

---

## 📋 Table of Contents

- [SaaS / Hosted Platforms](#-saas--hosted-platforms)
  - [Stripe Billing](#stripe-billing)
  - [Chargebee](#chargebee)
  - [Zuora](#zuora)
  - [Recurly](#recurly)
  - [Paddle](#paddle)
  - [Maxio](#maxio)
  - [Orb](#orb)
  - [Metronome](#metronome)
- [Open-Source Software](#-open-source-software)
  - [Lago](#lago)
  - [Kill Bill](#kill-bill)
  - [Zentla](#zentla)
  - [Meteroid](#meteroid)
  - [UniBee](#unibee)
  - [Invoice Ninja](#invoice-ninja)
- [Comparison at a Glance](#-comparison-at-a-glance)
- [Contributing](#-contributing)

---

## 🟦 SaaS / Hosted Platforms

Commercial, cloud-hosted Subscription and Recurring Billing platforms. These are not open-source but are included as reference points for feature comparison.

### Stripe Billing
**Type:** Billing layer on top of Stripe payments  
Stripe Billing is the lowest-friction option for teams already processing payments through Stripe: no new gateway, no new reconciliation surface, and one vendor for both payments and billing [citation:14]. It handles subscriptions, simple metered models, and invoicing, with excellent developer documentation. **Trade-off:** You remain the merchant of record and own global tax compliance end to end; complex usage models often require custom engineering on top, and fees stack across processing, billing, and tax tooling [citation:14].

### Chargebee
**Type:** Mature subscription management with usage add-ons  
Chargebee is a mature subscription management platform that extended into usage-based billing. If your pricing is a base subscription with metered overages, it handles upgrades, proration, dunning, and revenue reporting well [citation:14]. Its emphasis is inverted compared to usage-first platforms: subscription logic is the core and usage layers on top. **Trade-off:** Metering is not the architectural core, so extreme event volumes fit poorly, and costs stack once you add a gateway and tax provider [citation:14].

### Zuora
**Type:** Enterprise monetization and revenue recognition  
Zuora is the enterprise standard for subscription billing with strong revenue recognition (RevPro) capabilities. It is suited for complex, global monetization models where finance and compliance requirements are as important as the billing mechanics. Pricing is quote-based and typically targets mid-to-large enterprises.

### Recurly
**Type:** Subscription billing with revenue recovery focus  
Recurly provides subscription management with a strong emphasis on dunning and revenue recovery. It is often compared alongside Chargebee for mid-market SaaS, with strengths in automated payment retries and churn reduction. Pricing is tiered by revenue volume.

### Paddle
**Type:** Merchant of Record for SaaS  
Paddle acts as a merchant of record, handling payment processing, tax compliance, and subscription billing on your behalf. This removes the burden of global tax registration and remittance, making it attractive for indie SaaS and small teams selling internationally. Pricing is a percentage of revenue.

### Maxio
**Type:** Billing and financial operations for B2B SaaS  
Maxio combines subscription billing with financial operations, targeting B2B SaaS companies with complex contracts, usage, and revenue recognition needs. It emerged from the merger of SaaSOptics and Chargify.

### Orb
**Type:** Usage-based billing for API and AI products  
Orb provides usage-based pricing, metering, and invoicing for API and cloud products, with a focus on developer-friendly configuration and high-volume event ingestion. It is often compared to Metronome and Lago for modern usage-based models.

### Metronome
**Type:** High-volume usage billing (acquired by Stripe)  
Metronome is a usage-based billing platform for high-volume consumption pricing, acquired by Stripe [citation:14]. It is suited for large-scale metering and rating, particularly for teams already standardized on the Stripe ecosystem. **Trade-off:** Enterprise-only pricing with no published figures, and roadmap direction is now tied to Stripe, which matters if vendor independence drove your original evaluation [citation:14].

---

## 🟩 Open-Source Software

Self-hosted, community-driven Subscription and Recurring Billing tools. The open-source ecosystem has matured significantly, led by Lago and Kill Bill, with newer entrants targeting modern SaaS monetization.

### Lago
**Stack:** Ruby / PostgreSQL / Redis / ClickHouse | **License:** AGPL-3.0  
Lago is the most established open-source billing engine for usage-based, subscription, and hybrid pricing, explicitly positioned as an alternative to Chargebee, Recurly, and Stripe Billing [citation:4][citation:15]. It provides event-based usage metering, flexible price plans (pay-as-you-go and hybrid), coupons, add-ons, prepaid credits, and automated invoicing with PDF generation [citation:4]. Lago does not process payments itself—it calculates charges and pushes invoices to Stripe, Adyen, or GoCardless for collection [citation:9]. It has the largest community among open-source billing tools (11k+ stars) and scores highest on maintenance health (96/100) [citation:7]. **Trade-off:** AGPL licensing requires publishing changes if you distribute a modified version, and you own the operational burden of running the full stack (API, worker, PDF renderer, Postgres, Redis) [citation:7][citation:9].  
**Best for:** Teams wanting a proven, feature-rich open-source billing engine with genuine usage metering and hybrid pricing, accepting the operational overhead and AGPL obligations.

### Kill Bill
**Stack:** Java / PostgreSQL/MySQL | **License:** Apache-2.0  
Kill Bill is the closest like-for-like alternative to Lago's self-hosted model, with a long-running community and a plugin-oriented architecture that allows deep customization [citation:14]. It provides subscription billing and payments with real-time analytics and financial reports [citation:7]. **Trade-off:** Every operational cost applies in full with no vendor to escalate to, and capability depth depends on which plugins you adopt and maintain [citation:14].  
**Best for:** Teams with a strong platform function that have already decided to own billing operations and want a permissively licensed (Apache-2.0) alternative to AGPL.

### Zentla
**Stack:** Node.js / PostgreSQL / Redis | **License:** Open Source (per project)  
Zentla is a newer open-source monetization layer for SaaS that combines entitlements, usage metering, multi-provider billing (Stripe and Zuora), and revenue analytics in one API [citation:3]. It is designed to solve the "provider lock-in" problem by letting you switch payment providers without code changes. Features include feature gating, real-time usage summaries, pricing experiments, and enterprise-ready audit logging [citation:3]. **Trade-off:** It is a younger project than Lago or Kill Bill, and the community and ecosystem are still developing.  
**Best for:** Teams wanting an open-source billing layer that is explicitly provider-agnostic and includes entitlements and revenue analytics alongside billing.

### Meteroid
**Stack:** Rust / PostgreSQL / ClickHouse / Kafka | **License:** Open Source (per project)  
Meteroid is an open-source billing and subscription management platform built in Rust for high performance, positioned as a self-hosted alternative to Stripe Billing, Chargebee, and Zuora [citation:10]. It supports subscription billing, usage-based pricing, hybrid models, invoicing with tax compliance, coupons, trials, and revenue analytics. The architecture is API-first and designed to process millions of usage events for real-time metering [citation:10]. **Trade-off:** The full stack requires PostgreSQL, ClickHouse, and Kafka, making it heavier to operate than Lago or Kill Bill.  
**Best for:** Performance-sensitive teams wanting a Rust-based billing platform with high-volume event processing and a modern API-first design.

### UniBee
**Stack:** Go / MySQL / Redis | **License:** Open Source (per project)  
UniBee is an open-source, gateway-agnostic subscription billing platform that handles recurring payments, subscription lifecycle, automated invoicing, dunning recovery, usage-based billing, and global tax automation [citation:11]. It is explicitly positioned as a self-hosted alternative to Recurly, Chargebee, and Paddle, with the key differentiator of connecting multiple payment gateways (Stripe, PayPal, local methods) simultaneously without vendor lock-in [citation:11]. **Trade-off:** It is newer than Lago and Kill Bill, with a smaller community and less extensive documentation.  
**Best for:** Teams wanting a gateway-agnostic billing platform with dunning and tax automation, particularly those needing to support multiple payment providers.

### Invoice Ninja
**Stack:** PHP / Laravel / MySQL | **License:** Elastic-2.0 (source-available)  
Invoice Ninja is a powerful invoicing and billing tool that also handles subscriptions and recurring billing, with a health score of 96/100 and a very active codebase (475 commits in 90 days) [citation:7]. **Important caveat:** It is source-available under the Elastic License 2.0, not OSI-approved open source, which limits commercial reuse and redistribution [citation:7].  
**Best for:** Teams primarily needing invoicing with basic recurring billing, accepting the source-available licensing terms.

---

## 📊 Comparison at a Glance

| Software | License | Stack | Usage Metering | Payment Processing | Self-Hosted | Best For |
|----------|---------|-------|----------------|---------------------|-------------|----------|
| **Stripe Billing** | Proprietary | Cloud | ✅ (Simple) | ✅ (Stripe) | ❌ | Stripe-native teams |
| **Chargebee** | Proprietary | Cloud | ✅ (Add-on) | Via gateway | ❌ | Subscription-first + overages |
| **Zuora** | Proprietary | Cloud | ✅ | Via gateway | ❌ | Enterprise revenue recognition |
| **Paddle** | Proprietary | Cloud | (Check) | ✅ (MoR) | ❌ | Global SaaS tax handling |
| **Lago** | AGPL-3.0 | Ruby/Postgres | ✅ Deep | Via gateway | ✅ | Proven open-source billing |
| **Kill Bill** | Apache-2.0 | Java | (Plugins) | Via plugins | ✅ | Permissive OSS billing |
| **Zentla** | Open Source | Node.js/Postgres | ✅ | Multi-provider | ✅ | Provider-agnostic + entitlements |
| **Meteroid** | Open Source | Rust/ClickHouse | ✅ High-volume | (Check) | ✅ | High-performance usage billing |
| **UniBee** | Open Source | Go/MySQL | ✅ | Multi-gateway | ✅ | Gateway-agnostic + dunning |
| **Invoice Ninja** | Elastic-2.0 | PHP/MySQL | (Limited) | Via gateway | ✅ | Invoicing + basic recurring |

---

## 🤝 Contributing

Contributions are welcome! If you know of an open-source Subscription or Recurring Billing tool that should be listed here, please open a pull request with:

- Project name and URL
- Brief description (1–2 sentences)
- Stack and license
- Why it stands out

Please ensure the project is actively maintained (releases within the last 12 months) and genuinely open-source (or clearly note if it is source-available but not OSI-approved, as with Invoice Ninja). Note that the open-source ecosystem is led by **Lago** (most established, 11k+ stars, health 96/100) and **Kill Bill** (Apache-2.0, long-running community). Newer entrants like **Zentla**, **Meteroid**, and **UniBee** are targeting specific gaps: provider-agnostic billing, high-performance event processing, and multi-gateway support respectively. For teams with hard data residency or regulatory requirements, Lago and Kill Bill remain the most battle-tested self-hosted options [citation:14].

---

## 📄 License

This list is released under CC0 1.0 Universal (Public Domain). The software projects listed retain their respective licenses.

---

⭐ **If this list helped you discover a useful tool, please star the repo!** ⭐
