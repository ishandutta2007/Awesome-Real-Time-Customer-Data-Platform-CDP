# Awesome-Real-Time-Customer-Data-Platform-CDP

# Awesome-Real-Time-Customer-Data-Platform-CDP

## Top Real-Time Customer Data Platform (CDP) Ecosystem

**Curated List of SaaS Products & Open-Source GitHub Projects**  
*Focused on Warehouse-Native Data Ownership, Event Collection & Reverse ETL Activation*  
**Last updated: March 2026**

This repository tracks notable **SaaS platforms** and **open-source projects** for **Real-Time Customer Data Platforms (CDP)**. These tools unify customer data from every touchpoint — websites, apps, CRM, and offline sources — into a single profile, then activate that data in real time across marketing, sales, and service tools.

**Examples** include RudderStack, Jitsu, Multiwoven, LEO CDP, Helio, Hightouch, Segment, and mParticle (the category leaders).

**Open-source emphasis**: This section is heavily expanded with every major active project for self-hosting, warehouse-native data ownership, and transparent event pipelines — ideal for engineering-led teams who want CDP capabilities without per-MTU pricing that penalizes growth [citation:2][citation:9].

Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.

## Table of Contents
- [SaaS/Hosted Platforms](#saas-hosted-platforms)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## SaaS/Hosted Platforms

- **Segment** — **The reference commercial CDP.** Collects events once and routes them to hundreds of destinations. **Subscription-based** per Monthly Tracked User (MTU), which can become expensive at scale [citation:2]. **Best for teams starting their CDP journey** wanting the largest destination catalog and best documentation, accepting MTU-based pricing [citation:2][citation:15].

- **mParticle** — **The mobile-first enterprise CDP.** Purpose-built for iOS/Android with native SDKs and deep mobile attribution integrations (AppsFlyer, Adjust, Branch) [citation:2]. **Enterprise contact-sales pricing** based on event volume. **Best for mobile-first companies** where app instrumentation and attribution are primary concerns [citation:2].

- **Hightouch** — **The composable CDP and Reverse ETL leader.** Does not collect events — reads from your warehouse (Snowflake, BigQuery, Databricks) and syncs to 300+ SaaS destinations [citation:2]. **Free tier** (2 destinations, daily sync); **Starter $350/month**; **Business $1,500/month** [citation:2]. **Best for data-mature teams** with modeled warehouse data wanting activation without re-instrumentation [citation:2][citation:15].

- **Adobe Real-Time CDP** — Enterprise CDP within Adobe Experience Platform. Unifies known and anonymous data for real-time personalization across Adobe's ecosystem.

## Open-Source GitHub Projects

- **RudderStack** — **The leading open-source CDP and Segment alternative.** **AGPLv3 licensed**, warehouse-first architecture that keeps events in your own Snowflake/BigQuery rather than a vendor's infrastructure [citation:9]. **Segment API-compatible** — existing SDK integrations keep working; just swap the SDK [citation:2]. **200+ destination integrations**, JavaScript-based event transformations, and production deployments at Mattermost, IFTTT, and other large companies [citation:9]. **Pricing 50-80% below Segment** at comparable MTU volumes [citation:2][citation:9]. **Free tier (1M events/mo)** for the managed cloud; the open-source core can be self-hosted for free at any volume [citation:9]. **Best for technical teams** wanting warehouse-native data ownership with the lowest migration friction from Segment [citation:2][citation:15].

- **Jitsu** — **The open-source event collection layer.** **MIT licensed, self-hostable with no license restriction**, priced publicly from **$99/month for 2 million events** [citation:2]. **Segment-compatible SDKs** and event shape; ClickHouse included on the free tier (200,000 active events/month) [citation:2]. **Collection is the whole product** — it does not do reverse ETL or audience building [citation:2]. **Best for engineering-led teams** wanting a transparent, MIT-licensed pipe from app to warehouse with published pricing and no sales call [citation:2].

- **LEO CDP** — **The AI-first, self-hosted CDP framework.** Open-source, designed for developers and enterprises wanting **data sovereignty and on-premise intelligence** [citation:1]. **Omnichannel data collection** from websites, apps, CRM, POS, and IoT into a unified customer profile [citation:1]. **AI-based segmentation** with RFM analysis, CLV, churn prediction, purchase propensity, and lead scoring [citation:1]. **Event-driven architecture** with Dagster integration for ingestion and orchestration, plus **Agentic AI and LLM-powered personalization** [citation:1]. **Enterprise features**: consent management, RBAC, audit logs, multi-tenant architecture, Docker/Kubernetes support, and Prometheus/Grafana monitoring [citation:1]. **Best for organizations** wanting a fully customizable, self-hosted CDP with AI and ML at its core [citation:1].

- **Helio** — **The AI-native growth platform with CDP built in.** **Self-hostable and data-sovereign**, with **Segment/RudderStack-compatible HTTP Tracking API** so existing instrumentation points straight at Helio . **Insights**: event-stream funnels, cohort retention grids, multi-touch attribution (first/last/linear), and a read-only SQL explorer . **Multi-channel journeys**: email, web push, SMS (Twilio), WhatsApp (Cloud API), and in-app messages . **AI copilot** for segment/journey/email drafting, predictive lead scoring and churn, send-time optimization, and autonomous A/B winner selection — with **bring-your-own AI** (OpenAI, Anthropic, Groq, Ollama, or any OpenAI-compatible server) . **Enterprise SSO & SCIM**, credential vault with AES-256-GCM encryption, and **free forever with no contact caps** . **Best for teams wanting a modern, AI-native CDP** with self-hosting, unlimited contacts, and existing Segment-compatible instrumentation .

- **Multiwoven** — **The open-source Reverse ETL and CDP alternative.** **AGPL-3.0 licensed**, positioned as an open-source alternative to Hightouch, Census, and RudderStack [citation:3][citation:6]. **Connects to Snowflake, Redshift, BigQuery, and Databricks**; syncs to Salesforce, Braze, Slack, Klaviyo, Facebook Ads, and more [citation:3]. **SQL, visual builders, or dbt** for modeling; built-in scheduling and monitoring [citation:3]. **The honest limitation**: **Reverse ETL only** — it activates data from your warehouse but does not collect events from websites or apps [citation:3]. **Best for teams with an existing warehouse** wanting open-source activation to marketing and sales tools without Hightouch's pricing [citation:3].

## How to Contribute

1. Fork the repo.
2. Add/edit entries in `README.md` (follow existing format).
3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.
4. Submit PR with a short explanation.

Star the repo if you find it useful!

## Disclaimer

- This is a **community-curated** list — not exhaustive and not an endorsement.
- CDP tools differ significantly in architecture (event collection vs reverse ETL vs unified), licensing, and data ownership model. **RudderStack is the most complete open-source CDP** with Segment compatibility and warehouse-native design, but its **AGPLv3 license** requires review if you plan to modify and distribute it [citation:9]. **Jitsu is MIT-licensed and transparently priced**, but **does not do reverse ETL or audience building** — it is a collection pipe, not a full CDP [citation:2]. **Multiwoven is AGPL-licensed reverse ETL**, but **does not collect events** — it activates warehouse data [citation:3]. **Hightouch is commercial** with a free tier but requires a modeled warehouse and does not collect raw events [citation:2]. **LEO CDP and Helio are newer projects** — evaluate maturity and maintenance activity before production adoption [citation:1]. **The choice often comes down to architecture**: do you need event collection (RudderStack, Jitsu), warehouse activation (Multiwoven, Hightouch), or both?
- Self-hosted open-source solutions require proper database configuration (PostgreSQL for RudderStack, ClickHouse for Jitsu), reverse proxy setup, and awareness that "free" self-hosted still has infrastructure and maintenance costs.

---

**Made for data engineers, growth teams, and organizations building customer data platforms they can own and control.**
Let's make real-time CDP more open, warehouse-native, and licensing-transparent.
