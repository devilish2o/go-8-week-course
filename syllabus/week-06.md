# Week 6 — REST API and service architecture

**Daily session:** 30 minutes (5 min recall, 10 min study, 15 min coding).

## Daily targets

1. **17 Dec — HTTP server fundamentals**
   - Target: Implement /healthz and /version.
   - Study: https://gobyexample.com/http-servers

2. **18 Dec — Handlers and routing**
   - Target: Add /checks and /checks/{id}; keep handlers testable.
   - Study: https://go.dev/doc/articles/wiki/

3. **19 Dec — Request and response JSON**
   - Target: Decode, validate and encode payloads.
   - Study: https://go.dev/doc/tutorial/

4. **20 Dec — Middleware and server timeouts**
   - Target: Add request logging, test API-key middleware and server timeouts.
   - Study: https://pkg.go.dev/net/http

5. **21 Dec — Context propagation and graceful shutdown**
   - Target: Handle SIGINT/SIGTERM and shut down cleanly.
   - Study: https://gobyexample.com/context

6. **22 Dec — API integration tests**
   - Target: Use httptest for success, invalid input and timeout.
   - Study: https://pkg.go.dev/net/http/httptest

7. **23 Dec — Weekly review: local monitoring API**
   - Target: Expose /healthz and /checks; add curl examples and handler tests.
   - Study: https://go.dev/doc/tutorial/

## Weekly outcome
Expose the tool through a tested REST API.
