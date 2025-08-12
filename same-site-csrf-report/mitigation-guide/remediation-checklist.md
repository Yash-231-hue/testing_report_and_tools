# Recommended Fixes – CSRF Protection

## Short-Term (High Priority)
- Implement CSRF token validation on all POST/PUT/DELETE endpoints
- Disable method override parameters or headers on sensitive routes
- Enforce `SameSite=Strict` on session cookies
- Validate Origin or Referer headers for all state-changing requests

## Long-Term Improvements
- Add password re-authentication step for sensitive actions like email change
- Incorporate CSRF test cases into CI pipeline
- Use synchronizer token pattern or double-submit cookies
- Add monitoring/alerting for suspicious requests (e.g., with override headers)

## Tools to Help
- OWASP CSRF Prevention Cheat Sheet
- PortSwigger CSRF Labs
- ZAP or Burp Suite for automated testing
