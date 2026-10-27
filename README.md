# Awesome-Extended-Enterprise-Learning

# Top Extended Enterprise Learning Ecosystem

**Curated List of SaaS Products & Open-Source GitHub Projects**  
*Focused on Customer Training, Partner Enablement & External Learner Portals*  
**Last updated: October 2026**

This repository tracks notable **SaaS platforms** and **open-source projects** for **Extended Enterprise Learning**. These tools enable organizations to deliver training to external audiences—customers, partners, resellers, and franchisees—through branded, self-service learning portals that drive product adoption, reduce churn, and generate revenue.

**Examples** include Workday Extended Enterprise, Docebo, Cornerstone OnDemand, Absorb LMS, SAP Litmos, LearnUpon, Thought Industries, Skilljar, TalentLMS, and Canvas LMS (the category leaders).

**Open-source emphasis**: Extended Enterprise Learning is a domain where open-source tooling is **fragmented and largely incomplete**. The strongest options are **Moodle with IOMAD** (mature multi-tenancy with white-labeling, per-tenant SSO, and ecommerce)  and **Open edX with eox-tenant** (multi-tenant plugin for MOOC-scale external learning) . Newer projects like **TutorLoom** and **euron-open-lms** address multi-tenancy and external commerce but are early-stage . No open-source platform matches Skilljar's purpose-built external LMS capabilities (Salesforce integration, customer success data, revenue attribution) out of the box.

Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.

