<table><tr>
<td markdown="1">

# Riccardo Beninatto

📍 Via 11 Febbraio, 2, 31030, Breda di Piave, Treviso | 📞 340 958 5817 | ✉️ beninatto.riccardo@gmail.com  
🔗 [LinkedIn](https://www.linkedin.com/in/riccardo-beninatto-23444265/) | 🇮🇹 Italian | 🇬🇧 English B2  
Born 03/01/1992 | Gender M | Nationality Italian | Driving Licence A, B

</td>
<td><img src="Foto CV.jpg" alt="Riccardo Beninatto" width="150"></td>
</tr></table>

---

## 🎯 Professional Summary

Graduated as an IT Technician from I.T.I.S. Max Planck in Villorba, I began my professional career at TEXA as a C# .NET desktop application developer. Over the years I took on roles of increasing responsibility, eventually becoming coordinator of a development team, with the goal of optimising internal processes for corporate data management and overseeing strategic projects. Throughout 2024, I led the development of an innovative system for the production, installation and update of software for the Garage Equipment division, distributed globally to support mechanical workshops in vehicle diagnostics.

During my experience at TEXA I gained hands-on knowledge of Agile methodologies — in particular the Scrum framework — major architectural patterns such as DDD and Abstract Factory, and SOLID principles.

**Current Role:** Software Developer

### 🔭 Future Prospects

I am looking for roles as **Backend Architect** or **.NET Tech Lead**, where I can leverage the experience I have gained in developing .NET C# solutions, both on-premise and on-cloud, working on new, dynamic and challenging projects.

---

## 💼 Professional Experience

### Senior Software Developer
**Eurogroup S.p.A.** — Silea (TV)  
📅 December 2025 – Present

- Design and development of a **microservices system** with asynchronous communication via **RabbitMQ (MQTT)**
- Integration with **MongoDB** and **SQL Server** databases in a polyglot architecture
- Implementation of **resilience patterns** (retry, circuit breaker)
- Containerisation of services with **Docker** and orchestration in multi-container environments with **Docker Compose**
- Configuration of **Azure DevOps pipelines** for automated delivery (**build/test/deploy**), without Continuous Deployment
- Application of **Clean Architecture** and **SOLID** principles to ensure maintainability and testability
- Adoption of **software security practices**: secure management of secrets and credentials via **Azure Key Vault**, HTTPS enforcement, input validation and prevention of common vulnerabilities (OWASP Top 10)
- Use of **AI coding agents** (e.g. GitHub Copilot, OpenCode) to increase productivity and code quality

**Tech stack:** C# .NET 8, RabbitMQ, MongoDB, SQL Server, Docker, Azure DevOps, MSTest, xUnit

---

### Software Analyst Developer
**Stesi S.r.l.** — San Fior (TV)  
📅 July 2025 – December 2025

- Initial onboarding phase focused on secondary development activities to acquire domain-specific knowledge.
- Development of an **EDI interfacing system** between the corporate database and external partners via an AS2 server
- Analysis and acquisition of the **WMS (Warehouse Management System)** domain
- Development of integration components with a focus on reliability and data-flow traceability
- Company change to Eurogroup due to a role misaligned with my skills and the technical path described during interviews

**Tech stack:** C# .NET, SQL Server, EDI/AS2

---

### Team Leader & Senior Developer
**TEXA S.p.A.** — Monastier di Treviso  
📅 April 2022 – July 2025 *(Team Leader)*  
📅 November 2011 – July 2025 *(Developer, then Analyst Developer)*

**Leadership & Coordination (2022–2025):**
- Creation and management of a **3-person R&D development team** with direct responsibility for planning, code review and delivery
- Led the development of an **innovative system for the production, installation and software update** of the Garage Equipment division, distributed **globally** for vehicle diagnostics, managing over **75,000 devices** in **Europe, USA, South America (Brazil), Asia (Japan, China, Korea) and Australia**
- Technical supervision of resources and mentoring of junior developers
- Adoption and promotion of **Agile/Scrum** methodologies within the team
- Adoption of **software security practices**: secure management of secrets and passwords via **Azure Key Vault**, Managed Identity, HTTPS enforcement and vulnerability prevention (OWASP Top 10)
- Use of **AI coding agents** (e.g. GitHub Copilot) to increase team productivity and improve code quality

**Development & Architecture (2011–2025):**
- Development and maintenance of software for managing a **corporate database in a proprietary format**
- Setup development via **NSIS**
- Design and development of **Azure cloud services**: WebApp, Azure Functions, SQL Database, Azure Service Bus, Application Insights, Key Vault
- Development of **RESTful Web APIs** with ASP.NET Core and WCF services
- Development of **ASP.NET MVC 5** web portal with **Angular/TypeScript** frontend
- Implementation of **full-text search engines** based on **Apache Solr** (approx. **70,000 documents**) and **ElasticSearch** (several **million records** for statistical analysis)
- Development of **WPF** and **Windows Forms** desktop applications for corporate data management
- Development of embedded **Windows CE** software for diagnostic devices
- Implementation of **unit tests** with **MSTest**, **xUnit** and **Moq** to support code quality on critical projects (from 2020)
- Creation of **Azure DevOps pipelines** for automated delivery (**build/test/deploy**), without Continuous Deployment
- Use of **AI coding agents** (e.g. GitHub Copilot) to increase productivity and accelerate development
- Development of automated data processing workflows with scheduling and integrated notifications
- Supervision of internal projects for **data production for business purposes**
- Management of projects related to major **business areas**

**Tech stack:** C# .NET/.NET Core, Azure (WebApp, Functions, Service Bus, SQL, App Insights, Key Vault), ASP.NET MVC/Web API, Angular, TypeScript, ElasticSearch, Solr, WPF, WCF, MSTest, xUnit, Moq, Azure DevOps, Git

**Sector:** Automotive / Vehicle Diagnostics

---

## 🚀 Personal Projects

### Risurge — SaaS platform for training and coaching
**Personal full-stack project** — actively developed *(early access)*  
📅 2025 – Present

Web application for gym training management, aimed at both athletes and personal trainers: workout plan editor, session execution, history, analytics and periodic check-ins. **The whole application can be operated by talking to an AI agent**: the GUI and the AI coach are two equivalent paths to the same features. Designed, developed and released single-handedly, from architecture to deployment.

- **AI-first, agentic interaction**: a custom **agent loop** with **tool calling** (~40 in-process tools, no MCP) lets the model *actually operate* the app on the user's behalf — create, edit and activate plans, build periodised programs, manage the exercise catalogue, log one-rep maxes and body weight, correct the training diary, update volume landmarks, read profile, history and metrics
- The coach is not a bolt-on chatbot: every tool is **scoped per athlete** and carries its own domain **guardrails** (patch semantics on corrections, explicit confirmation before significant changes, clarification requests when the ask is ambiguous)
- **Layered architecture** (Contracts / DataAccess / Services / Server) with **SOLID** principles applied systematically and automated CI guards against duplication of domain decisions
- **ASP.NET Core (.NET 10)** backend with REST Web API, **JWT** authentication, Swagger and provider-aware data access (**Azure SQL** in production, **SQLite** in test/dev)
- **Angular 22** frontend in TypeScript, **PWA** with service worker, 6-language localisation with Transloco and a token-based design system for light/dark themes
- Integration with **Anthropic AI models** also for smart training-plan import, conversational memory with compaction and proactive reports, with **end-to-end cost control**: per-subscription spend caps, a single chokepoint that refuses calls without a declared payer, metering, model triage and budget gates
- **Stripe billing** (athlete and trainer plans, entitlements and feature gating), email notifications via MailKit
- **Azure deployment** (App Service, Azure SQL, Application Insights) with **CI/CD on GitHub Actions**, secretless OIDC authentication, automated versioning and changelog via **release-please**, separate TEST and PROD environments
- **~860 unit/integration tests** (MSTest) running in parallel, including guard tests covering architecture, type documentation and uniqueness of business decisions
- Focus on **privacy and GDPR compliance**: versioned and revocable consents, health data (art. 9) under explicit consent, genuine account deletion
- Development assisted by **AI coding agents** (Claude Code, GitHub Copilot) with project guidelines codified for the model

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
| **Monitoring** | Application Insights, structured logging |

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
| **AI & Productivity** | GitHub Copilot, AI coding agents |

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

## 🤝 Soft Skills

**Communication skills:**
- Strong listening skills and ability to empathise with others.

**Professional skills:**
- Quick learner and flexible. Good organisational ability in planning activities based on established priorities.
- From April 2022 I built my own working group within the R&D department, with the aim of improving development and project management activities.

---

## 🌱 Other Interests

- Gardening, fitness and nutrition

---

## 🏷️ Keywords

`.NET` `C#` `Azure` `Microservices` `Clean Architecture` `DDD` `CQRS` `RabbitMQ` `Docker` `SQL Server` `MongoDB` `ElasticSearch` `Angular` `TypeScript` `CI/CD` `Azure DevOps` `GitHub Copilot` `MSTest` `xUnit` `OWASP` `Team Leadership` `Agile` `Scrum` `.NET 10` `GitHub Actions` `Stripe` `SaaS` `AI Agent` `Tool Calling` `LLM Integration`

---

## 🔎 Extra Training (non-IT)

- **16-hour seminar on nutrition and sports supplementation** — Private instructor Marco Venturi (2015) — San Polo di Piave Municipal Library
- **AutoCAD 2D/3D Designer** — Pragma (2013–2014) — Grade: 28/30
- **BodyBuilding & Fitness Instructor Level 1** — C.S.E.N. (2014) — Anatomy, Physiology and Basic Biomechanics — Top marks

---

*I authorise the processing of my personal data pursuant to Legislative Decree 30 June 2003, No. 196 "Code regarding the protection of personal data".*
