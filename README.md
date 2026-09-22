# Tealista — Technical Case Study

Tealista is a production-oriented multilingual tea platform combining a canonical catalog, seller marketplace, commerce workflows, analytics and connected clients.

**Live:** https://tealista.com

> The application source is private. This repository documents the system without exposing production code, secrets or internal configuration.

## Platform

- Canonical tea and product catalog
- Seller offers and price comparison
- Native seller storefront and inventory workflows
- Cart, checkout and order domain
- Multilingual Web/PWA and technical SEO
- Browser extension, Telegram bot and Zepp OS client
- Editorial/admin workflows with role boundaries
- Market and price-history observation pipeline

## Engineering Highlights

**Catalog integrity**  
Tealista separates reusable tea identity from concrete products and seller offers:

```text
Tea -> TeaBatch / product -> Offer
                      ^
                VendorProduct
```

This allows offers to be compared only when product identity is sufficiently matched.

**Commerce**  
Seller products, variants, stock, delivery settings, orders, status history, returns/disputes and transactional stock reservation are implemented. Public payment surfaces remain feature-gated until payment/compliance rollout is approved.

**Multi-client platform**  
The same Core API supports Web/PWA, a browser extension, Telegram integration and a Zepp OS application with client-specific authentication boundaries.

**Analytics and market history**  
Offer price, availability and visibility changes can be recorded with provenance. Reconciliation/backfill tools are dry-run-first and designed to avoid inventing historical facts.

**Production engineering**  
PR validation runs on a self-hosted GitHub Actions runner with backend/frontend checks, database integration tests, client/device builds, Semgrep and secret scanning. Production releases use reviewed merges, Render deployment and live verification.

## Stack

| Area | Technology |
| --- | --- |
| Frontend | React, Vite, PWA |
| Backend | Node.js, Express |
| Data | MongoDB, Mongoose, Redis |
| Infrastructure | Render, Cloudflare |
| Quality | GitHub Actions, Playwright, Node tests, Semgrep |
| Integrations | Google Merchant, Telegram, browser extension, Zepp OS |

## More

- [Architecture](docs/architecture.md)
- [Project scope](docs/project-scope.md)
- [Security](docs/security-and-hardening.md)
- [SEO & production](docs/seo-and-production.md)
