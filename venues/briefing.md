---
title: "Briefing"
---

# Briefing : Venues

> Entry point for any new reader. Executive summary in 1-2 pages.

## Summary

Venues is a B2B event venue marketplace (MICE : Meetings, Incentives, Conferences, Exhibitions) developed for Autentik Events. The platform connects event organizers and venue owners through an RFQ (Request for Quote) workflow : search, quote, visit, book.

Unified V1 delivery : 371 JH, target end of September 2026. Full engagement : ~7 months.

## Key figures

| Item             | Value                                                                                  |
| ---------------- | -------------------------------------------------------------------------------------- |
| Client           | Autentik Events (Charlotte Goncalves Vaz, Léa Simon)                                  |
| Target platforms | Web (Marketplace + Admin) + CMS                                                        |
| Stack            | Next.js 15 (front), React+Vite (admin), NestJS 11+PostgreSQL (back), Strapi v5 (CMS)  |
| DU team          | 11 : 4 devs, 1 BA, 3 QC, 1 PM, 1 tech lead, 1 DevOps (shared)                        |
| Modules          | 15 : Auth, Search, Venues, Quotes/RFQ, Visits, Messaging, Subscriptions, Blog, Groups, Partners, Reviews, Admin, Notifications, i18n, Payments |
| Methodology      | Agile, bi-weekly demos                                                                 |

## Main features

1. **Venue search** : filters by type, destination, lifestyle, capacity
1. **Quote requests** : express quotes and multi-venue RFQ
1. **Video visits** : scheduled via Twilio
1. **Partner subscriptions** : Stripe billing
1. **Messaging** : real-time, client-partner
1. **Admin back-office** : client, partner, venue, content management
1. **i18n** : FR/EN

## Key decisions

- 2025-07-28 : Contract signed, initial WBS of ~200 items
- 2026-01-15 : Timeline extended, scope re-evaluated
- 2026-03-03 : CR/Amendment meeting : scope and staging alignment
- 2026-03-04 : Arthus Chambon takes over as PM
- 2026-03-05 : Sprint 6 paused, focus on QA and bug fixes (P0 stabilization)
- 2026-03-11 : Scope consolidated with client under a single V1 delivery targeting end of September 2026
- 2026-03-12 : Documentation hub created as single source of truth

## Key risks and mitigations

| ID | Risk | Mitigation |
|---|---|---|
| R-01 | Full scope delivery over extended timeline | Strict feature freeze per sprint, overflow rule to defer lowest-priority items if velocity slips |
| R-02 | QA validation throughput on admin panel | Dedicated QA team (3 testers), parallel QA/dev workflow |
| R-03 | Payment integration complexity (Stripe) | Prioritized in Sprint 7, dedicated backend developer |

## Team

| Role             | Name                          |
| ---------------- | ----------------------------- |
| Technical Lead   | Paul de Renty                 |
| PM               | Arthus Chambon                |
| BA               | June (Thao Hoang)             |
| QC Lead          | Huy Nguyen (Silencer)         |
| QC               | Nhung Nguyen (Kira)           |
| QC               | Nin                           |
| FE Lead          | Quoc Le (Ryan)                |
| FE Dev           | Nguyen Hieu                   |
| BE Lead          | Mai Ly (William)              |
| BE Dev           | Hoang Tran (Ethan)            |
| DevOps (shared)  | Dat Tran                      |

## Documentation map

| Document                                             | Content                                            |
| ---------------------------------------------------- | -------------------------------------------------- |
| **Client context**                                   | <br />                                             |
| [client/about](05-client/about)                         | Client profile and organizational context          |
| [client/glossaire](05-client/glossaire)                 | Business terminology                               |
| **PRD / Functional specifications**                  | <br />                                             |
| [product/prd](01-product/prd)                           | Product description, scope, user roles, feature list |
| [product/scope](01-product/scope)                       | Scope decisions and module classification         |
| [product/wbs](01-product/wbs)                           | 3-level breakdown : Module > Feature > Story       |
| **TRD / Technical specifications**                   | <br />                                             |
| [technical/architecture](03-technical/architecture)     | Architecture and technical choices                 |
| [technical/specs](03-technical/specs)                   | Non-functional requirements                        |
| [technical/infrastructure](03-technical/infrastructure) | Infrastructure and deployment                      |
| [technical/bom](03-technical/bom)                       | Technical bill of materials                        |
| **UX**                                               | <br />                                             |
| [ux/user-flows](02-ux/user-flows)                       | User journeys and flow diagrams                    |
| [ux/ui-specs](02-ux/ui-specs)                           | UI/UX specifications                               |
| **Planning & Delivery**                              | <br />                                             |
| [planning/phases](04-delivery/phases)                   | Phasing and timeline                               |
| [delivery/coverage](04-delivery/coverage)               | Coverage matrix                                    |
| [delivery/engagements](04-delivery/engagements)         | Quality commitments                                |
