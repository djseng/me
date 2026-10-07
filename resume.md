# David Seng
**Senior Software Engineer | .NET, Azure, Application Modernization, Agent-First Development**

**Email:** david@hessian.dev | **Location:** Bloomington, IL (remote US) | **LinkedIn:** [in/dave-seng](https://www.linkedin.com/in/dave-seng)

## Professional Summary
Remote US .NET/Azure engineer with more than 25 years of hands-on development, 16 of them with the same firm through two acquisitions. My title is Architect, but my day-to-day work is senior individual-contributor engineering from a Linux-based development environment. On a large .NET/Angular monorepo, I built an AI pull request review workflow that checks every finding against the original work item, and reworked an EF Core calculation pipeline to run more than 50% faster.

## Professional Experience

### **3Cloud** *(formerly Polaris Solutions)* | Oct 2010 – Present · 16 yrs
**Architect - Software Engineering** | May 2023 – Present · 3 yrs 6 mos<br>
**Senior Application Engineer - .NET** | Nov 2021 – Apr 2023 · 1 yr 4 mos<br>
**Senior Developer, Polaris Solutions** | Oct 2010 – Oct 2021 · 11 yrs 2 mos

*3Cloud acquired Polaris Solutions in November 2021, and Cognizant acquired 3Cloud effective January 1, 2026; my tenure carried over through both.*

#### **Enterprise .NET/Angular Monorepo Modernization** | May 2025 – Present · 1 yr 6 mos
*Enterprise client. .NET 8 / Angular 21 monorepo: ~220 backend projects, ~1.5M lines of code, 70+ contributors across five regions.*

- Reworked the core calculation pipeline (EF Core, SQL Server) behind a feature flag: replaced ~15 scattered `SaveChanges` calls with one transactional persist, moved lookups in memory, and fixed N+1 queries. More than 50% faster on typical projects in testing.
- Replaced AutoMapper with Mapperly, with a source generator for `IMapper` so call sites didn't change. Cut PR and release pipelines from ~15 minutes to under 5.
- Added ~40 functional tests, including end-to-end calculation scenarios, that run in CI against a real database, and got ~500 Angular tests running in CI for the first time, fixing ~100 broken ones.
- Built and tuned an AI pull request review workflow with Cursor and then GitHub Copilot. It pulls acceptance criteria through the Azure DevOps MCP server and runs reviews in parallel across git worktrees, and I checked every finding against the original work item's intent. Introduced the team to the Azure MCP server for Application Insights triage.
- Primary code reviewer and mentor for 5–6 developers; covered standups and support triage for the team lead.
- Moved the Angular SPA from webpack to Vite and Vitest and the single-spa shell to Rolldown, and modernized an unmaintained React micro-frontend SDK.
- Wrote PowerShell tooling about half the team adopted, including `Get-PR` (opens a PR in a ready-to-run git worktree with cached SDK builds) and a bacpac export that shrank databases from several hundred MB to ~20 MB.

#### **Short Engagements** | Oct 2023 – Oct 2024
- **Application Modernization** (Jul 2024 – Oct 2024 · 3 mos): Ported stored procedures to C# APIs and automated OpenAPI imports into Azure API Management.
- **Internal Chatbot POC** (Jun 2024 · 1 mo): Built a Teams RAG chatbot over prior statements of work using Azure AI Search.
- **Transcription Service** (Apr 2024 – May 2024 · 2 mos): Built an ASP.NET MVC and HTMX admin UI.
- **Integration Platform** (Oct 2023 – Mar 2024 · 6 mos): Built C# Durable Functions that split PDFs, extracted invoice data with Azure Document Intelligence, and merged Excel documents.

#### **Application Modernization and Greenfield Development** | Apr 2019 – Sep 2023 · 4 yrs 6 mos
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
- **Languages & Frameworks:** C#, TypeScript, JavaScript, T-SQL, PowerShell; .NET 8/9, ASP.NET Core, EF Core, Node.js, Angular 21, React
- **Azure & Data:** Application Insights, Bicep, Durable Functions, Document Intelligence, AI Search, API Management, SQL Server, MySQL, MongoDB, DB2
- **Platform & Delivery:** Azure DevOps Pipelines, GitHub Actions, GitLab CI/CD, Docker, Kubernetes, Kafka, OpenTelemetry, Vite
- **AI-Assisted Development:** Cursor, GitHub Copilot, Azure and Azure DevOps MCP servers, AI pull request review workflows
- **Git & Environment:** Git (worktrees, submodules, rebase, history rewrites, migrations), Linux, Bash
