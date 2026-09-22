# SEO and Production

## SEO

Tealista serves multilingual public pages through a dedicated SEO layer with:

- Canonical URLs and hreflang
- Sitemaps
- Localized metadata
- JSON-LD for catalog, product and offer pages
- Searchable concrete-product pages
- Google Merchant XML feed support

## Performance

Catalog work includes reduced database payloads, completed-page caching, cache prewarming and stale-content strategies to keep public browsing responsive during refreshes.

## Release process

```text
short-lived branch
      -> pull request
      -> tests + security checks
      -> reviewed merge to main
      -> Render deployment
      -> live production verification
```

CI includes backend/frontend tests, database integration checks, browser-extension and device builds, Semgrep and secret scanning on a self-hosted runner.
