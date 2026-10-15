# IT Express Centre — Launch Roadmap

This repository contains a **prototype/marketing website**, not yet a transactional platform.

## Implemented in repository
- Bilingual Arabic/English main website with smart home, managed service desk, digital product creation, technology shopping ideas and technician network sections.
- AI Business Transformation discovery assessment (rules-based, not connected to an AI API).
- Affordable online store starter offers and client briefing form.
- Customer support guided troubleshooting and support request email draft.
- Technician interest registration email draft.
- Privacy/service disclosures for demo status.

Forms generate local email drafts. No backend, account registration, ticket database, commerce checkout, scheduling engine or remote-control integration is live.

## P0 — Before receiving real customer requests
1. Confirm GitHub Pages deployment and custom domain DNS + HTTPS.
2. Configure professional email (info@, support@, partners@), SPF, DKIM and DMARC at the mail provider.
3. Decide business entity, market, payment and terms; replace provisional policy with jurisdiction-appropriate privacy, refund and service terms.
4. Build secure backend, database, verified email notifications and admin dashboard.
5. Secure intake with spam protection, consent, retention and deletion procedures.

## P1 — MVP operations
1. Identity and roles (customer, verified technician, administrator).
2. Ticket lifecycle: open, triage, assigned, resolved, closed; email updates.
3. Secure helpdesk and human handoff from AI assistant; human escalation and transcript consent.
4. Technician onboarding, credential verification, availability, city coverage, pricing and dispatch.
5. Remote session workflow with explicit consent, vetted tooling and logs.

## P2 — Revenue
1. Managed service desk discovery, service tiers, SLAs, service quotes.
2. Smart home product compatibility checks + site assessment + installation partner offers.
3. Affordable store build packages: define platform, scope, revisions and third-party fees.
4. Affiliate/product sourcing pilot: verify program approval and supplier terms. No assumed Amazon/AliExpress integrations.
5. Domain and hosting reseller/partner agreements before collecting orders.

## P3 — Scale
1. AI Business Transformation consultation workflow, scoped discovery and measured pilots.
2. AI-powered support via secure API with bounded knowledge base; do not expose secrets in client JS.
3. Payment provider, tax handling, returns, fraud and cancellation flows.
4. Localized currencies, verified geographic coverage and service provider payouts.

## Editorial/technical standard
- Every new offer must be discoverable from the homepage/navigation and linked sensibly from related pages.
- Full Arabic and English coverage; navigation retains language via localStorage + optional URL language param.
- No promises of 24/7 coverage, global technicians, fixed cost, guaranteed earnings or unavailable inventory.
- Test responsive iPhone rendering, keyboard, accessibility and links before announcing production readiness.

## Business contacts
Current prototype sends mailto drafts to thamerwalsalem@hotmail.com until professional domain email is configured.
