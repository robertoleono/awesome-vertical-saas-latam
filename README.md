# Awesome Vertical SaaS LatAm [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> A curated list of open source software, hosted alternatives, and tooling for building vertical SaaS targeting Latin American small and medium businesses (SMBs).

LatAm has 30M+ SMBs across dental, salons, law firms, accountants, restaurants, real estate, gyms, vet clinics and more. Most operate on WhatsApp + spreadsheets. This list maps the **open source building blocks** founders can use to build vertical SaaS for them, plus distribution channels that work in Spanish/Portuguese markets.

Maintained by [Roberto Leon](https://github.com/robertoleono). Contributions welcome — see [contributing](#contributing).

---

## Built using this stack · live products

A working demonstration of what this list enables. All built on the OSS components below, deployed to a single Hetzner server, billed via PayPal LIVE without LLC. Spanish-first for LatAm and Spain creators.

| Product | What it is | Stack | Pricing |
|---|---|---|---|
| [Boletines](https://nemomot.com/boletines/) | Managed Listmonk newsletter platform · alternative to Mailchimp billed in pesos | Listmonk + FastAPI + PayPal subscriptions | $9-29/mo |
| [Boletines Concierge](https://nemomot.com/concierge/) | Automated newsletter setup in 5 minutes · AI-generated branded templates | Listmonk + Claude API + PayPal one-time | $197 one-time |
| [100 Prompts AI Pack](https://nemomot.com/prompts/) | Curated AI prompts in Spanish for entrepreneurs · 7 categories | Static + PayPal one-time + Zoho delivery | $19 one-time |
| [NEMOMOT Community](https://nemomot.com/community/) | Premium community for Spanish entrepreneurs building with AI | Listmonk + PayPal subscriptions | $99/mo or $499/yr |

Affiliate program available · 25-40% commission · whitelisted manual approve: [/api/affiliate/signup](https://nemomot.com/api/affiliate/signup)

The full stack architecture is open and documented in this list. Anyone can replicate it.

## Contents

- [Booking and Scheduling](#booking-and-scheduling)
- [CRM and Sales](#crm-and-sales)
- [Customer Communication](#customer-communication)
- [Forms and Intake](#forms-and-intake)
- [Documents and E-signature](#documents-and-e-signature)
- [Email and Newsletters](#email-and-newsletters)
- [Analytics and Tracking](#analytics-and-tracking)
- [Workflow Automation](#workflow-automation)
- [Project and Task Management](#project-and-task-management)
- [Accounting and Invoicing](#accounting-and-invoicing)
- [Healthcare and Clinics](#healthcare-and-clinics)
- [Voice and Telephony](#voice-and-telephony)
- [AI Agents and LLM Tooling](#ai-agents-and-llm-tooling)
- [Payments LatAm](#payments-latam)
- [Vertical Niches Underexploited](#vertical-niches-underexploited)
- [Distribution Channels for LatAm](#distribution-channels-for-latam)
- [Hosting and Infrastructure](#hosting-and-infrastructure)
- [License Survival Guide](#license-survival-guide)
- [Bootstrap Playbooks Verified](#bootstrap-playbooks-verified)
- [Contributing](#contributing)

---

## Booking and Scheduling

- [Cal.diy](https://github.com/calcom/cal.diy) - MIT-licensed community fork of Cal.com after the latter went closed-source in April 2026. Self-host friendly, no AGPL friction. Strong base for vertical bookings (dental, salon, therapist).
- [Easy!Appointments](https://github.com/alextselegidis/easyappointments) - GPL-3.0 PHP self-hosted scheduler. Light, stable, weaker feature set than Cal.com but trivial to deploy.
- [Rallly](https://github.com/lukevella/rallly) - AGPLv3 group-poll scheduler (Doodle alternative). Wedge for events, classes, group therapy.
- [Odoo Calendar](https://www.odoo.com/page/community) - LGPL Community Edition. Native multi-tenant if you commit to Odoo as full ERP.

## CRM and Sales

- [Twenty CRM](https://github.com/twentyhq/twenty) - OSS Salesforce alternative built by ex-Pipedrive/Apple founders. Modern UI, GraphQL API, deployable on Hetzner in 10 minutes. Real LatAm wedge if you add WhatsApp-native pipeline view.
- [EspoCRM](https://github.com/espocrm/espocrm) - GPLv3 mature CRM. Strong Spanish localization already exists; good for traditional sales teams.
- [Krayin](https://github.com/krayin/laravel-crm) - MIT Laravel-based CRM. Easy for PHP-shops to fork and verticalize.
- [SuiteCRM](https://github.com/salesagility/SuiteCRM) - AGPLv3 SugarCRM Community successor. Heavy but battle-tested for enterprise-style features.
- [Monica](https://github.com/monicahq/monica) - AGPLv3 "personal CRM" — adaptable to coaches, realtors, therapists who manage individual relationships.

## Customer Communication

- [Chatwoot](https://github.com/chatwoot/chatwoot) - MIT (core) - Intercom/Zendesk alternative. Multi-channel inbox (web chat, email, WhatsApp via Twilio, Facebook, Instagram). One of the best LatAm-relevant OSS for small services teams.
- [Crisp Alternative · Tawk.to clones](https://github.com/papercups-io/papercups) - Papercups MIT-licensed live chat (now archived but forkable).
- [Mattermost](https://github.com/mattermost/mattermost) - MIT - Self-hosted Slack alternative. For LatAm SMB teams that need on-prem control for regulated industries.
- [Rocket.Chat](https://github.com/RocketChat/Rocket.Chat) - MIT - More mature Slack alternative with strong on-prem story. Brazil-based core team.
- [Evolution API](https://github.com/EvolutionAPI/evolution-api) - WhatsApp Business API wrapper. WARNING: Baileys-mode = HIGH ban risk per 2025 data; use only with official WA Cloud API.

## Forms and Intake

- [Formbricks](https://github.com/formbricks/formbricks) - AGPLv3 + cloud - Open Typeform/Qualaroo. Product Hunt #1 winner. Strong wedge for patient intake, lead capture, NPS surveys in Spanish.
- [Tally Alternative · Forms](https://github.com/forms-flow-ai/formsflow.ai) - Apache 2.0 form-builder + workflow.
- [Survey.js](https://github.com/surveyjs/survey-library) - MIT JS library + paid hosted Creator. Embedable forms for any vertical SaaS.
- [SelfHostedHQ Forms list](https://github.com/awesome-selfhosted/awesome-selfhosted#form-builders) - directory of additional options.

## Documents and E-signature

- [Documenso](https://github.com/documenso/documenso) - AGPLv3 + cloud - Open DocuSign. PH #1. Real wedge for LatAm notarías, abogados, contadores who pay USD-prices for Adobe Sign.
- [OpenSign](https://github.com/OpenSignLabs/OpenSign) - AGPLv3 simpler alternative, fewer features, lighter to deploy.
- [Docassemble](https://github.com/jhpyle/docassemble) - MIT - Interview/guided-document-generation system. Strong fit for legal vertical (intake → contract automatically).
- [Stirling-PDF](https://github.com/Stirling-Tools/Stirling-PDF) - MIT - Web-based PDF manipulation. Vertical play: PDF-heavy industries (notarías, contadores).

## Email and Newsletters

- [Listmonk](https://github.com/knadh/listmonk) - AGPLv3 single-binary newsletter manager. Used by Zerodha at millions/campaign on modest hardware. Wedge: Mailchimp es caro · Listmonk in pesos.
- [Mautic](https://github.com/mautic/mautic) - GPLv3 marketing automation. Notoriously hard to operate well → managed-Mautic-in-Spanish is a real play.
- [Keila](https://github.com/pentacent/keila) - AGPLv3 newer Elixir-based alternative, cleaner UX than Listmonk.
- [Postal](https://github.com/postalserver/postal) - MIT self-hosted SMTP relay (Mailgun/Postmark alt). Pair with Listmonk for full stack.
- [PowerMTA Alternative · Cuttlefish](https://github.com/openaustralia/cuttlefish) - GPL transactional email server.

## Analytics and Tracking

- [Umami](https://github.com/umami-software/umami) - MIT - Privacy-friendly Google Analytics alternative. Wedge: GA4 hates LatAm SMB users · Umami simpler + in pesos.
- [Plausible](https://github.com/plausible/analytics) - AGPLv3 - Bootstrapped to $1M ARR with 2 founders. Reference business model for OSS analytics.
- [PostHog](https://github.com/PostHog/posthog) - MIT (core) + paid enterprise. Product analytics + feature flags + session replay. Powerful but heavy for SMB.
- [Matomo](https://github.com/matomo-org/matomo) - GPLv3 - Mature GA alternative, complex.
- [Ackee](https://github.com/electerious/Ackee) - MIT - Lighter privacy analytics for personal sites.

## Workflow Automation

- [n8n](https://github.com/n8n-io/n8n) - Sustainable Use license (fair-code) - Zapier/Make alternative. $40M ARR · $2.5B valuation 2025. Vertical play: n8n templates pack for LatAm agencies + 1-click deploy.
- [Activepieces](https://github.com/activepieces/activepieces) - MIT alternative with TypeScript-first ergonomics.
- [Windmill](https://github.com/windmill-labs/windmill) - AGPLv3 - Faster execution engine; backend-friendly.
- [Huginn](https://github.com/huginn/huginn) - MIT - Old-school agent-based automation, low-level but powerful.
- [Trigger.dev](https://github.com/triggerdotdev/trigger.dev) - Apache 2.0 - TypeScript-native workflows + queues. Developer-tier.

## Project and Task Management

- [Plane](https://github.com/makeplane/plane) - AGPLv3 - Linear/Jira alternative. Spanish localization needed → real wedge.
- [Vikunja](https://kolaente.dev/vikunja/vikunja) - AGPLv3 - Todoist + Asana alternative. Single-user to small-team.
- [Focalboard](https://github.com/mattermost/focalboard) - MIT (Mattermost) - Trello-style kanban.
- [Wekan](https://github.com/wekan/wekan) - MIT - Mature Trello clone.
- [Tracim](https://github.com/tracim/tracim) - LGPL collaborative workspace alternative to Confluence.

## Accounting and Invoicing

- [Akaunting](https://github.com/akaunting/akaunting) - GPLv3 + paid modules - SMB accounting. Multi-currency, multi-language (ES/PT). Wedge: paired with LatAm e-invoicing (CFDI México, NFe Brasil) it becomes a vertical play.
- [InvoiceNinja](https://github.com/invoiceninja/invoiceninja) - Elastic License v2 (core free, hosted paid) - Established invoicing for freelancers and small teams.
- [Crater](https://github.com/crater-invoice/crater) - AGPLv3 - Modern Laravel + Vue invoicing.
- [Frappe Books](https://github.com/frappe/books) - LGPLv3 - Free desktop accounting for SMBs.
- [ERPNext](https://github.com/frappe/erpnext) - GPLv3 - Full ERP (Odoo-class) for small enterprises.

## Healthcare and Clinics

- [Medplum](https://github.com/medplum/medplum) - Apache 2.0 - FHIR-native, multi-tenant, 20M+ patients deployed. **The best base for new clinic SaaS in 2026.**
- [OpenEMR](https://github.com/openemr/openemr) - GPLv3 - ONC-certified mature EHR. Requires custom multi-tenant ops.
- [GNU Health](https://www.gnuhealth.org/) - GPL hospital information system. Hospital-scale.
- [Bahmni](https://github.com/Bahmni/bahmni-distro-default) - AGPL hospital + EMR + ERP stack for low-resource settings. Widely deployed in India and Africa.
- AVOID: HospitalRun (archived Oct 2025), LibreHealth (low signal), "Open Dental Software" (NOT OSS · source-visible only).

## Voice and Telephony

- [Asterisk](https://github.com/asterisk/asterisk) - GPL - Open source PBX. Pair with FreePBX UI for self-hosted phone systems.
- [FreePBX](https://github.com/FreePBX/) - GPL - GUI on top of Asterisk. Industry standard for on-prem PBX.
- [Kamailio](https://github.com/kamailio/kamailio) - GPL - Carrier-grade SIP server. Heavy for SMB; relevant for telephony resellers.
- [Faster-Whisper](https://github.com/SYSTRAN/faster-whisper) - MIT - 4-10x faster than vanilla Whisper, same accuracy. Self-hosted STT.
- [Kokoro-82M](https://huggingface.co/hexgrad/Kokoro-82M) - Apache 2.0 - Top of HuggingFace TTS Arena Jan 2025. CPU-viable. Commercial-clean.
- [Piper TTS](https://github.com/rhasspy/piper) - MIT (original) / GPL fork - 30+ languages including es-MX and pt-BR. Real-time on Raspberry Pi.
- [CosyVoice 2](https://github.com/FunAudioLLM/CosyVoice) - Apache 2.0 - Voice cloning from 5s reference, cross-lingual ES/PT/EN, 150ms streaming.
- [OpenVoice v2](https://github.com/myshell-ai/OpenVoice) - MIT - Voice cloning with style + emotion control.
- AVOID for commercial: F5-TTS (CC-BY-NC 4.0), XTTS-v2 (Coqui shut down Jan 2024, CPML license limbo), ChatTTS (AGPL).

## AI Agents and LLM Tooling

- [LangGraph](https://github.com/langchain-ai/langgraph) - MIT - Production-grade agent orchestration.
- [CrewAI](https://github.com/crewAIInc/crewAI) - MIT - Role-based multi-agent framework. Streaming tool calls Jan 2026.
- [AutoGen](https://github.com/microsoft/autogen) - CC-BY-4.0 + MIT - Microsoft multi-agent framework, prod-ready Oct 2025.
- [OpenHands](https://github.com/All-Hands-AI/OpenHands) - MIT - Most-starred autonomous coding agent (ex-OpenDevin).
- [Goose](https://github.com/block/goose) - Apache 2.0 - Block (Square) coding agent. 25+ LLM providers, 70+ MCP extensions, Linux Foundation governance.
- [Aider](https://github.com/Aider-AI/aider) - Apache 2.0 - Git-native AI coding assistant.
- [Cline](https://github.com/cline/cline) - Apache 2.0 - VS Code agent. Roo Code fork adds multi-agent modes.
- [Letta](https://github.com/letta-ai/letta) - Apache 2.0 - Stateful agent runtime (ex-MemGPT).
- [Mem0](https://github.com/mem0ai/mem0) - Apache 2.0 - Memory layer for any agent.
- [LiteLLM](https://github.com/BerriAI/litellm) - MIT - Unified gateway for 100+ LLM providers. Self-host on Hetzner.
- [Langfuse](https://github.com/langfuse/langfuse) - MIT (acquired by ClickHouse Jan 2026) - LLM observability + prompt management.
- [Inspect AI](https://github.com/UKGovernmentBEIS/inspect_ai) - MIT (UK AI Safety Institute) - 200+ pre-built evals.
- [Promptfoo](https://github.com/promptfoo/promptfoo) - MIT - Cross-model regression testing.
- AVOID: SuperAGI (dead · CVEs since Jan 2024), Helicone (maintenance mode post-Mintlify acquisition).

## Payments LatAm

- [Mercado Pago Checkout](https://github.com/mercadopago) - Official SDKs (closed but well-documented) for Argentina, Brazil, México, Colombia, Chile.
- [Wompi (Bancolombia)](https://docs.wompi.co/) - Colombia checkout · pesos colombianos.
- [Stripe LatAm](https://stripe.com/en-co) - Now available in Mexico/Brazil but requires LLC.
- [PayPal LIVE](https://developer.paypal.com/) - Works without US LLC. Critical for solo bootstrap operators in LatAm.
- [LemonSqueezy](https://www.lemonsqueezy.com/) - Merchant of Record, no LLC required, handles tax compliance globally.
- [Paddle](https://www.paddle.com/) - Alternative MoR, similar terms.
- [Belvo](https://belvo.com/) - Open Finance API for LatAm (Pluggy/Plaid for LatAm). Fintech building block.

## Vertical Niches Underexploited

Underserved verticals in LatAm where OSS base + vertical wrap + Spanish-first + WhatsApp-native could create a real moat:

- **Dental** clinics MX/CO/AR — Medplum + Cal.diy + Twilio WA
- **Salones / peluquerías** — Cal.diy + Listmonk for client retention
- **Notarías / abogados** MX — Documenso + Docassemble + e-firma SAT compliance
- **Contadores PYMES** AR/MX/CO — Akaunting + CFDI 4.0 (México) / NFe (Brasil) integration
- **Restaurantes** — Twenty CRM + Chatwoot + Plane for staffing + Listmonk for diner reactivation
- **Inmobiliarias** Brasil/MX — Twenty CRM + WhatsApp WA Cloud API + Listmonk for nurturing
- **Psicólogos / terapeutas** — Cal.diy + Formbricks intake + secure-notes (Standard Notes)
- **Gimnasios** — GymDesk-class (closed) opportunity for OSS Spanish equivalent
- **Veterinarias** — Medplum (FHIR adaptable) + Cal.diy + WhatsApp
- **Talleres mecánicos** — Twenty CRM + Akaunting + WA confirmations
- **Iglesias / religiosas** — ChurchTools-class, OSS gap in Spanish
- **Constructoras** — Plane (project mgmt) + Akaunting + Documenso (contratos)
- **Logística última milla** — n8n + Twenty CRM + WA shipper tracking
- **Educación / cursos** — Moodle / Open edX + Listmonk + Stripe Atlas LatAm
- **Eventos / wedding planners** — Cal.diy + Twenty CRM + Listmonk + Documenso

## Distribution Channels for LatAm

How OSS-based vertical SaaS actually reaches LatAm SMB owners:

- **WhatsApp groups by vertical** (Asociación Dental, Cámara Restaurantera, Colegio de Notarios, etc.) — high-trust, low-cost.
- **HDA · Hispanic Dental Association** (and equivalent associations per vertical).
- **r/Mexico, r/Argentina, r/Colombia, r/PararSer** — Reddit communities by country.
- **Latitud, Endeavor, Platzi, NUMA** newsletters — LatAm tech ecosystem reach.
- **Facebook Groups** vertical (e.g., "Dueños de Salones México") — still dominant for SMB owners 40+.
- **LinkedIn Posts in Spanish** — Latin professional class, B2B reach.
- **Local trade publications** (El Financiero, Valor Económico, La República, Cinco Días) — earned media.
- **Spanish-language podcasts** (Whitepaper, Founderz, Tres Tortas, Conscious Founders LatAm).
- **YouTube tutorials in Spanish** — vertical-specific deploy/usage guides convert.
- **University career-services boards** in LatAm engineering schools — recruit contributors + early users.

## Hosting and Infrastructure

- [Hetzner](https://www.hetzner.com/) - German hoster, cheapest dedicated + cloud in Europe. Foundation for LatAm OSS deployments. CCX13 starts at €18/mo; GEX44 GPU at €184/mo.
- [Coolify](https://github.com/coollabsio/coolify) - Apache 2.0 - Self-hosted Heroku/Vercel alternative. Deploy any GitHub repo to your own server.
- [Dokploy](https://github.com/Dokploy/dokploy) - Apache 2.0 - Lightweight PaaS, Argentina-built.
- [CapRover](https://github.com/caprover/caprover) - Apache 2.0 - Mature self-hosted PaaS.
- [Caddy](https://github.com/caddyserver/caddy) - Apache 2.0 - Auto-HTTPS reverse proxy. Simpler than Nginx for most cases.
- [Traefik](https://github.com/traefik/traefik) - MIT - Container-native reverse proxy. Works well with Docker Compose.
- [Cloudflare Free Tier](https://www.cloudflare.com/) - CDN + DNS + DDoS protection. Critical for LatAm latency.

## License Survival Guide

Which licenses are safe for commercial SaaS hosting:

| License | Commercial SaaS OK? | Notes |
|---|---|---|
| MIT / Apache 2.0 / BSD | YES | Free game. Compete on distribution. |
| MPL 2.0 | YES | Only modifications to MPL files must be open. |
| GPLv3 | YES (SaaS exception) | Distributing binary = must release. SaaS-only OK. |
| AGPLv3 | RISKY | Must release ALL modifications including SaaS. Buy commercial license from vendor or stay vanilla. |
| SSPL | NO for cloud providers | Designed to block "managed service" wrap by hyperscalers. |
| BSL | RESTRICTED | 4-year delay to OSS. Cannot compete with vendor cloud during BSL period. |
| Elastic v2 (ELv2) | NO | Same intent as SSPL. |
| CC-BY-NC | NO commercial | Will burn you silently. Common in AI models (F5-TTS). |
| Fair-code / Sustainable Use | RESTRICTED | n8n style. Self-host for internal OK; resale needs license. |

**Recent license changes that destroyed forks:**
- Redis SSPL → AGPL → [Valkey](https://github.com/valkey-io/valkey) fork (Linux Foundation, 83% enterprise migration in 1 year).
- Elastic SSPL → [OpenSearch](https://github.com/opensearch-project/OpenSearch) (AWS-backed).
- HashiCorp Terraform BSL → [OpenTofu](https://github.com/opentofu/opentofu) (Linux Foundation).
- MongoDB SSPL → AWS [DocumentDB](https://aws.amazon.com/documentdb/) (proprietary API-compat).
- Cal.com (April 2026) AGPL → closed-source for cloud; community fork [Cal.diy](https://github.com/calcom/cal.diy) preserves MIT path.

## Bootstrap Playbooks Verified

Real solo/small-team OSS bootstrap revenue cases with sources:

- [Plausible](https://plausible.io/blog/open-source-saas) — 2 founders, no VC, $1M ARR in 3 years. Tactic: 1 polemical blog post/month + HN front page.
- [Ghost](https://www.indiehackers.com/interview/how-john-onolan-grew-his-publishing-platform-to-750-000-year-14e5bac2fa) — Kickstarter $300K validation, 30K mailing list from one viral HN post, $7M+ ARR (Sep 2024) bootstrapped non-profit.
- [PostHog](https://www.plg.news/p/posthog-unconventional-growth) — 70% growth word-of-mouth, transparency core voice. Now $57.5M ARR Feb 2026.
- [Cal.com Open Startup](https://cal.com/open) — public salaries + ARR. $5.1M ARR 2024 before going closed-source.
- [Caleb Porzio · GitHub Sponsors](https://calebporzio.com/i-just-hit-dollar-100000yr-on-github-sponsors-heres-how-i-did-it) — $112K/yr from Sponsors via Livewire/Alpine.js ecosystem.

## Contributing

Pull requests welcome. Each entry must:

1. Be open source (have a clear OSI-approved license OR be source-available with explicit terms).
2. Have meaningful relevance to LatAm SMB verticals.
3. Be actively maintained (last commit within 12 months).
4. Include URL + 1-line description in present tense.
5. Specify license inline when license is restrictive (AGPL, SSPL, BSL, CC-BY-NC).

Categories should follow the existing structure. Add new categories only if 3+ entries justify them.

For commercial closed-source tools, propose them as "alternative-to" references rather than direct entries.

## License

[CC0 1.0 Universal](LICENSE) — public domain. Use freely.
