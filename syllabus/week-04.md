# Week 4 — Concurrency and networking

**Daily session:** 30 minutes (5 min recall, 10 min study, 15 min coding).

## Daily targets

1. **3 Dec — Goroutines**
   - Target: Launch independent checks and wait for completion.
   - Study: https://go.dev/tour/concurrency/1

2. **4 Dec — Channels**
   - Target: Send check results through channels to main.
   - Study: https://go.dev/tour/concurrency/2

3. **5 Dec — WaitGroups and worker pools**
   - Target: Bound concurrent URL checks.
   - Study: https://gobyexample.com/worker-pools

4. **6 Dec — Select, timeouts and cancellation**
   - Target: Use context.WithTimeout to stop slow checks.
   - Study: https://gobyexample.com/timeouts

5. **7 Dec — HTTP client**
   - Target: Request endpoints, inspect status and latency; set timeout.
   - Study: https://gobyexample.com/http-clients

6. **8 Dec — TCP and DNS basics**
   - Target: Use net.DialTimeout and net.LookupHost.
   - Study: https://pkg.go.dev/net

7. **9 Dec — Weekly review: concurrent endpoint checker**
   - Target: Check five owned/public endpoints concurrently with timeouts; do not scan networks.
   - Study: https://gobyexample.com/worker-pools

## Weekly outcome
Write concurrent network checks with timeouts.
