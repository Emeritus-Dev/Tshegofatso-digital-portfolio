<div align="center">

# 🚗 B.E. Cortege
### *Arrive in Procession*

**Work-Integrated Learning (WIL) Digital Portfolio**  
*Project Presentation 3 (PRP370S / PRP372S)*

[![CPUT](https://img.shields.io/badge/CPUT-Informatics%20%26%20Design-005A9C?style=for-the-badge)](https://www.cput.ac.za)
[![Assessment](https://img.shields.io/badge/Assessment-2%20(Oct%202026)-teal?style=for-the-badge)](https://github.com/Emeritus-Dev/beCortege)
[![Status](https://img.shields.io/badge/Build-Passing-2ea44f?style=for-the-badge)](https://github.com/Emeritus-Dev/beCortege)
[![Deployment](https://img.shields.io/badge/Deployed-Netlify-00C7B7?style=for-the-badge&logo=netlify&logoColor=white)](https://github.com/Emeritus-Dev/beCortege)

</div>

---

## 📌 Executive Summary

**B.E. Cortege** is an enterprise-grade, luxury e-hailing web and mobile solution engineered for the **Black Elegance Group (B.E.Group)** and its community ecosystem. South Africa's transport sector lacks high-touch, event-focused convoy services. B.E. Cortege bridges this gap through real-time convoy tracking (2 to 4 matching vehicles), verified chauffeur selection, an accessible riding profile (mobility, sensory, and calming preferences), and a tiered loyalty program.

> **Operational Scope:** Cape Town Metropolitan Area (V&A Waterfront, Bo-Kaap, Camps Bay, Cape Town Stadium, Table Mountain, and Cape Town International Airport).

---

## 🎓 Academic & Student Credentials

| Attribute | Profile Information |
| :--- | :--- |
| **Candidate Name** | **Tshegofatso Hlabela** |
| **Student Number** | `222975016` |
| **Academic Department** | Department of Information Technology |
| **Faculty** | Faculty of Informatics and Design |
| **Institution** | Cape Peninsula University of Technology (CPUT) |
| **Qualification** | National Diploma in ICT: Applications Development |
| **Module** | Project Presentation 3 (`PRP370S` / `PRP372S`) |
| **Assessor** | Mrs. P. Inderlal |

---

## 🛠️ Architecture & Technology Stack

### Client-Side Architecture

* <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/react/react-original.svg" alt="React" width="16" height="16"/> **React 18** — Powers the component-driven interface, state synchronization, and reactive UI pipelines.
* <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/vitejs/vitejs-original.svg" alt="Vite" width="16" height="16"/> **Vite 8** — Optimized build tooling providing lightning-fast Hot Module Replacement (HMR).
* <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/javascript/javascript-original.svg" alt="JavaScript" width="16" height="16"/> **Modern ECMAScript (ES6+)** — Modular application logic and asynchronous data mapping.
* <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/css3/css3-original.svg" alt="CSS3" width="16" height="16"/> **CSS Custom Properties (Variables)** — Dark luxury palette aligned with B.E.Group brand standards (`#0D9488` teal, `#1E40AF` blue, `#EA580C` accent).
* <img src="https://raw.githubusercontent.com/simple-icons/simple-icons/develop/icons/leaflet.svg" alt="Leaflet" width="16" height="16"/> **Leaflet & OSRM Engine** — Real-time geospatial mapping, road route geometry, and turn-by-turn simulation.
* <img src="https://raw.githubusercontent.com/simple-icons/simple-icons/develop/icons/capacitor.svg" alt="Capacitor" width="16" height="16"/> **Capacitor** — Native runtime bridge packaging the responsive web build for Android deployment.

### Persistence, Security & Services

* <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/postgresql/postgresql-original.svg" alt="PostgreSQL" width="16" height="16"/> **PostgreSQL / Supabase** — Cloud data persistence for `profiles`, `member_accounts`, `drivers`, `trips`, and `ratings`.
* <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/java/java-original.svg" alt="Java" width="16" height="16"/> **Java & Spring Boot** — Planned enterprise domain service layer and robust API boundaries.
* <img src="https://raw.githubusercontent.com/simple-icons/simple-icons/develop/icons/jsonwebtokens.svg" alt="Security" width="16" height="16"/> **POPIA Compliance & Card Masking** — Secure credential management storing only issuer and last-4 digits; CVV and raw PAN are excluded by design.

### Cloud Infrastructure & CI/CD

* <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/git/git-original.svg" alt="Git" width="16" height="16"/> **Git / GitHub** — Strict version control workflows, branch protection, and Agile asset organization.
* <img src="https://raw.githubusercontent.com/simple-icons/simple-icons/develop/icons/netlify.svg" alt="Netlify" width="16" height="16"/> **Netlify Edge** — Automated CI/CD deployment pipeline with custom SPA rewrite headers (`netlify.toml`).

<p align="right"><sub><em>Technology badges and vector logos sourced via Simple Icons and Devicon.</em></sub></p>

---

## 🔗 Project Repositories & Artifacts

| Resource | Direct Link | Details |
| :--- | :--- | :--- |
| **🌐 Production Web App** | [B.E. Cortege Live](https://becortege.netlify.app) | Production Single-Page Application |
| **🐙 GitHub Source Code** | [Emeritus-Dev/beCortege](https://github.com/Emeritus-Dev/beCortege) | Master source code and Capacitor build |
| **📋 Trello Agile Board** | [B.E. Cortege Agile Workspace](https://trello.com) | Product & Sprint Kanban board |

---

## 🗂️ Portfolio Evidence & Reflections

Following the Assessment 2 criteria, each section contains documented primary **Evidence** and a structured **STAR Methodology Reflection** (Situation, Task, Action, Result).

<table>
  <thead>
    <tr>
      <th width="35%">Agile Component</th>
      <th width="45%">Description</th>
      <th width="20%" align="center">Navigation</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><b>01. Agile Team Charter</b></td>
      <td>Team operating contract defining shared vision, values, communication guidelines, and the Definition of Done (DoD).</td>
      <td align="center">
        <a href="./01-agile-team-charter/evidence.md"><b>Evidence</b></a><br>
        <a href="./01-agile-team-charter/reflection.md"><b>Reflection</b></a>
      </td>
    </tr>
    <tr>
      <td><b>02. User Stories & Tasks</b></td>
      <td>Four core user journeys structured in standard Agile format with detailed technical task breakdowns and UI states.</td>
      <td align="center">
        <a href="./02-user-stories-and-tasks/evidence.md"><b>Evidence</b></a><br>
        <a href="./02-user-stories-and-tasks/reflection.md"><b>Reflection</b></a>
      </td>
    </tr>
    <tr>
      <td><b>03. Product Backlog</b></td>
      <td>Prioritized feature requirements structured using the MoSCoW framework, entity schema layouts, and database integration records.</td>
      <td align="center">
        <a href="./03-product-backlog/evidence.md"><b>Evidence</b></a><br>
        <a href="./03-product-backlog/reflection.md"><b>Reflection</b></a>
      </td>
    </tr>
    <tr>
      <td><b>04. Sprint Backlog</b></td>
      <td>Traceability matrix across Sprints 1 through 5, tracking feature implementation from Foundation to Deployment.</td>
      <td align="center">
        <a href="./04-sprint-backlog/evidence.md"><b>Evidence</b></a><br>
        <a href="./04-sprint-backlog/reflection.md"><b>Reflection</b></a>
      </td>
    </tr>
    <tr>
      <td><b>05. Agile Logbook</b></td>
      <td>Documentation of team stand-up cadences, Trello Kanban tracking records, sprint reviews, and retrospective action items.</td>
      <td align="center">
        <a href="./05-agile-logbook/evidence.md"><b>Evidence</b></a><br>
        <a href="./05-agile-logbook/reflection.md"><b>Reflection</b></a>
      </td>
    </tr>
  </tbody>
</table>

---

<div align="center">
<sub>Faculty of Informatics and Design • Cape Peninsula University of Technology • Cape Town Campus</sub>
</div>
