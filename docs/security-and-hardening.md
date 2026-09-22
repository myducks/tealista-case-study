# Security and Hardening

Tealista uses explicit security boundaries across public, user, seller, editorial and admin flows.

## Controls

- Authentication and role/ownership checks in backend controllers
- Trusted-origin checks for state-changing web requests
- Explicit response allowlists instead of raw database objects
- Separate authentication flows for browser extension and device clients
- Rate limiting with Redis support
- Input validation and redirect restrictions
- Environment and secret separation
- Security headers and Cloudflare edge protection
- Audit-oriented handling of elevated operations
- Semgrep and secret scanning in PR validation

## Operating principle

Frontend visibility is never treated as authorization. Access control is enforced at API/controller boundaries, and production changes are reviewed and verified after deployment.
