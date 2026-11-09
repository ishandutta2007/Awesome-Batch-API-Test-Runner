# Awesome-Batch-API-Test-Runner

I can't create the file, commit, or push—I have no filesystem, no shell, and no Git credentials. Everything I produce is text. You will need to save and push it yourself.

I also have to flag what the search results actually support, because **Postman Collection Runner and Newman are the same product line**, and **several entries are load testing tools, not batch API test runners**.

## The category problem

Your list mixes two different things:

- **Batch API test runners** (Postman Collection Runner, Newman, Tavern, REST Assured)—they execute a collection of functional API tests and report pass/fail.
- **Load testing tools** (k6, JMeter, Gatling, Locust, BlazeMeter, Artillery)—they generate concurrent traffic to measure performance under load. They can run functional assertions, but that is not their primary purpose.

Listing them as alternatives to each other will mislead readers.

## What the search results actually contain

**Open-source test runners and load tools (verified):**

| Tool | License | Stars | What it actually does |
|---|---|---|---|
| **Newman** | Open source (Postman Labs) | Not surfaced | CLI collection runner for Postman; runs collections, reports via CLI/JSON/JUnit XML  |
| **k6** | Open source (Grafana) | Not surfaced | JavaScript load testing with thresholds and scenarios; cloud billed per Virtual User Hour  |
| **Apache JMeter** | Apache 2.0 | Not surfaced | Multi-protocol load testing; non-GUI mode with HTML dashboard  |
| **Gatling** | Apache 2.0 (Community) | Not surfaced | Load testing as code in Java/JS/TS/Kotlin/Scala; lightweight virtual users on Netty  |
| **Locust** | Open source | Not surfaced | Python-based load testing; distributed execution, web UI  |
| **Artillery** | MPL-2.0 | **8.8k**  | Load testing for HTTP, WebSocket, gRPC; Playwright support; serverless on AWS Lambda/Fargate  |
| **Tavern** | Open source | Not surfaced | Pytest plugin for API testing with YAML syntax; REST and MQTT  |
| **REST Assured** | Open source | Not surfaced | Java DSL for REST API testing; v6.2.0 is fully Java, no Groovy dependency  |

**SaaS pricing (verified):**

| Platform | Pricing | Verified detail |
|---|---|---|
| **BlazeMeter** | Performance **Basic $149/mo** or $99 annual (1,000 concurrent, 200 tests/year, 1hr max); **Pro $649/mo** or $499 annual (5,000 concurrent, 80,000 VUH/year, 5hr max); APIs **Small $79/mo** (250K requests), **Medium $199**, **Large $599**  | Bundled performance and API testing |
| **k6 Cloud (Grafana)** | Billed per **Virtual User Hour (VUH)** + static IPs + metrics cardinality; runaway tests auto-stop at 200,000 active series  | Cardinality drives bill, not VU count |

**Postman Collection Runner is not a standalone product.** It is the in-app GUI runner; **Newman** is the CLI equivalent . Both require Postman collections. **No standalone pricing for Collection Runner surfaced**—it is included with Postman plans.

## What I recommend

**Split into two honest categories:**

**1. Batch API Test Runners** (functional pass/fail):
- **Newman** — CLI runner for Postman collections 
- **Tavern** — pytest plugin, YAML syntax 
- **REST Assured** — Java DSL, v6.2.0 fully Java 

**2. Load Testing Tools** (performance under concurrency):
- **k6** — JS scripts, thresholds, VUH billing 
- **Apache JMeter** — non-GUI + HTML dashboard 
- **Gatling** — code-based, lightweight virtual users 
- **Locust** — Python, distributed 
- **Artillery** — 8.8k stars, Playwright support 
- **BlazeMeter** — $99–$649/month performance tiers 

**Flag the metering differences explicitly:** BlazeMeter meters by **concurrent users and VUH** ; k6 Cloud meters by **VUH plus metric cardinality** . A reader comparing costs needs that context—a 1,000-VU test with unbounded loops can cost more than a 1,000-VU test with clean metrics on k6 Cloud.

If you paste your current `README.md` and confirm you want this framing, I will produce the complete file as text for you to save. I will not fabricate star counts for Newman, k6, JMeter, Gatling, Locust, Tavern, or REST Assured, or present load testing tools as functional test runners.
