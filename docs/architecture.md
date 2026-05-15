# Architecture

Tealista uses a split web platform architecture built around a frontend application, backend API, database layer and infrastructure services.

## High-Level Structure

```text
Client / Search Bot
        |
        v
Frontend and SEO Layer
        |
        v
Backend API
        |
        v
Database and External Services
```

## Frontend Layer

The frontend is responsible for public user-facing pages, discovery flows, tea catalog navigation, vendor offer presentation, localization and responsive UI.

Main areas:

- React application structure
- Vite build pipeline
- Multilingual route handling
- Tea catalog and detail views
- Vendor offer UI
- Responsive layouts
- Theme-aware interface styling

## Backend Layer

The backend provides API functionality for teas, vendors, offers, users, admin workflows and tracking-related foundations.

Main areas:

- Node.js and Express API
- MongoDB data models
- Mongoose schema layer
- Authentication and role-based logic
- Vendor and offer data handling
- Redirect and click-tracking foundations
- Validation and production safeguards

## SEO Layer

The project includes a dedicated SEO-oriented rendering layer for public pages.

Main areas:

- Search-engine-friendly HTML output
- Canonical URLs
- hreflang structure
- Sitemap support
- JSON-LD structured data
- Public route metadata

## Infrastructure Layer

The platform runs with external production services for deployment, CDN/security, monitoring and transactional email.

Main areas:

- Render deployment
- Cloudflare DNS/CDN/security
- MongoDB database
- Sentry monitoring
- Resend transactional email
- Environment-based configuration

## Design Principle

The architecture prioritizes production stability, clear separation between frontend and backend, SEO visibility, multilingual scalability and safe handling of vendor-related marketplace flows.