## Table of Contents
- [SaaS/Hosted Platforms](#saas-products)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## SaaS/Hosted Platforms

- **[Workday Extended Enterprise](https://www.workday.com/)**  
  External learning capabilities within Workday's suite for delivering training to customers, partners, and extended workforce with branded portals and integration with Workday HCM and financial data.

- **[Docebo](https://www.docebo.com/)**  
  AI-powered learning platform with **Extended Enterprise** module for customer, partner, and employee training through branded, multi-portal experiences with ecommerce and Salesforce integration.

- **[Cornerstone OnDemand](https://www.cornerstoneondemand.com/)**  
  Talent management platform with extended enterprise capabilities for external training delivery and partner enablement.

- **[Absorb LMS](https://www.absorblms.com/)**  
  LMS with external training support including ecommerce, branded portals, and content integrations for customer and partner education.

- **[SAP Litmos](https://www.litmos.com/)**  
  Rapid-deployment LMS with built-in ecommerce and external learner support for customer and partner training.

- **[LearnUpon](https://www.learnupon.com/)**  
  LMS with **multi-portal support** for customer, partner, and employee training, plus ecommerce and Salesforce integration.

- **[Thought Industries](https://www.thoughtindustries.com/)**  
  Purpose-built **customer, partner, and professional training** platform named #1 Customer Training System three years running by Craig Weiss Group; features **Panorama** multi-tenant portals for channel partners/resellers/franchisees , instructor-led and virtual instructor-led training management , ecommerce, and advanced reporting.

- **[Skilljar](https://www.skilljar.com/)**  
  The external LMS purpose-built for **customer and partner education** by Gainsight; features branded Academies with SSO, AI-assisted content creation, certification programs with proctored exams, native Stripe commerce (100+ currencies), Salesforce/Gainsight CS/Zendesk/Marketo integrations, and an MCP Server for AI workflows . Gartner reviewers praise ease of use and analytics but note cost concerns and lack of native mobile app .

- **[TalentLMS](https://www.talentlms.com/)**  
  Cloud LMS with ecommerce and external training capabilities for small to mid-sized teams.

- **[Canvas LMS](https://www.instructure.com/canvas)**  
  Academic LMS with open-source core; can be configured for external training but not purpose-built for extended enterprise commerce or partner enablement.

## Open-Source GitHub Projects

- **[Moodle + IOMAD](https://github.com/iomad/moodle-local_iomad)**  
  The **most mature open-source extended enterprise solution** available. IOMAD is a suite of Moodle plugins adding **comprehensive multi-tenancy**: white-labeling (themes, URLs, certification, emails, authentication, course sharing), **per-tenant OIDC and SAML 2 SSO**, per-tenant corporate hierarchies (parent/child), per-tenant role capabilities for tenant self-management, license-based enrollment, advanced compliance reporting, automated course lifecycles, face-to-face training events with waiting rooms and approval workflows, learning paths, and an **ecommerce solution with per-tenant payment accounts and pricing structures** . Developed by Moodle Partner e-Learn Design. Requires Moodle core patches. **This is the closest open-source equivalent to Docebo Extended Enterprise or Thought Industries Panorama**, with years of production use in commercial training contexts.

- **[Open edX + eox-tenant](https://github.com/eduNEXT/eox-tenant)**  
  Open edX is the MOOC-scale platform powering edX.org; **eox-tenant** (by eduNEXT) is a plugin replacing the older microsites feature with a **robust multi-tenancy model**: microsites for tenant configuration, routes for tenant URLs, tenant configs, and tenant organizations linking organizations to tenants . Compatible with Open edX releases from Ironwood through Verawood. While not purpose-built for commerce like IOMAD, it enables running multiple branded learning portals from a single Open edX instance—suitable for organizations delivering external training at scale without per-tenant infrastructure. **Commerce and partner enablement require additional development**; Open edX itself is course-delivery focused rather than customer-training focused.

- **[TutorLoom](https://github.com/pacewisdomhq/TutorLoom)**  
  Self-hosted, **multi-tenant LMS** for training institutes and teams (Apache-2.0); features course builder, trainer and student portals, progress tracking, batches, organizations, analytics dashboards, and JWT authentication with role-based access . Django 6 + React 19 + PostgreSQL + Redis/Celery stack. **Early-stage** but explicitly designed for multi-tenant training delivery—the architecture aligns with extended enterprise needs, though it lacks the ecommerce, white-labeling depth, and partner hierarchy features of IOMAD.

- **[euron-open-lms](https://github.com/euron-sde-team/euron-open-lms)**  
  Open-source, self-hosted LMS with **Stripe Checkout/Billing and Razorpay** commerce, verifiable certificates with public verification pages, subscriptions, coupons, refunds, and a full admin control plane . Features HLS video, quizzes, reviewed assignments, Q&A threads, moderation, and a mobile app (iOS/Android) with offline downloads. **Commerce is native and well-architected** (gateway routing per currency, tax handling, webhook reconciliation). **Not explicitly multi-tenant**—each deployment serves one organization/brand—but provides the ecommerce and certification infrastructure extended enterprise training businesses need. Early-stage but architecturally ambitious.

- **[ClassroomIO](https://github.com/classroomio/classroomio)**  
  Open-source no-code LMS for bootcamps, educators, and businesses (SvelteKit + Supabase); features unlimited courses, multi-teacher management, AI course creation, student forums, and dedicated dashboards . **Not multi-tenant** and lacks commerce/partner features, but suitable for small training businesses delivering external education without enterprise complexity.

### Additional Strong Open-Source Options

- **MuTMS** — Moodle distribution with multi-tenancy patches and plugins (programs, certifications, training credits, supervisors/teams) assembled for easier deployment ; an alternative packaging of Moodle multi-tenancy if IOMAD's specific feature set isn't required.
- **Richie (with Open edX)** — Learning portal CMS that can aggregate courses from multiple Open edX instances into branded course catalogs; the `tutor-contrib-richie-site-factory` plugin enables running multiple Richie sites ; useful for creating external-facing course catalogs while Open edX handles delivery.

**Frameworks for building custom systems**: **Moodle + IOMAD** is the only mature open-source option that covers the core extended enterprise requirements: multi-tenancy, white-labeling, per-tenant SSO, partner hierarchies, and ecommerce . **Open edX + eox-tenant** provides multi-tenant course delivery at MOOC scale but requires commerce development . **euron-open-lms** provides modern commerce infrastructure but single-tenant . A complete extended enterprise stack for organizations needing customer/partner training with revenue generation would most practically center on IOMAD, with custom development for Salesforce/customer-success integrations comparable to Skilljar.

## How to Contribute

1. Fork the repo.
2. Add/edit entries in `README.md` (follow existing format).
3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.
4. Submit PR with a short explanation.

Star the repo if you find it useful!

## Disclaimer

- This is a **community-curated** list — not exhaustive and not an endorsement.
- Extended enterprise learning platforms handling customer and partner data must comply with applicable privacy regulations and ecommerce laws; training records and certification data may have contractual and regulatory retention requirements.
- **Open-source extended enterprise learning is viable but not turnkey**—IOMAD provides mature multi-tenancy and ecommerce on Moodle, but requires Moodle expertise and core patches . Open edX multi-tenancy is course-delivery focused without native commerce . Newer projects (TutorLoom, euron-open-lms) are architecturally promising but early-stage . Organizations requiring Salesforce/customer-success integration and revenue attribution comparable to Skilljar should plan for commercial platforms or significant custom development.
- Verify license terms for commercial use; IOMAD is GPL-compatible Moodle plugin , eox-tenant is open-source , TutorLoom is Apache-2.0 , and euron-open-lms is open-source .

---

**Made for customer education leaders, partner enablement teams, training business owners, and extended enterprise platform architects.**  
Let's make extended enterprise learning more open, branded, and revenue-capable.
