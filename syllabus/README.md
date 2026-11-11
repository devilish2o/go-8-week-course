# Complete 56-Day Syllabus

**Dates:** 12 Nov 2026 – 6 Jan 2027 · **Pace:** 30 minutes daily · **Timezone:** America/Toronto  
Daily routine: 5 min recall, 10 min lesson, 15 min hands-on coding.

## Week 1 — Getting started and fundamentals
1. **12 Nov — Install Go/toolchain.** Run `go version`, `go env`, `go help`; create and run Hello World. [Getting started](https://go.dev/doc/tutorial/getting-started)
2. **13 Nov — Packages/imports/main.** Split a small app into main and helper package. [Tour: packages](https://go.dev/tour/basics/1)
3. **14 Nov — Variables, constants, types.** Build MB↔GB and Celsius↔Fahrenheit converters. [Tour: basic types](https://go.dev/tour/basics/11)
4. **15 Nov — Functions/multiple returns.** Write conversions and disk percentage; return value plus error. [Functions](https://gobyexample.com/functions)
5. **16 Nov — Control flow.** Practise if/switch/for/range/defer; build a repeating menu. [Flow control](https://go.dev/tour/flowcontrol/1)
6. **17 Nov — Strings, formatting, input.** Use fmt, Scanner, strconv; accept a hostname and print a report. [String functions](https://gobyexample.com/string-functions)
7. **18 Nov — Review mini CLI.** Three commands, validation, useful errors, gofmt. [CLI arguments](https://gobyexample.com/command-line-arguments)

## Week 2 — Data structures, pointers and organisation
8. **19 Nov — Arrays/slices.** Store and edit service names. [Slices](https://go.dev/tour/moretypes/7)
9. **20 Nov — Maps.** Model service→status and hostname→latency; practise comma-ok. [Maps](https://go.dev/tour/moretypes/19)
10. **21 Nov — Structs.** Define Host, CheckResult and Service. [Structs](https://go.dev/tour/moretypes/1)
11. **22 Nov — Pointers.** Update a Host through a pointer. [More types](https://go.dev/tour/moretypes/1)
12. **23 Nov — Methods/receivers.** Add methods; compare value and pointer receivers. [Methods](https://go.dev/tour/methods/1)
13. **24 Nov — Modules/packages.** Use go mod init; split internal/checks and internal/report. [Create a module](https://go.dev/doc/tutorial/create-module)
14. **25 Nov — Review host inventory.** Combine structs, slices, maps, methods and packages. [Structs](https://gobyexample.com/structs)

## Week 3 — Interfaces, errors and testing
15. **26 Nov — Interfaces.** Define Checker; implement fake and URL-checker stub. [Tour: interfaces](https://go.dev/tour/methods/9)
16. **27 Nov — Implicit interfaces/composition.** Add Reporter with text and JSON implementations. [Effective Go](https://go.dev/doc/effective_go)
17. **28 Nov — Error handling.** Return errors, wrap with fmt.Errorf and %w. [Errors](https://gobyexample.com/errors)
18. **29 Nov — Custom errors/validation.** Validate hostnames, ports and thresholds. [Custom errors](https://gobyexample.com/custom-errors)
19. **30 Nov — Unit tests.** Write table-driven tests for calculations and validation. [Add a test](https://go.dev/doc/tutorial/add-a-test)
20. **1 Dec — Coverage/race detector.** Run go test ./..., -cover and -race; fix an introduced bug. [Go command](https://go.dev/cmd/go/)
21. **2 Dec — Review tested checker.** Two Checker implementations, validation, errors and tests; commit milestone. [Testing](https://gobyexample.com/testing-and-benchmarking)

## Week 4 — Concurrency and networking
22. **3 Dec — Goroutines.** Launch independent checks and wait for completion. [Goroutines](https://go.dev/tour/concurrency/1)
23. **4 Dec — Channels.** Send check results back to main. [Channels](https://go.dev/tour/concurrency/2)
24. **5 Dec — WaitGroups/worker pools.** Bound concurrent URL checks. [Worker pools](https://gobyexample.com/worker-pools)
25. **6 Dec — Select/timeouts/cancellation.** Use context.WithTimeout to stop slow checks. [Timeouts](https://gobyexample.com/timeouts)
26. **7 Dec — HTTP client.** Request endpoints, inspect status and latency; set timeout. [HTTP clients](https://gobyexample.com/http-clients)
27. **8 Dec — TCP/DNS.** Use net.DialTimeout and net.LookupHost. [net package](https://pkg.go.dev/net)
28. **9 Dec — Review concurrent checker.** Check five owned/public endpoints concurrently with timeouts. Do not scan networks or ports you do not own. [Worker pools](https://gobyexample.com/worker-pools)

## Week 5 — JSON, files, CLI and logging
29. **10 Dec — JSON.** Encode/decode CheckResult with struct tags. [Go tutorials](https://go.dev/doc/tutorial/)
30. **11 Dec — Files.** Save/load JSON; handle missing files and permissions. [Reading files](https://gobyexample.com/reading-files)
31. **12 Dec — CLI flags.** Add --url, --timeout, --format, --output. [Command-line flags](https://gobyexample.com/command-line-flags)
32. **13 Dec — Environment/config.** Define precedence: flags, environment, defaults. [Environment variables](https://gobyexample.com/environment-variables)
33. **14 Dec — Structured logging.** Use log/slog; never log secrets. [log/slog](https://pkg.go.dev/log/slog)
34. **15 Dec — Tickers/periodic work.** Run checks repeatedly and stop cleanly. [Tickers](https://gobyexample.com/tickers)
35. **16 Dec — Review first usable CLI.** Combine config, concurrency, JSON and slog into hostwatch.

## Week 6 — REST API and service architecture
36. **17 Dec — HTTP server.** Implement /healthz and /version. [HTTP servers](https://gobyexample.com/http-servers)
37. **18 Dec — Handlers/routing.** Add /checks and /checks/{id}; keep handlers testable. [Writing web apps](https://go.dev/doc/articles/wiki/)
38. **19 Dec — JSON requests/responses.** Decode, validate and encode payloads. [Go tutorials](https://go.dev/doc/tutorial/)
39. **20 Dec — Middleware/timeouts.** Request logging, test API-key middleware, server timeouts. [net/http](https://pkg.go.dev/net/http)
40. **21 Dec — Context/graceful shutdown.** Handle SIGINT/SIGTERM and shut down cleanly. [Context](https://gobyexample.com/context)
41. **22 Dec — API integration tests.** Use httptest for success, invalid input and timeout. [httptest](https://pkg.go.dev/net/http/httptest)
42. **23 Dec — Review local API.** Expose /healthz and /checks; add curl examples and handler tests.

## Week 7 — Persistence, Linux and notifications
43. **24 Dec — Database concepts.** Design a small check-history table. [Database access](https://go.dev/doc/tutorial/database-access)
44. **25 Dec — SQLite integration.** Use database/sql; create table and insert/read results. [Database access](https://go.dev/doc/tutorial/database-access)
45. **26 Dec — Linux processes.** Safely call systemctl is-active for a known service. [Spawning processes](https://gobyexample.com/spawning-processes)
46. **27 Dec — Disk/filesystem checks.** Use os.Stat and safe, documented APIs/commands. [os package](https://pkg.go.dev/os)
47. **28 Dec — ntfy notifications.** POST to your own topic; read topic from environment. [ntfy publish](https://docs.ntfy.sh/publish/)
48. **29 Dec — Security/dependency audit.** Validate input, timeouts, least privilege and dependencies. [govulncheck](https://go.dev/doc/tutorial/govulncheck)
49. **30 Dec — Review end-to-end.** Endpoint/service checks, SQLite, API status and test ntfy alert; read-only.

## Week 8 — Production polish and deployment
50. **31 Dec — Project structure.** Review packages, naming, interfaces and errors. [Effective Go](https://go.dev/doc/effective_go)
51. **1 Jan — Operational modes/config.** One-shot and periodic modes; validate startup config. [Environment variables](https://gobyexample.com/environment-variables)
52. **2 Jan — Observability.** Structured logs, counters and durations. [Go diagnostics](https://go.dev/doc/diagnostics)
53. **3 Jan — Build/cross-compile.** Build Linux binary; inspect with file/ldd. [Go command](https://go.dev/cmd/go/)
54. **4 Jan — Deployment rehearsal.** Test directory on Debian VPS as normal user; no existing service/nginx changes.
55. **5 Jan — systemd design.** Draft an unprivileged unit with restart policy and restricted permissions; review only. [systemd.service](https://www.freedesktop.org/software/systemd/man/latest/systemd.service.html)
56. **6 Jan — Final demo.** Tests, race detector, build, CLI/API/history/ntfy demo; document architecture and lessons.

## Final project — hostwatch
Build a small Go infrastructure-monitoring app:
- Check a small explicitly configured set of HTTP endpoints with timeouts.
- Optionally inspect an allowlist of local systemd services using read-only status commands.
- Use bounded concurrency; provide human-readable and JSON output.
- Expose /healthz and /checks over HTTP.
- Persist recent results in SQLite and send alerts to your own ntfy topic.
- Log useful operational information without exposing secrets.

**Safety boundary:** develop in your home directory and a separate test directory. Do not run as root, scan networks, change existing nginx configuration or modify existing services. The systemd unit remains a draft until you explicitly choose to deploy it.

## Completion checklist
- [ ] Create/run a Go module independently.
- [ ] Understand structs, methods, interfaces, pointers and errors.
- [ ] Write table-driven tests.
- [ ] Use goroutines, channels, contexts and timeouts safely.
- [ ] Build a CLI and HTTP API.
- [ ] Read/write JSON and persist data.
- [ ] Explain and demonstrate hostwatch.
