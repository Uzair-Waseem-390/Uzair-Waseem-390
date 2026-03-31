<!--
  Premium GitHub Profile README
  Designed for Uzair Waseem - Backend & Agentic AI Developer
  Theme: Clean White Premium | Focus: System Design, Backend, AI Agents
-->

<p align="center">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&size=28&duration=3000&pause=500&color=000000&center=true&vCenter=true&width=600&lines=Uzair+Waseem;Backend+%26+Agentic+AI+Developer;System+Design+%3E+Code;Building+Scalable+Ecosystems" alt="Typing Animation" />
</p>

<p align="center">
  <img src="https://raw.githubusercontent.com/Uzair-Waseem-390/Uzair-Waseem-390/main/assets/coding.gif" width="500" alt="Coding GIF" />
</p>

---

### 🧠 About Me

I architect **scalable backend systems** and **agentic AI workflows** that operate at the intersection of reliability and intelligence.  
My philosophy is simple: **Don't build features. Build systems.**

- 🔧 **System Design** – from monoliths to microservices, with a focus on resilience
- ⚙️ **Async Processing** – mastering Celery, Redis, and distributed task queues
- 🤖 **Agentic AI** – creating autonomous agents for real-world automation
- 🏗️ **SaaS Architecture** – multi-tenancy, RBAC, and enterprise-grade patterns
- 📍 Based in **Pakistan**, building for a global impact

---

### 🛠️ Tech Stack

<p align="center">
  <img src="https://skillicons.dev/icons?i=python,django,fastapi,react,postgres,redis,docker,githubactions,openai&perline=9" />
</p>

---

### 🚀 Featured Projects

<table align="center">
  <tr>
    <td width="50%" valign="top">
      <h3>PathWeaver</h3>
      <p><strong>AI Job Automation System</strong></p>
      <p>End-to-end job pipeline: scraping, AI matching, resume analysis, and automated applications. Powered by Celery and Redis for asynchronous workflows.</p>
      <p><strong>Tech:</strong> Django, React, Celery, Redis, PostgreSQL, AI Models</p>
      <a href="https://github.com/Uzair-Waseem-390/PathWeaver">🔗 Repository</a>
      <br><br>
      <img src="project_images/pathweaver/thumbnail.png" width="100%" alt="PathWeaver Screenshot" />
    </td>
    <td width="50%" valign="top">
      <h3>School Management System (SaaS)</h3>
      <p><strong>Multi-Branch Educational Platform</strong></p>
      <p>Enterprise SaaS with 7 role-based dashboards, finance analytics, and real institutional workflow automation.</p>
      <p><strong>Tech:</strong> Django, PostgreSQL, Bootstrap</p>
      <a href="https://github.com/Uzair-Waseem-390/SMS">🔗 Repository</a>
      <br><br>
      <img src="project_images/school/thumbnail.png" width="100%" alt="School Management System Screenshot" />
    </td>
  </tr>
  <tr>
    <td width="50%" valign="top">
      <h3>Datavo</h3>
      <p><strong>AI Schema Generator</strong></p>
      <p>An AI agent that asks clarifying questions before generating optimized database schemas. Structured outputs for production readiness.</p>
      <p><strong>Tech:</strong> FastAPI, React, OpenAI API</p>
      <a href="https://github.com/Uzair-Waseem-390/Datavo">🔗 Repository</a>
      <br><br>
      <img src="project_images/datavo/thumbnail.png" width="100%" alt="Datavo Screenshot" />
    </td>
    <td width="50%" valign="top">
      <h3>Virelix</h3>
      <p><strong>AI ERP Builder</strong></p>
      <p>Translates business requirements into working ERP modules with RBAC and multi-tenancy. Modular architecture for scalability.</p>
      <p><strong>Tech:</strong> Django, React, Celery, Redis, OpenAI API</p>
      <a href="https://github.com/Uzair-Waseem-390/Virelix">🔗 Repository</a>
      <br><br>
      <img src="project_images/virelir/thumbnail.png" width="100%" alt="Virelix Screenshot" />
    </td>
  </tr>
</table>

---

### 🏛️ System Design Philosophy

I believe **systems should be built to evolve, not to impress**.  
My approach combines:

- **Loose Coupling** – Independent services that communicate through well-defined APIs
- **Event-Driven Architecture** – Using message brokers for asynchronous, resilient workflows
- **Data Consistency** – Balancing ACID with eventual consistency where it matters
- **Observability First** – Logging, metrics, and tracing as non-negotiable components
- **Security by Design** – From API gateways to database encryption

> "Simplicity is the ultimate sophistication. Complex systems should be broken down into simple, manageable pieces."

---

### 📊 GitHub Analytics

<p align="center">
  <img height="180em" src="https://github-readme-stats.vercel.app/api?username=Uzair-Waseem-390&show_icons=true&theme=default&hide_border=true&bg_color=ffffff&title_color=000000&icon_color=000000&text_color=333333" />
  <img height="180em" src="https://github-readme-streak-stats.herokuapp.com/?user=Uzair-Waseem-390&theme=default&hide_border=true&background=ffffff&stroke=000000&ring=000000&fire=000000&currStreakNum=000000&sideNums=000000&currStreakLabel=000000&sideLabels=000000" />
</p>

---

### 🐍 Contribution Snake

<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/Uzair-Waseem-390/Uzair-Waseem-390/output/github-contribution-grid-snake-dark.svg" />
    <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/Uzair-Waseem-390/Uzair-Waseem-390/output/github-contribution-grid-snake.svg" />
    <img alt="github contribution grid snake animation" src="https://raw.githubusercontent.com/Uzair-Waseem-390/Uzair-Waseem-390/output/github-contribution-grid-snake.svg" />
  </picture>
</p>

<details>
  <summary>🔧 Setup Guide for Snake Animation</summary>
  
  Add this GitHub Action to your repository to keep the snake animation updated daily:
  
  ```yaml
  name: Generate Snake Animation
  on:
    schedule:
      - cron: "0 0 * * *"
    workflow_dispatch:
  jobs:
    build:
      runs-on: ubuntu-latest
      steps:
        - uses: actions/checkout@v3
        - uses: Platane/snk@v3
          with:
            github_user_name: Uzair-Waseem-390
            outputs: |
              dist/github-contribution-grid-snake.svg
              dist/github-contribution-grid-snake-dark.svg?palette=github-dark
        - uses: peaceiris/actions-gh-pages@v3
          with:
            github_token: ${{ secrets.GITHUB_TOKEN }}
            publish_dir: ./dist
            publish_branch: output
