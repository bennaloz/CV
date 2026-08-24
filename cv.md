<table><tr>
<td>

# Riccardo Beninatto

📍 Via 11 Febbraio, 2, 31030, Breda di Piave, Treviso | 📞 340 958 5817 | ✉️ beninatto.riccardo@gmail.com  
🔗 [LinkedIn](https://www.linkedin.com/in/riccardo-beninatto-23444265/) | 🇮🇹 Italiano | 🇬🇧 Inglese B2  
Nato il 03/01/1992 | Sesso M | Nazionalità Italiano | Patente A, B

</td>
<td><img src="Foto CV.jpg" alt="Riccardo Beninatto" width="150"></td>
</tr></table>

---

## 🎯 Sintesi Professionale

Sviluppo software da 14 anni, quasi tutti in TEXA. Applicazioni desktop WPF e Windows Forms, software per dispositivi diagnostici su Windows CE, portali web ASP.NET MVC con frontend Angular, Web API REST, servizi cloud su Azure, motori di ricerca full-text con Solr ed ElasticSearch. Pipeline di build, test e deploy su Azure DevOps e unit test con MSTest, xUnit e Moq.

Nel 2024 ho guidato lo sviluppo del sistema di produzione, installazione e aggiornamento del software della divisione Garage Equipment: oltre 75.000 dispositivi tra Europa, Stati Uniti, Brasile, Giappone, Cina, Corea e Australia. Da aprile 2022 ho creato e coordinato un team di tre sviluppatori in R&D.

Oggi in Eurogroup lavoro su un sistema a microservizi in .NET 8 con RabbitMQ, MongoDB e SQL Server. Ho creato da zero le pipeline Azure DevOps e introdotto lo stack di osservabilità con Grafana, Loki e Prometheus.

Nel tempo libero sviluppo Risurge, SaaS per atleti utilizzabile anche conversando con un agente AI. .NET 10, Angular 22, Azure, Anthropic API, CI/CD su GitHub Actions con ~860 test in parallelo.

---

## 💼 Esperienza Professionale

### Senior Software Developer
**Eurogroup S.p.A.** — Silea (TV)  
📅 Dicembre 2025 – Presente

- Subentrato su un **sistema a microservizi** esistente, di cui curo manutenzione ed evoluzione: comunicazione asincrona via **RabbitMQ (MQTT)**, persistenza poliglotta su **MongoDB** e **SQL Server**
- Applicazione di pattern di **resilienza** (retry, circuit breaker, timeout, bulkhead) alla comunicazione tra servizi
- Creazione da zero delle **pipeline Azure DevOps** per build, test e deploy, con segreti gestiti tramite pipeline library
- Introduzione dello **stack di osservabilità** (**Grafana**, **Loki**, **Prometheus**) tramite container **Docker**
- Applicazione di **Clean Architecture** e principi **SOLID** nell'estensione del codebase, input validation e prevenzione **OWASP Top 10**
- Ho introdotto l'uso dei **coding agent AI**, oggi utilizzati nel gruppo per accelerare la digitalizzazione dei processi interni

**Tech stack:** C# .NET 8, RabbitMQ, MongoDB, SQL Server, Docker, Azure DevOps, Grafana, Loki, Prometheus, MSTest, xUnit

---

### Senior Software Developer
**Stesi S.r.l.** — San Fior (TV)  
📅 Luglio 2025 – Dicembre 2025

- Sviluppo di un sistema di **interfacciamento EDI** tra il database aziendale e partner esterni tramite server AS2, in dominio **WMS**, con focus su affidabilità e tracciabilità dei flussi dati

**Tech stack:** C# .NET, SQL Server, EDI/AS2

---

### Senior Software Developer & Team Lead
**TEXA S.p.A.** — Monastier di Treviso  
📅 Novembre 2011 – Luglio 2025 *(Team Lead da aprile 2022)*

- Ho proposto e progettato la sostituzione del sistema di setup della divisione basato su **InstallShield** con un sistema **VS-installer-like**, comprensivo di produzione pacchetti, frontend di aggiornamento e logiche di update. Seguito dall'architettura al rollout globale
- Il sistema gestisce oltre **75.000 dispositivi** per la diagnostica veicolare in Europa, Stati Uniti, Brasile, Giappone, Cina, Corea e Australia
- Motori di ricerca full-text su **Apache Solr** (~70.000 documenti) ed **ElasticSearch** (alcuni milioni di record per analisi statistiche)
- Servizi cloud **Azure** (WebApp, Functions, SQL Database, Service Bus, Application Insights, Key Vault) e **Web API REST** con ASP.NET Core
- Portale web **ASP.NET MVC 5** con frontend **Angular/TypeScript**, applicazioni desktop **WPF** e **Windows Forms**, software su dispositivi **Windows CE** per la diagnostica
- Pipeline di build e delivery su **Azure DevOps** e introduzione degli **unit test** (MSTest, xUnit, Moq) sui progetti critici
- Da aprile 2022: creazione e coordinamento di un **team di 3 sviluppatori in R&D**, con responsabilità su pianificazione, code review e delivery

**Tech stack:** C# .NET/.NET Core, Azure, ASP.NET MVC/Web API, Angular, TypeScript, ElasticSearch, Solr, WPF, WCF, Azure DevOps, Git

**Settore:** Automotive / Diagnostica veicolare

---

## 🚀 Progetti Personali

### Risurge — Piattaforma SaaS per allenamento e coaching
**Progetto personale full-stack** — in sviluppo attivo *(early access)*  
📅 2026 – Presente

Applicazione web per la gestione dell'allenamento in palestra, rivolta agli atleti: editor di schede, esecuzione della seduta, storico, analisi e check-in periodici. **L'intera applicazione è utilizzabile conversando con un agente AI**: l'interfaccia grafica e il coach AI sono due strade equivalenti sulle stesse funzionalità. Progettato, sviluppato e rilasciato in autonomia, dall'architettura al deploy.

- **Interazione AI-first, agentica**: un **agent loop** proprietario con **tool calling** (~40 tool in-process, senza MCP) permette al modello di *operare davvero* nell'app al posto dell'utente — creare, modificare e attivare schede, costruire programmi periodizzati, gestire il catalogo esercizi, registrare massimali e peso, correggere il diario, aggiornare i landmark di volume, leggere profilo, storico e metriche
- Il coach non è un chatbot bolt-on: ogni tool è **scopato per-atleta** e ha i propri **guardrail** di dominio (semantica a patch sulle correzioni, richiesta di conferma prima delle modifiche importanti, chiarimento esplicito quando la richiesta è ambigua)
- **Architettura a layer** (Contracts / DataAccess / Services / Server) con principi **SOLID** applicati in modo sistematico e guardie automatiche in CI contro la duplicazione delle decisioni di dominio
- Backend **ASP.NET Core (.NET 10)** con Web API REST, autenticazione **JWT**, Swagger e accesso dati **provider-aware** (**Azure SQL** in produzione, **SQLite** in test/dev)
- Frontend **Angular 22** in TypeScript, **PWA** con service worker, multilingua (6 lingue) con Transloco e design system a token per tema chiaro/scuro
- Integrazione con **modelli AI Anthropic** anche per import intelligente delle schede di allenamento, memoria conversazionale con compattazione e report proattivi, con **controllo dei costi end-to-end**: tetti di spesa per abbonamento, chokepoint unico che rifiuta chiamate senza pagatore dichiarato, metering, triage del modello e budget gate
- **Billing con Stripe** (piani atleta e trainer, entitlement e gating delle funzionalità), notifiche email via MailKit
- **Deploy su Azure** (App Service, Azure SQL, Application Insights) con **CI/CD su GitHub Actions** con autenticazione a Azure via **OIDC**, versionamento automatico e changelog con **release-please**, ambienti TEST e PROD separati
- **~860 unit/integration test** (MSTest) eseguiti in parallelo, con test-guardia che presidiano architettura, documentazione dei tipi e unicità delle decisioni di business
- Attenzione a **privacy e compliance GDPR**: consensi versionati e revocabili, dati sanitari (art. 9) sotto consenso esplicito, cancellazione reale dell'account
- Sviluppo assistito da **coding agents AI** (Claude Code, GitHub Copilot) con linee guida di progetto codificate per il modello

**Tech stack:** C# .NET 10, ASP.NET Core, Angular 22, TypeScript, Azure SQL, SQLite, Azure App Service, Application Insights, Stripe, Anthropic API, GitHub Actions, MSTest, Astro (sito vetrina)

---

## 🛠️ Competenze Tecniche

### Linguaggi & Framework
| Area | Tecnologie |
|---|---|
| **Backend** | C# .NET 8 / .NET Core, ASP.NET Core Web API, ASP.NET MVC, WCF |
| **Frontend** | Angular, TypeScript, JavaScript, jQuery, Bootstrap, Google Material |
| **Desktop** | WPF, Windows Forms, Windows CE |
| **Scripting/Altri** | NSIS, XSLT, JSON |

### Architettura & Pattern
| Area | Competenze |
|---|---|
| **Architettura** | Clean Architecture, Domain-Driven Design (DDD), Microservizi, Monolith |
| **Pattern** | CQRS (MediatR), Repository, Abstract Factory, Dependency Injection, Observer |
| **Principi** | SOLID, DRY, KISS, Separation of Concerns |
| **Messaging** | RabbitMQ, Azure Service Bus, pattern Pub/Sub |
| **Protocolli IoT** | MQTT |
| **Resilienza** | Retry, Circuit Breaker, Timeout, Bulkhead |

### Cloud & DevOps
| Area | Tecnologie |
|---|---|
| **Azure** | WebApp, Functions, SQL Database, Service Bus, Application Insights, Key Vault |
| **Container** | Docker, Docker Compose |
| **CI/CD** | Azure DevOps Pipelines, Git, branching strategies |
| **Monitoring** | Application Insights, Grafana, Loki, Prometheus, logging strutturato |

### Database & Search
| Area | Tecnologie |
|---|---|
| **Relazionali** | SQL Server, Azure SQL, SQLite |
| **NoSQL** | MongoDB |
| **Full-text Search** | ElasticSearch, Apache Solr |

### Testing & Quality
| Area | Tecnologie |
|---|---|
| **Unit Testing** | MSTest, xUnit, Moq, FluentAssertions |
| **Approccio** | Test-driven development, code review sistematiche |
| **AI & Produttività** | GitHub Copilot, coding agents AI |

### Security
| Area | Competenze |
|---|---|
| **Fondamenti** | OWASP Top 10, input validation, autenticazione/autorizzazione sicura |
| **Azure** | Key Vault, Managed Identity, HTTPS enforcement |
| **Segreti & Credenziali** | Gestione sicura di segreti, password e chiavi API (Key Vault, variabili d'ambiente protette, no hardcoding) |

---

## 🎓 Istruzione

### Diploma di Perito Informatico (79/100)
**I.T.I.S. Max Planck** — Lancenigo, Villorba  
📅 2006 – 2011

---

## 🌐 Lingue

| Lingua | Livello |
|---|---|
| 🇮🇹 Italiano | Madrelingua |
| 🇬🇧 Inglese | B2 (comprensione, parlato, scritto) |

---

## 🤝 Competenze Personali

**Capacità comunicative:**
- Ottima capacità e sensibilità nell'ascolto e di entrare in empatia con il prossimo.

**Competenze professionali:**
- Dinamicità nell'apprendimento e flessibilità. Buona capacità organizzativa nella pianificazione delle attività sulla base delle priorità stabilite.
- Da aprile 2022 ho formato un mio gruppo di lavoro all'interno dell'ufficio di R&D, così da avere la possibilità di migliorare le attività di sviluppo e gestione dei progetti.

---

## 🌱 Altre Competenze

- Giardinaggio, fitness e nutrizione

---

## 🏷️ Keywords

`.NET` `C#` `Azure` `Microservizi` `Clean Architecture` `DDD` `CQRS` `RabbitMQ` `Docker` `SQL Server` `MongoDB` `ElasticSearch` `Angular` `TypeScript` `CI/CD` `Azure DevOps` `GitHub Copilot` `MSTest` `xUnit` `OWASP` `Team Leadership` `Agile` `Scrum` `.NET 10` `GitHub Actions` `Stripe` `SaaS` `AI Agent` `Tool Calling` `LLM Integration`

---

## 🔎 Formazione Extra (non IT)

- **Seminario 16 ore su nutrizione ed integrazione sportiva** — Privato Marco Venturi (2015) — Biblioteca comunale San Polo di Piave
- **Progettista AutoCAD 2D/3D** — Pragma (2013–2014) — Voto: 28/30
- **Istruttore BodyBuilding & Fitness 1° Livello** — C.S.E.N. (2014) — Anatomia, Fisiologia e Biomeccanica base — Massimo dei voti

---

*Autorizzo il trattamento dei miei dati personali ai sensi del Decreto Legislativo 30 giugno 2003, n. 196 "Codice in materia di protezione dei dati personali".*
