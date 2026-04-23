---
title: "Glossaire"
---

# Glossaire : Venues

## Business terms

| Term | Definition | French equivalent |
|---|---|---|
| Venue | A physical location available for events (hotel, restaurant, event space, etc.) | Lieu |
| Partner | A venue owner or service provider registered on the platform | Partenaire |
| Client | An event organizer searching for venues and requesting quotes | Client |
| Quote / RFQ | A formal request for pricing and availability sent to one or more venues | Devis / Demande de devis |
| Express Quote | A single-venue quote request with immediate response expected | Devis express |
| Multi-venue Quote | A quote request sent to multiple venues simultaneously | Devis multiple |
| Visit | A scheduled tour of a venue (in-person or video call) | Visite |
| Video Visit | A remote venue tour conducted via video call (Twilio) | Visite vidéo |
| Subscription | A paid plan allowing partners to list venues on the platform | Abonnement |
| Pioneer Subscription | A lifetime subscription offered to the first 1000 partners (one-time payment) | Abonnement pionnier |
| Group | An organization owning multiple venues or partners | Groupe |
| Independent | A partner not affiliated with any group | Indépendant |
| Label | A certification or quality marker for venues | Label |
| Positioning | The market segment of a venue (budget, mid-range, premium, luxury) | Positionnement |
| Lifestyle | A thematic category for venue discovery (e.g., eco-friendly, urban) | Lifestyle |
| Le Mag | The platform blog/magazine section (Strapi CMS) | Le Mag |
| Custom Project | An event brief submitted by a client for venue suggestions matching specific criteria | Projet sur mesure |
| MICE | Meetings, Incentives, Conferences, Exhibitions : the B2B professional events industry | MICE |
| Staging | The pre-production environment where validated features are shown to the client | Recette / Staging |
| CR | Change Request : a modification to the original scope | Demande de changement |
| Location | Legacy code term for a Venue entity (frontend routes use `my-location`; backend entity is `VenueEntity`) | Lieu (code) |
| Project | A quote request context where a client describes their event needs | Projet |
| Highlights | Featured or promoted content on the homepage (venues, articles) | Mise en avant |
| Sheet | A partner's public profile page displaying venue details | Fiche partenaire |

## Acronyms

| Acronym | Expanded | Context |
|---|---|---|
| RFQ | Request for Quote | Core marketplace flow |
| MICE | Meetings, Incentives, Conferences, Exhibitions | Industry vertical |
| CMS | Content Management System | Strapi for blog/content |
| SSO | Single Sign-On | Google/LinkedIn authentication |
| RBAC | Role-Based Access Control | Admin permission system |
| QC | Quality Control | Internal testing before staging |
| QA | Quality Assurance | Client-side acceptance testing |
| CR | Change Request | Scope modification tracking |
| BA | Business Analyst | Requirements and Jira management |
| PM | Project Manager | Sprint planning and client communication |
| PV | Procès-Verbal | Sprint acceptance document |
| CI/CD | Continuous Integration/Deployment | Build and deploy pipeline |
| RGPD | Règlement Général sur la Protection des Données | GDPR in French context |
| CGU/CGV | Conditions Générales d'Utilisation/Vente | Terms of use/sale |

## Roles and user profiles

| Role | Description | Key permissions |
|---|---|---|
| Client (Company) | Corporate event organizer | Search, quote request, visit booking, messaging, reviews |
| Client (Event Agency) | Professional event planning agency | Same as Company plus multi-venue quotes |
| Client (Association) | Non-profit organization | Same as Company |
| Partner | Venue owner or service provider | Venue listing, quote response, subscription management, messaging |
| Admin (Super Admin) | Platform administrator | Full access to all management modules |
| QC Tester | Internal quality control | Access to staging, bug reporting |

## Standards and applicable regulations

| Standard | Scope | Description |
|---|---|---|
| RGPD / GDPR | Data protection | Personal data processing, consent management, right to deletion, data export. Applies to all user data (clients, partners, admins). |
| PCI-DSS | Payment security | Compliance via Stripe (PCI Level 1 certified processor). No card data stored on platform servers. |
| WCAG 2.1 AA | Accessibility | Web Content Accessibility Guidelines : keyboard navigation, screen reader support, contrast ratios (4.5:1), responsive design up to 200% zoom. |

## Key business rules

- `[RG-01]`: partners must have an **active subscription** to list venues
- `[RG-02]`: each partner can list up to **5 venues** by default (admin can increase the limit)
- `[RG-03]`: venues shift to **expired** status if partner subscription lapses
- `[RG-04]`: quote requests generate **automatic notifications** to relevant partners
- `[RG-05]`: reviews require a **validated quote** before submission
- `[RG-06]`: reviews are subject to **admin moderation** before publication
- `[RG-07]`: content flagged by users triggers **admin notification**
- `[RG-08]`: partner profile photos have subscription-based **color coding** (Hotels: Rose, Restaurants: Orange, Event venues: Blue, Multi: Bordeaux)
- `[RG-09]`: pioneer subscriptions are **lifetime** (1000 max, one-time payment)
- `[RG-10]`: admin can **block** clients or partners (venues become invisible)
- `[RG-11]`: RGPD: admin receives notification on **data deletion requests**, automatic email sent
- `[RG-12]`: labels can be proposed by users but require **admin validation**
- `[RG-13]`: newsletter managed via **Brevo** integration
- `[RG-14]`: site must be available in **FR and EN**
