# hostwatch — Final Project Specification

## Goal
Build a small, safe Go infrastructure-monitoring application suitable for a portfolio demonstration.

## Functional scope
- Configured HTTP endpoint checks with explicit timeouts.
- Optional checks for an allowlist of local systemd services using read-only status commands.
- Bounded concurrent workers; no unbounded goroutine fan-out.
- Human-readable and JSON CLI output.
- HTTP API: /healthz and /checks.
- SQLite persistence for recent check results.
- ntfy alerts to a topic owned by the developer.
- Structured logs with no credentials or tokens.

## Suggested implementation milestones
1. Data model and fake checker.
2. Interfaces, validation and table-driven tests.
3. HTTP/TCP checks with contexts and bounded concurrency.
4. CLI flags, environment config, JSON and slog.
5. HTTP API plus httptest coverage.
6. SQLite history and ntfy notification.
7. Documentation, build and deployment rehearsal.

## Operational safety
- Develop under a home-directory project path and use a separate test directory.
- Run as an unprivileged user; never require root for normal checks.
- Do not scan networks or ports. Only check explicitly configured targets you own or are authorised to test.
- Service checks must be allowlisted and read-only.
- Do not alter existing nginx configuration or running services.
- Draft the systemd unit for review; do not enable it until deployment is separately approved.

## Definition of done
- gofmt clean; go test ./... passes.
- go test -race ./... passes.
- CLI produces readable and JSON output.
- API handlers have tests.
- Results persist and an opt-in ntfy test alert works.
- README explains architecture, configuration, security boundaries and demo commands.
