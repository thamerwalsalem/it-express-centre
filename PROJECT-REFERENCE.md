# IT Express Centre | ITEC AI — Project Reference
Updated: 2026-10-21

## Purpose and governance
Bilingual Arabic/English IT-services platform for individuals and businesses, AI automation, smart home, digital projects, and tech shopping.
**Release rule:** Always prototype and get user approval before changing the production website. The user explicitly approved publishing the latest design after fixing the mobile dropdown on 2026-10-21. Do not publish future unapproved updates.
Avoid claims that services are available globally 24/7 without verified coverage, and do not imply that preview contact email is an operational ticketing backend.

## Public URLs
- Production: https://itec-ai.com
- GitHub repository: https://github.com/thamerwalsalem/it-express-centre
- GitHub Pages currently uses main /(root): https://thamerwalsalem.github.io/it-express-centre/
- Isolated design preview: https://thamerwalsalem.github.io/it-express-centre/preview-v2/
- Main production source: `index.html` on `main`
- Preview source: `preview-v2/index.html` on `main`
- Deploy workflow: `.github/workflows/deploy-hostinger.yml`, SSH/SFTP-over-SSH via rsync. Push changes to root-level *.html on main trigger deployment; edits in preview-v2 alone do not trigger production deployment.

## Domain and subscriptions
- Domain: `itec-ai.com`
- Registrar: **IONOS**
- Domain expiration/renewal date confirmed in prior user discussion: **2027-03-10**. Recheck within IONOS prior to renewal; renewal price/auto-renew status not verified here.
- Hosting: **Hostinger**, Business Web Hosting plan shared with Before9 / befor9.com; hosting plan expiration **2027-08-09** (this is hosting expiry, NOT itec-ai.com domain expiry). Hosting renewal pricing for ITEC not independently established.
- Prior B12 project used `it-express-center.b12sites.com`; current project deploys to Hostinger.
- DNS at IONOS was manually updated: A `@` → `147.93.54.140`; CNAME `www` → `itec-ai.com`; existing MX records were left unchanged. The public resolution status should be revalidated after any change.
- Hostinger SSH access: port `65002`; login info managed via Hostinger/GitHub secrets (never store passwords, secret values, or private host-key fingerprint in this file).
- GitHub Actions secrets for deployment include `HOSTINGER_SSH_PASSWORD`, `HOSTINGER_SSH_FINGERPRINT`. GitHub repository may contain other legacy FTP secrets; avoid copying or displaying values.

## Design decisions
- Homepage identity: rich navy/blue/cyan palette, original deployed-style wordmark/icon, NOT the light version tested in preview. Hero Arabic text:
  - `حلول تقنية برؤية عالمية`
  - `التقنية أصبحت أبسط معنا.`
  - `من المشكلات التقنية اليومية إلى تطوير أعمال الشركات، يساعدك IT Express Centre في الوصول إلى الدعم والحلول التقنية المناسبة.`
- Homepage contents reorganized into six destination cards while maintaining original dark visual identity.
- Internal pages: lighter backgrounds, separated informative cards, division-specific accent colors, consistent tricolor wordmark where IT and CENTRE are neutral while EXPRESS takes the section's accent color.
- Contextual contact CTA per page. Current mailto destination: `thamerwalsalem@hotmail.com`; form intake/ticket infrastructure is NOT confirmed as implemented.
- Arabic / English switch.
- A mobile dropdown contrast bug (white-on-white/unreadable navigation on dark homepage) was fixed in the preview and corresponding production source on 2026-10-21.

## Site structure
Current implementation is a hash-router single page HTML document: 1 landing view and 6 top-level division views = **7 interface views**, not 7 standalone HTML files.
Six categories and **35 service topics**:
1. `#/people` **الأفراد** / Individuals — red, 6: remote support; laptops/computers; phones/tablets; Internet/printers/networks; technician visit enquiry; device shopping/setup advice.
2. `#/business` **الشركات** / Businesses — electric blue, 6: service desk; managed IT support; device/software management; networks/infrastructure; cybersecurity/backup; consulting/on-site support.
3. `#/ai` **الذكاء الاصطناعي** / AI Transformation — purple, 6: AI readiness; roadmapping; AI customer-support assistants; contact-center automation; sales/process automation; intelligent reporting.
4. `#/home` **المنزل الذكي** / Smart Home — teal, 6: cameras/monitoring; smart locks; lighting; climate/device control; sensors/security; planning/installation.
5. `#/build` **ابنِ مشروعك** / Build Your Idea — gold, 6: e-commerce; websites; mobile apps; digital platforms; domains/hosting/email; payment/delivery integration.
6. `#/store` **المتجر التقني** / Tech Store — magenta, 5: cameras/locks; smart home devices; networking/WiFi; computer/mobile accessories; device/installation packages.

## What has been done
- Domain purchased via IONOS, hooked up to Hostinger with DNS changes.
- GitHub source-control repository and GitHub Pages preview working.
- GitHub Actions SSH-based deploy pipeline established and at least one previous deployment run shown successful by user.
- Reorganized six category layout and the internal designs.
- Updated homepage to preserve favored navy/cyan identity and text; dark vs light mobile nav contrast corrected.
- Production `index.html` was updated on GitHub after explicit approval on 2026-10-21. **Do not describe public website as verified live until independently tested.**

## Not finished / to verify before business launch
- Confirm last GitHub Actions deployment succeeded and production `itec-ai.com` displays the correct version on mobile + desktop, in both languages and across all six category views.
- Test navigation, accessibility, content, metadata, SEO, performance, SSL, privacy policy, terms, cookie policy if applicable.
- Design/implement secure working enquiry form, spam prevention, case/ticket data storage, notifications, and real support processes. A mailto link is currently only a link.
- Verify services and country-by-country partner coverage, pricing, support response commitments, fulfillment and payment before advertising those operationally.
- Verify e-commerce transactions/catalog, user accounts, technician partner enrollment/workflows; none confirmed as production ready.
- Confirm domain registrar renewal setting and payment instrument, subscription details and applicable renewal dates; monitor renewal before 2027-03-10.
- Keep project reference up to date after approved structural changes.

## External identifiers and safety
- Project/public site name: IT Express Centre | ITEC AI
- Administrative contact currently used by site's mail link: `thamerwalsalem@hotmail.com`.
- Do not commit FTP/SSH passwords, security tokens, Apple sign-in info, personal keys, or GitHub secrets.
