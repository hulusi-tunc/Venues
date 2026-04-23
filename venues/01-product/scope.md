---
title: "Scope"
---

# Scope : Venues

Scope definition for the Venues project. All features below are part of the unified V1 delivery, target end of September 2026.

> **Module classification note** : the WBS retains the historical module grouping (M1-M14 as Core and M15 as Admin Advanced) for estimation and traceability. Both groups are delivered as part of the unified V1 scope — there is no separate V2 phase.

## Scope summary

| Feature | Module | Notes |
|---------|--------|-------|
| Authentication (email, Google SSO, LinkedIn SSO) | M1 | |
| Two-factor authentication (admin) | M1 | F1.7 |
| Venue search, filters, comparison | M2 | |
| Venue listing, detail pages, creation | M3 | |
| Price catalog per venue | M3 | F3.8. Partner-managed catalog (articles, PU, TVA, CGV) |
| Venue limit configuration (admin) | M3 | F3.6 |
| Venue preview mode (admin) | M3 | F3.7 |
| Quote request (express + multi-venue) | M4 | |
| Quote drafts (save and resume) | M4 | F4.6 |
| Quote per-day article selection (7 categories) | M4 | F4.7 |
| Invoice generation post-quote | M4 | F4.8 |
| Visit scheduling (in-person + video) | M5 | |
| Real-time messaging (Socket.io) | M6 | |
| File attachments in messaging | M6 | F6.3 |
| Message archiving and flagging | M6 | F6.4 |
| Notification history in chat thread | M6 | F6.5 |
| Subscriptions and Stripe payments | M7 | |
| Promo codes and discounts | M7 | F7.5 |
| Invoice download (partner subscriptions) | M7 | F7.6 |
| Cancellation reason tracking | M7 | F7.7 |
| Reviews and ratings | M8 | |
| Favorites (venues + partners) | M9 | |
| Groups and partner directory | M10 | |
| Blog / Le Mag (Strapi), FAQ, static pages | M11 | |
| Admin : client, partner, venue, content CRUD | M12 | |
| Admin RBAC (6 roles) | M12 | F12.7. Super Admin, Moderateur, Support client, Dev, Marketing, Commercial |
| Admin messaging (admin-to-user) | M12 | F12.8 |
| Admin payment management and Stripe sync | M12 | F12.11 |
| Admin dashboard (key metrics, KPIs) | M12 | F12.6 |
| i18n (FR / EN) | M13 | |
| Navigation, layout, legal pages, Calendly | M14 | |
| Axeptio cookie consent | M14 | RGPD requirement |
| Action history / audit log | M12 | Code exists |
| Newsletter signup (Brevo) | M14 | |
| Backup management UI | M15 | Code exists in dev |
| Maintenance mode toggle | M15 | Code exists in dev |
| A/B testing framework | M15 | F15.2 |
| Advanced analytics dashboards | M15 | F15.1 |
| ODOO integration | M15 | F15.6 |
| Advanced SEO (Google Search Console, scoring) | M15 | F15.6 |
| Notification system (templates, campaigns, metrics) | M15 | F15.4 |
| Content moderation (approval, auto-flagging, history) | M15 | F15.5 |
| Translation management UI | M15 | F15.8 |
| Media buying / donation management | M15 | F15.8 |
| Sandbox mode | M15 | F15.9 |
| Beta feature access | M15 | F15.10 |
| Feedback widget | M15 | F15.11 |
| Email tracking (open/click rates) | M15 | F15.12 |
| Newsletter full management (Brevo) | M15 | F15.13. Templates, lists, campaigns, automation |
| Global media management | M15 | F15.14. Compression, Remove.bg config |
| Admin documentation (Loom, guidelines) | M15 | F15.15 |
| Graphic management (typography, icons) | M15 | F15.16 |
| Tidio or equivalent live chat | M15 | F15.6 |
| Automated subscription reminders | M15 | F15.3 |
| Support tickets and feedback tracking | M15 | F15.17 |
| CRM notes (internal notes per client) | M15 | F15.18 |
| Media buying and venue credits | M15 | F15.19 |
| Login activity tracking and security logging | M15 | F15.20 |
| Data export (CSV, analytics, GDPR) | M15 | F15.21 |

## Pending decisions

| Subject | Options | Target date | Blocker |
|---|---|---|---|
| Admin panel full scope | Streamlined admin vs full admin at launch | 2026-03-14 | Dedicated admin cadrage session planned |
| Stripe plan structure | Monthly/Annual only vs Pioneer + Monthly/Annual | 2026-03-14 | Pending Charlotte validation |
| Video visit implementation | Full Twilio vs simplified link sharing | 2026-03-21 | Integration approach to be confirmed |
| Notification system | Basic email only vs email + in-app + push | 2026-03-21 | Automation scope to be confirmed |
| Remove.bg integration | Client provides API key vs DU account | TBD | Pending client input |
| Moderation queue (US-167) | Delivered as part of admin workflow at launch vs later iteration | 2026-03-14 | Pending client input on launch requirements |
