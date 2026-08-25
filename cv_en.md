# Riccardo Beninatto

📍 Treviso, Italy | 📞 340 958 5817 | ✉️ beninatto.riccardo@gmail.com  
🔗 [LinkedIn](https://www.linkedin.com/in/riccardo-beninatto-23444265/)

---

## 🎯 Professional Summary

14 years building software, most of them at TEXA. WPF and Windows Forms desktop applications, software for diagnostic devices on Windows CE, ASP.NET MVC web portals with Angular frontends, REST Web APIs, Azure cloud services, full-text search engines with Solr and ElasticSearch. Build, test and deploy pipelines on Azure DevOps, unit testing with MSTest, xUnit and Moq.

In 2024 I led the development of the build, installation and update system for the Garage Equipment division's software: 75,000+ devices across Europe, the US, Brazil, Japan, China, Korea and Australia. Since April 2022 I formed and led a three-person R&D development team.

Currently at Eurogroup, working on a .NET 8 microservice system with RabbitMQ, MongoDB and SQL Server. I built the Azure DevOps pipelines from scratch and introduced the observability stack with Grafana, Loki and Prometheus.

In my own time I build Risurge, a SaaS for athletes that can also be operated by talking to an AI agent. .NET 10, Angular 22, Azure, Anthropic API, CI/CD on GitHub Actions with ~860 tests running in parallel.

---

## 💼 Professional Experience

### Senior Software Developer
**Eurogroup S.p.A.** — Silea (TV)  
📅 December 2025 – Present

- Took over an existing **microservice system**, responsible for its maintenance and evolution: asynchronous communication via **RabbitMQ (MQTT)**, polyglot persistence on **MongoDB** and **SQL Server**
- Applied **resilience patterns** (retry, circuit breaker, timeout, bulkhead) to inter-service communication
- Built the **Azure DevOps** build, test and deploy pipelines from scratch, with secrets managed through pipeline libraries
- Introduced the **observability stack** — **Grafana**, **Loki** and **Prometheus**, run as **Docker** containers
- Introduced **AI coding agents**, now used across the group to accelerate the digitalisation of internal processes
- Applied **Clean Architecture** and **SOLID** when extending the codebase, with input validation and **OWASP Top 10** mitigations

**Tech stack:** C# .NET 8, RabbitMQ, MongoDB, SQL Server, Docker, Azure DevOps, Grafana, Loki, Prometheus, MSTest, xUnit

---

### Senior Software Developer
**Stesi S.r.l.** — San Fior (TV)  
📅 July 2025 – December 2025

- Development of an **EDI interfacing system** between the corporate database and external partners via an AS2 server, in the **WMS** domain, with a focus on reliability and data-flow traceability

**Tech stack:** C# .NET, SQL Server, EDI/AS2

---

### Senior Software Developer & Team Lead
**TEXA S.p.A.** — Monastier di Treviso  
📅 November 2011 – July 2025 *(Team Lead since April 2022)*

- Proposed and designed the replacement of the division's **InstallShield**-based setup system with a **VS-installer-like** system, covering package production, update frontend and update logic. Owned it from architecture to global rollout
- The system manages over **75,000 devices** for vehicle diagnostics across Europe, the United States, Brazil, Japan, China, Korea and Australia
- Full-text search engines on **Apache Solr** (~70,000 documents) and **ElasticSearch** (several million records for statistical analysis)
- **Azure** cloud services (WebApp, Functions, SQL Database, Service Bus, Application Insights, Key Vault) and **REST Web APIs** with ASP.NET Core
- **ASP.NET MVC 5** web portal with **Angular/TypeScript** frontend, **WPF** and **Windows Forms** desktop applications, software running on **Windows CE** devices for diagnostics
- Build and delivery pipelines on **Azure DevOps** and introduction of **unit testing** (MSTest, xUnit, Moq) on critical projects
- Since April 2022: formed and led a **three-person R&D development team**, responsible for planning, code review and delivery

**Tech stack:** C# .NET/.NET Core, Azure, ASP.NET MVC/Web API, Angular, TypeScript, ElasticSearch, Solr, WPF, WCF, Azure DevOps, Git

**Sector:** Automotive / Vehicle Diagnostics

---

## 🚀 Personal Projects

### Risurge — SaaS platform for training
**Personal full-stack project** — actively developed *(early access)*  
📅 2026 – Present

Web application for gym training management, aimed at athletes: workout plan editor, session execution, history, analytics and periodic check-ins. **The whole application can be operated by talking to an AI agent**: the GUI and the AI coach are two equivalent paths to the same features. Designed, developed and released single-handedly, from architecture to deployment.

- **AI-first, agentic interaction**: a custom **agent loop** with **tool calling** (~40 in-process tools, no MCP) lets the model *actually operate* the app on the user's behalf — create, edit and activate plans, build periodised programs, manage the exercise catalogue, log one-rep maxes and body weight, correct the training diary, update volume landmarks, read profile, history and metrics
- The coach is not a bolt-on chatbot: every tool is **scoped per athlete** and carries its own domain **guardrails** (patch semantics on corrections, explicit confirmation before significant changes, clarification requests when the ask is ambiguous)
- **Layered architecture** (Contracts / DataAccess / Services / Server) with **SOLID** principles applied systematically and automated CI guards against duplication of domain decisions
- **ASP.NET Core (.NET 10)** backend with REST Web API, **JWT** authentication, Swagger and provider-aware data access (**Azure SQL** in production, **SQLite** in test/dev)
- **Angular 22** frontend in TypeScript, **PWA** with service worker, 6-language localisation with Transloco and a token-based design system for light/dark themes
- Integration with **Anthropic AI models** also for smart training-plan import, conversational memory with compaction and proactive reports, with **end-to-end cost control**: per-subscription spend caps, a single chokepoint that refuses calls without a declared payer, metering, model triage and budget gates
- **Stripe billing** (entitlements and feature gating), email notifications via MailKit
- **Azure deployment** (App Service, Azure SQL, Application Insights) with **CI/CD on GitHub Actions** with **OIDC** authentication to Azure, automated versioning and changelog via **release-please**, separate TEST and PROD environments
- **~860 unit/integration tests** (MSTest) running in parallel, including guard tests covering architecture, type documentation and uniqueness of business decisions
- Focus on **privacy and GDPR compliance**: versioned and revocable consents, health data (art. 9) under explicit consent, genuine account deletion
- Development assisted by **AI coding agents** (Claude Code, GitHub Copilot) with project guidelines codified for the model. I take every architecture decision myself and run periodic structural reviews of the codebase

**Tech stack:** C# .NET 10, ASP.NET Core, Angular 22, TypeScript, Azure SQL, SQLite, Azure App Service, Application Insights, Stripe, Anthropic API, GitHub Actions, MSTest, Astro (landing site)

---

## 🛠️ Technical Skills

### Languages & Frameworks
| Area | Technologies |
|---|---|
| **Backend** | C# .NET 8 / .NET Core, ASP.NET Core Web API, ASP.NET MVC, WCF |
| **Frontend** | Angular, TypeScript, JavaScript, jQuery, Bootstrap, Google Material |
| **Desktop** | WPF, Windows Forms, Windows CE |
| **Scripting/Other** | NSIS, XSLT, JSON |

### Architecture & Patterns
| Area | Skills |
|---|---|
| **Architecture** | Clean Architecture, Domain-Driven Design (DDD), Microservices, Monolith |
| **Patterns** | CQRS (MediatR), Repository, Abstract Factory, Dependency Injection, Observer |
| **Principles** | SOLID, DRY, KISS, Separation of Concerns |
| **Messaging** | RabbitMQ, Azure Service Bus, Pub/Sub pattern |
| **IoT Protocols** | MQTT |
| **Resilience** | Retry, Circuit Breaker, Timeout, Bulkhead |

### Cloud & DevOps
| Area | Technologies |
|---|---|
| **Azure** | WebApp, Functions, SQL Database, Service Bus, Application Insights, Key Vault |
| **Containers** | Docker, Docker Compose |
| **CI/CD** | Azure DevOps Pipelines, Git, branching strategies |
| **Monitoring** | Application Insights, Grafana, Loki, Prometheus, structured logging |

### Database & Search
| Area | Technologies |
|---|---|
| **Relational** | SQL Server, Azure SQL, SQLite |
| **NoSQL** | MongoDB |
| **Full-text Search** | ElasticSearch, Apache Solr |

### Testing & Quality
| Area | Technologies |
|---|---|
| **Unit Testing** | MSTest, xUnit, Moq, FluentAssertions |
| **Approach** | Test-driven development, systematic code reviews |
| **AI & Productivity** | Claude Code, GitHub Copilot |

### Security
| Area | Skills |
|---|---|
| **Fundamentals** | OWASP Top 10, input validation, secure authentication/authorisation |
| **Azure** | Key Vault, Managed Identity, HTTPS enforcement |
| **Secrets & Credentials** | Secure management of secrets, passwords and API keys (Key Vault, protected env vars, no hardcoding) |

---

## 🎓 Education

### IT Technician Diploma (79/100)
**I.T.I.S. Max Planck** — Lancenigo, Villorba  
📅 2006 – 2011

---

## 🌐 Languages

| Language | Level |
|---|---|
| 🇮🇹 Italian | Native |
| 🇬🇧 English | B2 (reading, speaking, writing) |

---

## 🌱 Interests

Strength training, gardening, hiking in the Dolomites.
