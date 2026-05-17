<div align="center">

<a href="https://github.com/Uzair-Waseem-390">
  <img src="https://readme-typing-svg.demolab.com?font=Sora&weight=600&size=28&duration=3000&pause=1200&color=0A0A0A&background=FFFFFF00&center=true&vCenter=true&multiline=false&width=700&height=60&lines=Hi%2C+I%27m+Uzair+Waseem+%F0%9F%91%8B;Backend+%26+Agentic+AI+Developer;I+build+systems%2C+not+just+features." alt="Typing SVG" />
</a>

<br/>

<img src="https://readme-typing-svg.demolab.com?font=Sora&weight=400&size=15&duration=4000&pause=2000&color=555555&background=FFFFFF00&center=true&vCenter=true&width=600&height=30&lines=%E2%80%9CScalability+isn%27t+added+later.+It%27s+designed+from+the+start.%E2%80%9D" alt="Quote" />

<br/><br/>

[![GitHub](https://img.shields.io/badge/GitHub-0A0A0A?style=for-the-badge&logo=github&logoColor=white)](https://github.com/Uzair-Waseem-390)
&nbsp;
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A0A0A?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/uzairwaseem)
&nbsp;
[![Location](https://img.shields.io/badge/Pakistan-0A0A0A?style=for-the-badge&logo=googlemaps&logoColor=white)](https://github.com/Uzair-Waseem-390)
&nbsp;
[![Open to Work](https://img.shields.io/badge/Open%20to%20Work-2EA44F?style=for-the-badge&logo=checkmarx&logoColor=white)](https://github.com/Uzair-Waseem-390)

</div>

---

<br/>

<div align="center">
  <h2>⬛ About Me</h2>
</div>

```
  Role     →  Backend & Agentic AI Developer
  Focus    →  System Design · Async Pipelines · SaaS Architecture
  Stack    →  Python · Django · FastAPI · Redis · Celery · PostgreSQL
  Current  →  Building GazaBridge (prod) + NovaDB (database engine)
  Belief   →  "Scalability isn't added later. It's designed from the start."
```

I design and build backend infrastructure that scales — from async task pipelines to multi-tenant SaaS platforms to AI agent systems that replace entire manual workflows.

My work sits at the intersection of **distributed systems**, **AI automation**, and **real-world product engineering**.

<br/>

---

<br/>

<div align="center">
  <h2>⬛ Tech Stack</h2>
  <br/>
  <img src="https://skillicons.dev/icons?i=python,django,fastapi,react&theme=light&perline=8" alt="Languages" />
  <br/><br/>
  <img src="https://skillicons.dev/icons?i=postgres,redis,docker,github&theme=light&perline=8" alt="Infra" />
  <br/><br/>
  <img src="https://skillicons.dev/icons?i=openai&theme=light&perline=8" alt="AI" />
  &nbsp;
  <img src="https://img.shields.io/badge/Celery-37814A?style=flat-square&logo=celery&logoColor=white" height="48"/>
  &nbsp;
  <img src="https://img.shields.io/badge/Supabase-3ECF8E?style=flat-square&logo=supabase&logoColor=white" height="48"/>
  &nbsp;
  <img src="https://img.shields.io/badge/JWT-000000?style=flat-square&logo=jsonwebtokens&logoColor=white" height="48"/>
</div>

<br/>

---

<br/>

<div align="center">
  <h2>⬛ Featured Projects</h2>
  <p><i>Systems built to solve real problems at scale</i></p>
</div>

<br/>

<table width="100%">
<tr>
<td width="50%" valign="top">

### 🌍 GazaBridge — Humanitarian API Platform

**The problem:** Palestinian individuals lack structured access to global mentors, educators, and resources.

**The system:** A full-stack platform (Django DRF + React) connecting Palestinians with global volunteers offering mentorship, courses, live sessions, and curated resources.

**Architecture highlights:**
- JWT auth with **Redis-based token blacklisting** (DB 2)
- **3-partition Redis** — broker (DB 0) · API cache (DB 1) · rate limiter (DB 2)
- **Celery** async pipeline for email verification + password reset
- Custom **sliding-window rate limiter** middleware (100 req/min auth · 20 req/min anon)
- **Google OAuth2** + Gmail SMTP
- **Supabase PostgreSQL** via PgBouncer connection pooling
- OpenAPI 3.0 schema via `drf-spectacular`
- 6 backend modules: users · auth · posts · courses · live sessions · resources

**Stack:** `Django` · `DRF` · `Celery` · `Redis` · `PostgreSQL` · `Supabase` · `JWT` · `React`

[![View Repo](https://img.shields.io/badge/View%20Repo-%230A0A0A?style=for-the-badge&logo=github&logoColor=white)](https://github.com/Uzair-Waseem-390/GazaBridge)

</td>
<td width="50%" valign="top">

### 🗄️ NovaDB — Database Engine *(In Progress)*

**The problem:** Most developers use databases without understanding what's happening underneath — and that lack of knowledge creates bad systems.

**The system:** A PostgreSQL-inspired relational database engine built from scratch — with intelligent native caching as its defining feature.

**Planned architecture:**
- **SQL Parser** → Lexer + AST generation
- **Storage Engine** → page-based binary file layout (4KB pages)
- **Adaptive Cache Layer** → LRU + query result cache + hot-table prediction
- **B+ Tree Index Engine** → insert, split, search, delete
- **Query Planner/Optimizer** → cost-based decision engine
- **Execution Engine** → scan, filter, project, join
- **WAL + Transactions** → crash recovery, rollback, ACID
- **MVCC** → Postgres-style versioned rows for concurrent access

**CV line:**
> Built NovaDB, a PostgreSQL-inspired relational database engine with SQL parsing, B+ tree indexing, intelligent native caching, WAL, and MVCC-based concurrency control.

**Stack:** `Python` · `struct` · `mmap` · `asyncio`

[![View Repo](https://img.shields.io/badge/View%20Repo-%230A0A0A?style=for-the-badge&logo=github&logoColor=white)](https://github.com/Uzair-Waseem-390/NovaDB)

</td>
</tr>
<tr><td colspan="2"><br/></td></tr>
<tr>
<td width="50%" valign="top">

### 🤖 PathWeaver — AI Job Assistant

**The problem:** Job hunting is broken. It's manual, slow, and inefficient.

**The system:** A fully automated AI pipeline that scrapes jobs, parses resumes, calculates match scores, and surfaces only the right opportunities — while you sleep.

- Async pipeline via **Celery + Redis**
- Resume analysis + job compatibility scoring
- Scheduled job scraping with dynamic filtering
- Full SaaS-ready architecture

**Stack:** `Django` · `React` · `Celery` · `Redis` · `PostgreSQL` · `AI Models`

[![View Repo](https://img.shields.io/badge/View%20Repo-%230A0A0A?style=for-the-badge&logo=github&logoColor=white)](https://github.com/Uzair-Waseem-390/PathWeaver)

</td>
<td width="50%" valign="top">

### ⚙️ Virelix — AI ERP Builder

**The problem:** Building an ERP takes months and costs a fortune.

**The system:** Converts business requirements into a working, modular ERP system — with RBAC, multi-tenant design, and AI-assisted module generation.

- Business requirements → working ERP modules
- Role-Based Access Control (RBAC) built-in
- Multi-tenant from the ground up
- Modular, not monolithic

**Stack:** `Django` · `React` · `Celery` · `Redis` · `OpenAI API`

[![View Repo](https://img.shields.io/badge/View%20Repo-%230A0A0A?style=for-the-badge&logo=github&logoColor=white)](https://github.com/Uzair-Waseem-390/Virelix)

</td>
</tr>
<tr><td colspan="2"><br/></td></tr>
<tr>
<td width="50%" valign="top">

### 🧠 Datavo — AI Schema Generator

**The problem:** Designing database schemas requires deep domain knowledge most developers lack.

**The system:** A conversational AI agent that asks clarifying questions before generating optimized, production-ready schemas — structured outputs, no hallucinations.

- Clarification loop before schema generation
- Structured output engineering
- Dynamic prompt optimization
- Clean FastAPI + React interface

**Stack:** `FastAPI` · `React` · `OpenAI SDK`

[![View Repo](https://img.shields.io/badge/View%20Repo-%230A0A0A?style=for-the-badge&logo=github&logoColor=white)](https://github.com/Uzair-Waseem-390/Datavo)

</td>
<td width="50%" valign="top">

### 🏫 School Management System (SaaS)

**The problem:** Educational institutions run on spreadsheets and WhatsApp.

**The system:** A full multi-tenant SaaS platform with 7 distinct role-based dashboards, finance modules, and institutional workflow automation.

- Multi-branch, multi-tenant architecture
- **7 role-based dashboards** (Admin, Teacher, Student, Finance...)
- Finance reporting for decision-making
- Real-world institutional logic baked in

**Stack:** `Django` · `PostgreSQL`

[![View Repo](https://img.shields.io/badge/View%20Repo-%230A0A0A?style=for-the-badge&logo=github&logoColor=white)](https://github.com/Uzair-Waseem-390/SMS)

</td>
</tr>
</table>

<br/>

---

<br/>

<div align="center">
  <h2>⬛ System Design Philosophy</h2>
</div>

<br/>

```
┌─────────────────────────────────────────────────────────────────────┐
│                    HOW I THINK ABOUT SYSTEMS                        │
├───────────────────┬─────────────────────────────────────────────────┤
│  Scalability      │  Horizontal by design, not by accident          │
│  Async Pipelines  │  Celery + Redis for decoupled task execution     │
│  AI Integration   │  Agents as workers in larger orchestrated flows  │
│  Data Modeling    │  Schema-first, migration-safe, query-optimized   │
│  Multi-tenancy    │  Isolated by design from row 1                   │
│  Caching          │  3 logical Redis partitions, never one flat pool │
│  Rate Limiting    │  Sliding-window, IP-aware, trusted-proxy safe    │
│  Observability    │  If you can't measure it, you can't fix it       │
└───────────────────┴─────────────────────────────────────────────────┘
```

<br/>

---

<br/>

<div align="center">
  <h2>⬛ GitHub Stats</h2>
  <br/>
  <img src="https://streak-stats.demolab.com?user=Uzair-Waseem-390&theme=default&hide_border=true&ring=0A0A0A&fire=0A0A0A&currStreakLabel=0A0A0A&dates=666666&sideNums=0A0A0A&sideLabels=555555&currStreakNum=0A0A0A" alt="GitHub Streak" />
</div>

<br/>

---

<br/>

<div align="center">
  <h2>⬛ Currently Building</h2>
</div>

<br/>

```python
class CurrentFocus:
    active = {
        "GazaBridge": "Shipping production features — live sessions, resource modules, deployment",
        "NovaDB":     "Phase 1 — SQL parser + page-based storage engine (Python)",
    }

    next = [
        "Adaptive cache layer with hot-table prediction (NovaDB Phase 3)",
        "MVCC + concurrent transaction support (NovaDB Phase 5)",
        "Multi-agent orchestration pipelines with memory & tool use",
    ]

    philosophy = "Every system I build must survive production."

    milestone = "Ship NovaDB Phase 1 with working SELECT/INSERT/CREATE TABLE."
```

<br/>

---

<br/>

<div align="center">
  <h2>⬛ Writing</h2>
  <p><i>Secure & Scalable Backend Engineering</i></p>
</div>

<br/>

> 📝 **Why I Use 3 Redis Partitions Instead of One**
> *How GazaBridge separates task brokering, API caching, and rate limiting in isolated logical DBs — and why mixing them is a hidden reliability risk.*

> 📝 **Building a Sliding-Window Rate Limiter From Scratch**
> *The custom GlobalRateLimitMiddleware in GazaBridge: trusted proxy detection, IP spoofing prevention, and Redis-backed counters.*

> 📝 **How I Structure Celery Pipelines That Don't Break Under Load**
> *Task routing, retry strategies, and failure isolation in production async pipelines.*

> 📝 **Multi-Tenancy at the Database Level: Row-Level vs Schema-Level Isolation**
> *When to use which — and why getting it wrong costs you a full rewrite.*

<br/>

---

<br/>

<div align="center">
  <h2>⬛ Let's Connect</h2>
  <br/>
  <p>I'm interested in backend roles, AI/agent systems, and ambitious SaaS products.</p>
  <p>If you're building something real — let's talk.</p>
  <br/>

  [![GitHub](https://img.shields.io/badge/GitHub-0A0A0A?style=for-the-badge&logo=github&logoColor=white)](https://github.com/Uzair-Waseem-390)
  &nbsp;
  [![LinkedIn](https://img.shields.io/badge/LinkedIn-0A0A0A?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/uzairwaseem)
  &nbsp;
  [![Email](https://img.shields.io/badge/Email-0A0A0A?style=for-the-badge&logo=gmail&logoColor=white)](mailto:uzairwaseem390@gmail.com)

  <br/><br/>

  <img src="https://komarev.com/ghpvc/?username=Uzair-Waseem-390&color=000000&style=flat-square&label=Profile+Views" alt="Profile Views" />

</div>

<br/>

---

<div align="center">
  <sub>
    Designed with precision. Built with purpose. &nbsp;·&nbsp; <b>Uzair Waseem</b> &nbsp;·&nbsp; Pakistan 🇵🇰
  </sub>
</div>
