# Awesome Batch API Test Runner

A curated list of Batch API Test Runners, Collection Runners, and Load Testing tools for APIs.

---

## Sector Overview & Market Dynamics

The API testing and observability market is estimated at **$1.6B to $3.5B**, projected to reach over **$6B to $16B** at an 18–23% CAGR driven by microservices sprawl and automated CI/CD pipelines. The sector is **moderately fragmented** with high developer tool diversity (open-source frameworks alongside product-led growth startups), while enterprise spend is moderately concentrated among scaled QA and monitoring platform providers.

---

## SaaS Platforms

| Platform | Company Valuation / Revenue | Pricing | Free Tier Limit | Description |
|---|---|---|---|---|
| **Grafana Cloud k6** | Valuation: **$6.0B** (ARR: ~$600M) | Starting at **$19/month** (Grafana Cloud Pro platform fee + ~$0.15/VUh overages) | **500 Virtual User Hours (VUh)/month** forever; 10k active metrics series, 14-day test result retention | Managed cloud execution and distributed performance testing for k6 scripts. |
| **Postman** | Valuation: **$5.6B** (ARR: ~$171M–$313M) | Starting at **$14/user/month** (billed annually at $9/user/month for Solo, $19/user/month for Team) | **1 user**, **10,000 API calls/month**, up to 5 integrations, 50 Postbot AI credits | Industry-standard API client and automated collection runner (includes Newman CLI compatibility). |
| **BlazeMeter** | Revenue: **~$200M+** (Perforce Software) | Starting at **$99/month** (billed annually, or $149/mo billed monthly for Basic performance tier; API testing starts at $79/mo) | **50 concurrent virtual users**, **10 tests/month**, **20 min max duration**, 1 shared load generator, 1,000 API monitoring calls/month | Cloud load and API performance testing platform supporting JMeter, Taurus, and Selenium scripts. |

---

## Open-Source Test Runners & Load Tools

| Tool | License | Description |
|---|---|---|
| **Newman** | Apache-2.0 | Postman's CLI collection runner; executes collections directly in CI/CD pipelines with JUnit/HTML/JSON reporting. |
| **k6** | AGPL-3.0 | Modern, developer-centric load testing tool written in Go with JavaScript test scripting. |
| **Apache JMeter** | Apache-2.0 | Java-based performance and load testing framework supporting multiple protocols with rich reporting. |
| **Gatling** | Apache-2.0 | High-performance load testing tool written as code (Java, Kotlin, Scala, TypeScript/JavaScript) running on Netty. |
| **Locust** | MIT | Developer-friendly, Python-based distributed load testing tool with real-time web UI dashboard. |
| **Artillery** | MPL-2.0 | Cloud-native, distributed load and functional testing toolkit for HTTP, WebSocket, and gRPC with Playwright engine support. |
| **Tavern** | Apache-2.0 | Command-line tool and Python library for automated API testing using clear, concise YAML-defined test cases. |
| **REST Assured** | Apache-2.0 | Java domain-specific language (DSL) making REST service functional testing straightforward and expressive. |

