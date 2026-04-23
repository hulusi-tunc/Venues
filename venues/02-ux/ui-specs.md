---
title: "UI Specs"
---

# UI/UX Specifications : Venues

> UI components and interface specifications for the Venues platform.

## 1. Design principles

- **Clarity** : consistent layout, visible hierarchy, readable typography
- **Trust** : subscription-based color coding, partner verification badges, public reviews
- **Efficiency** : single-form quote requests, comparison tools, multi-venue workflows
- **Responsive** : desktop-first, full mobile support

## 2. Global navigation

### Header (not logged in)

| Position | Element |
|----------|---------|
| Left | Venues logo (links to homepage) |
| Center | Type de lieu, Destination, Lifestyle, Projet sur mesure |
| Right | Devenir partenaire, Se connecter, Language selector (FR/EN) |

### Header (logged in, Client)

| Position | Element |
|----------|---------|
| Left | Venues logo |
| Center | Type de lieu, Destination, Lifestyle, Projet sur mesure |
| Right | Profile icon with dropdown menu |

**Client dropdown menu**:

| Section | Items |
|---------|-------|
| - | Dashboard |
| Gestion | Mes devis, Mes visites |
| VENUES | Mes recherches sauvegardees, Mes favoris, Mes avis |
| Partenaires | Mes favoris, Mes avis |
| - | Messagerie |
| - | Profil, Mot de passe, RGPD |
| - | Aide |
| - | Se deconnecter |

### Header (logged in, Partner)

Same structure as Client. Partner-specific dropdown menu:

| Section | Items |
|---------|-------|
| - | Dashboard, VENUES |
| Gestion | Mes devis, Mes visites |
| - | Messagerie |
| - | Profil, Abonnement, Mot de passe, RGPD |
| - | Aide |
| - | Se deconnecter |

### Footer

| Section | Content |
|---------|---------|
| Brand | Venues logo + social media icons (LinkedIn, Instagram, Facebook, YouTube) |
| Quick access | S'inscrire, Se connecter, Devenir partenaire, Les partenaires, Les groupes, Labels |
| En savoir + | A propos, Glossaire MICE, Manifeste, Projet sur mesure, Aide & FAQ, Le Mag |
| Nos brands | Seminaire international, Autentik Events, Anim'Finder |
| Legal | Mentions legales, CGU/CGV, Politique de confidentialite |
| Newsletter | Email signup field |
| Copyright | Copyright notice |

## 3. Key screens

### Homepage

| Section | Description |
|---------|------------|
| Hero | Search bar (keyword + "Rechercher" + "Recherche avancee" button) |
| References | Client logos carousel (admin-managed) |
| Notre collection | Category cards (10 categories, color-coded by subscription type) |
| Key features | Platform features section |
| Latest venues | Carousel: 12 venues, 3 per page, navigation arrows |
| Partner focus | Video spotlight (4 max, admin-managed) |
| Testimonials | Carousel of testimonials |

### Search Results

| Element | Description |
|---------|------------|
| Filter sidebar | Type, destination, lifestyle, capacity, services (modal on mobile) |
| Venue cards | Image, title, category tag (color-coded), country, city, capacity |
| Sort options | Relevance, newest, capacity |
| Pagination | Numbered pages with prev/next arrows |
| Comparison bar | Sticky bottom bar showing selected venues for comparison |

### Venue Detail

| Element | Description |
|---------|------------|
| Image gallery | Photo carousel with thumbnails |
| Venue info | Name, category, location, capacity, rooms, meeting rooms |
| Services | Services and equipment lists |
| Map | Google Maps embed with venue location |
| Primary CTA | "Request quote" button |
| Secondary CTA | "Schedule visit" button |
| Actions | Favorite toggle (heart), add to comparison |
| Partner sidebar | Photo, name, rating, contact button |
| Reviews | User reviews section |

### Partner Profile Page

| Element | Description |
|---------|------------|
| Header | Photo (subscription-colored border), first name, function, company, group (link), rating |
| Contact | "Contact" button (opens messaging or login popup) |
| Badge | "Cap vers l'avenir" badge (if donated) |
| About | Languages, values (carousel), anecdote |
| Commitments | Ethical commitments (6 max) |
| Video | Video section (subscription-colored border) |
| Statistics | Venue distribution by category/country/city (charts) |
| Venues | Thumbnail list, recent to oldest |
| Reviews | Sortable, 3 criteria ratings, partner replies |

### Client Dashboard

| Section | Content |
|---------|--------|
| My quotes | Sent, pending, accepted, refused |
| My visits | Upcoming, past |
| My favorites | Venues, partners |
| My reviews | Submitted reviews |
| Saved searches | Stored search criteria |
| Messaging | Conversation inbox |

### Partner Dashboard

| Section | Content |
|---------|--------|
| My venues | Venue list, create new |
| Incoming quotes | Quote requests received |
| Visit requests | Pending and confirmed visits |
| Reviews | Reviews received |
| Subscription | Current plan and status |
| Messaging | Conversation inbox |

## 4. Transversal patterns

| Pattern | Behavior |
|---------|---------|
| Search | Autocomplete suggestions, keyboard accessible |
| Filters | Dropdown/autocomplete, combinable, clearable |
| Empty state | Contextual message + CTA (e.g., "No favorites yet, discover venues") |
| Confirmation | Modal dialog for destructive actions (delete, cancel) |
| Loading | Skeleton screens for cards, spinners for actions |
| Toast notifications | Sonner toasts for success/error feedback |
| Pagination | Numbered pages with prev/next arrows |
| Image upload | Drag-and-drop + file picker, preview before upload |
| Rich text | Tiptap editor for descriptions and content |
| Form validation | Inline errors below fields, red borders |
| Auth guard | Non-logged users see popup: "Sign up / Login" on protected actions |

## 5. Color coding (subscription-based)

| Subscription | Color | Usage |
|-------------|-------|-------|
| Hotels | Rose / Pink | Category tags, partner photo border |
| Restaurants | Orange | Category tags, partner photo border |
| Event Venues | Blue | Category tags, partner photo border |
| Multi-VENUES | Bordeaux | Category tags, partner photo border |

## 6. Responsiveness

| Breakpoint | Behavior |
|-----------|---------|
| < 640px (Mobile) | Single column, hamburger menu, stacked cards, bottom sheet filters |
| 640-1023px (Tablet) | 2-column grid, collapsible sidebar |
| 1024-1279px (Desktop) | Full layout, sidebar filters, 3-column card grid |
| >= 1280px (Large) | Max-width container, 4-column grid |
