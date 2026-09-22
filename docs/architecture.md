# Architecture

Tealista is built as a shared platform rather than a collection of independent clients.

```text
Web / PWA        Browser Extension        Telegram        Zepp OS
     \                 |                    |               /
                      Core API
                         |
              Catalog / Commerce / Users
                         |
                  MongoDB + Redis
                         |
               Jobs and integrations
```

## Core domains

### Catalog

```text
Tea
  -> TeaBatch / identifiable product
       -> Offer
VendorProduct -> matching / source evidence
```

The canonical tea remains independent from a seller. Seller-specific price, stock and URL data live on offers.

### Commerce

Native shop infrastructure includes seller products, variants, stock, delivery settings, checkout, orders and transactional inventory reservation/restoration.

Payment UI remains feature-gated.

### Clients

Current clients include Web/PWA, browser extension, Telegram bot and Zepp OS.

Each client uses the same API contracts while keeping authentication and permissions scoped to its needs.

### Public web

A dedicated SEO layer serves canonical, localized public pages and structured data without exposing private application state.
