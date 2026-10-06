# David Seng
**Senior Software Engineer | .NET, Azure, Application Modernization, Agent-First Development**

**Email:** david@hessian.dev | **Location:** Bloomington, IL (remote US) | **LinkedIn:** [in/dave-seng](https://www.linkedin.com/in/dave-seng)

## Professional Summary
Remote US .NET/Azure engineer with more than 25 years of hands-on development, 16 of them with the same firm through two acquisitions. My title is Architect, but my day-to-day work is senior individual-contributor engineering, from a Linux-based development environment, and I stay on systems until I'm their institutional memory. My current work is agent-first delivery on a large .NET/Angular monorepo: agents write most of the code, and I own the design, review, and validation.

## Professional Experience

### **3Cloud, a Cognizant company** *(formerly Polaris Solutions)* | Oct 2010 – Present · 16 yrs
**Architect - Software Engineering** | May 2023 – Present · 3 yrs 6 mos<br>
**Senior Application Engineer - .NET** | Nov 2021 – Apr 2023 · 1 yr 4 mos<br>
**Senior Developer, Polaris Solutions** | Oct 2010 – Oct 2021 · 11 yrs 2 mos

*3Cloud acquired Polaris Solutions in November 2021, and Cognizant acquired 3Cloud effective January 1, 2026; my tenure carried over through both.*

#### **Enterprise .NET/Angular Monorepo Modernization** | May 2025 – Present · 1 yr 6 mos
*Enterprise client. .NET 8 / Angular 21 monorepo: ~220 backend projects, ~1.5M lines of code, 70+ contributors across five regions.*

- Worked agent-first with Cursor and then GitHub Copilot. Built and tuned an AI pull request review workflow that pulls acceptance criteria through the Azure DevOps MCP server and runs reviews in parallel across git worktrees; I checked every finding against the original work item's intent.
- Introduced the team to the Azure MCP server for Application Insights triage and the Azure DevOps MCP server for managing work items, through standup demos and wiki docs.
- Primary code reviewer and mentor for 5–6 developers; covered standups and support triage for the team lead.
- Reworked the core calculation pipeline (EF Core, SQL Server) behind a feature flag: replaced ~15 scattered `SaveChanges` calls with one transactional persist, moved lookups in memory, and fixed N+1 queries. More than 50% faster on typical projects in testing.
- Added ~40 functional tests, including end-to-end calculation scenarios, that run in CI against a real database, and got ~500 Angular tests running in CI for the first time, fixing ~100 broken ones.
- Moved the Angular SPA from webpack to Vite and Vitest and the single-spa shell to Rolldown, and modernized an unmaintained React micro-frontend SDK.
- Replaced AutoMapper with Mapperly, with a source generator for `IMapper` so call sites didn't change. Cut PR and release pipelines from ~15 minutes to under 5.
- Wrote PowerShell tooling about half the team adopted, including `Get-PR` (opens a PR in a ready-to-run git worktree with cached SDK builds) and a bacpac export that shrank databases from several hundred MB to ~20 MB.

#### **Short Engagements and Bench** | Oct 2023 – Apr 2025
- **Integration Platform** (6 mos): Built C# Durable Functions that split PDFs, extracted invoice data with Azure Document Intelligence, and merged Excel documents; led a small offshore team.
- **Application Modernization** (3 mos): Ported stored procedures to C# APIs and automated OpenAPI imports into Azure API Management.
- **Internal Chatbot POC** (1 mo): Built a Teams RAG chatbot over prior statements of work using Azure AI Search.
- **Transcription Service** (2 mos): Built an ASP.NET MVC and HTMX admin UI. **Bench** (Nov 2024 – Apr 2025): Earned AZ-204.

#### **Application Modernization and Greenfield Development** | Apr 2019 – Apr 2024 · 5 yrs
- Built and supported microservices on Kubernetes in Azure with Kafka, MongoDB, Grafana, and OpenTelemetry.
- Migrated services from .NET 5 to .NET 6 and moved source and CI/CD from GitHub to GitLab.
- Maintained a portability layer that synchronized greenfield applications with a legacy DB2 system of record.
- Modernized a Web Forms application to .NET Framework 4.8 with Microsoft.Extensions.DependencyInjection and YAML pipelines.

#### **Health Insurance Portal Modernization** | Sep 2011 – Dec 2018 · 7 yrs 2 mos
- Modernized a health insurance portal from Classic ASP to ASP.NET MVC with a WCF and SQL Server backend.
- Built an ETL application that moved data from iSeries DB2 to SQL Server.

#### **Earlier Polaris Engagements**
- **Angular Scheduling App** (Jan 2019 – May 2019 · 5 mos) and **Windows CE Scanner App** (Oct 2010 – Aug 2011 · 10 mos).

### **Earlier Experience**
- **PII, Web Developer** | Jun 2001 – Sep 2010 · 9 yrs 4 mos: Classic ASP to ASP.NET migrations, SQL Server, and AS/400 DB2 web services.
- **Websoft, Inc., Web Developer** | Feb 1998 – May 2001 · 3 yrs 4 mos: Classic ASP and Access applications.

## Certifications & Education
- **Microsoft:** AZ-204 (Jan 2025), AI-102 (Jun 2024), AI-900 (Jun 2024), AZ-900 (May 2024)
- **BS, Computer Science**, Illinois State University, 2003

## Technical Skills
- **Languages & Frameworks:** C#, T-SQL, TypeScript, PowerShell; .NET 8/9, ASP.NET Core, EF Core, Angular 21, React
- **Azure & Data:** Application Insights, Bicep, Durable Functions, Document Intelligence, AI Search, API Management, SQL Server, MongoDB, DB2
- **Platform & Delivery:** Azure DevOps Pipelines, GitHub Actions, GitLab CI/CD, Docker, Kubernetes, Kafka, OpenTelemetry, Vite
- **AI & Environment:** MCP servers, agent skills, Git (worktrees, submodules, rebase, history rewrites, migrations), Linux, Bash
