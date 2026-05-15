# Tealista — Technical Case Study

Tealista is a private, production-oriented multilingual tea discovery and marketplace platform.

The platform helps users discover teas, explore tea by type, origin and flavor profile, compare vendor offers and navigate to trusted tea shops.

Live website: https://tealista.com

> Source code is private. This repository presents the project scope, architecture and production engineering areas without exposing implementation details.

## Project Overview

Tealista combines a tea catalog, discovery experience, multilingual content structure, vendor offer flows and SEO-focused landing pages.

The product is designed as a marketplace foundation where tea shops can publish offers and users can compare available options before visiting a vendor website.

## Core Product Areas

- Multilingual tea catalog
- Tea detail pages
- Tea type, origin and flavor pages
- Vendor offers and external shop redirects
- Tea discovery and filtering experience
- Admin-oriented content management foundation
- Vendor/shop profile foundation
- Click tracking foundation for offer analytics
- SEO-oriented public pages
- Responsive desktop and mobile interface
- Light and dark theme support

## Technology Stack

### Frontend

- React
- Vite
- JavaScript / JSX
- Responsive UI
- Multilingual routing
- Custom styling system

### Backend

- Node.js
- Express
- MongoDB
- Mongoose
- REST API
- Authentication and role-based logic
- Vendor and offer handling

### SEO

- Custom SEO rendering layer
- Canonical URLs
- hreflang structure
- Sitemap structure
- JSON-LD structured data
- Search-engine-friendly public pages

### Infrastructure

- Render deployment
- Cloudflare DNS, CDN and security layer
- MongoDB database
- Sentry monitoring
- Resend transactional emails
- Environment-based configuration

## Architecture Overview

```text
User / Search Engine Bot
        |
        v
Frontend / SEO Layer
React + Vite + custom SEO rendering
        |
        v
Backend API
Node.js + Express
        |
        v
Database and Services
MongoDB, Sentry, Resend
        |
        v
Infrastructure
Render + Cloudflare
```

## Engineering Focus

### Multilingual Platform Structure

The platform supports multiple languages and language-specific public routes. The content architecture is designed to support localized tea pages, marketplace pages and SEO landing pages.

### SEO and Indexing

The project includes technical SEO work beyond standard meta tags, including canonical URLs, hreflang, sitemaps, structured data and bot-oriented rendering for public pages.

### Marketplace Logic

Tealista includes vendor offers, shop profiles, offer visibility rules and external redirect flows. The foundation supports future vendor analytics and monetization workflows.

### Production Deployment

The platform is deployed as a live production project with environment-based configuration, monitoring, logging and infrastructure-level routing.

### UX and Mobile Quality

The interface is developed with attention to responsive behavior, mobile usability, visual consistency and dark/light theme compatibility.

### Security and Hardening

The project includes practical hardening work around headers, redirects, rate limiting, environment separation, CDN configuration and production error monitoring.

## What This Project Demonstrates

- Building and maintaining a real production web platform
- Connecting frontend, backend, database and external services
- Designing multilingual content and routing structures
- Implementing technical SEO for public marketplace pages
- Handling production deployment and debugging
- Working with vendor and offer data flows
- Improving performance, mobile UX and reliability
- Applying infrastructure and security awareness in a real project

## Repository Scope

This repository does not contain source code, secrets, environment files or internal implementation details.

It is a public technical case study for a private commercial project.
