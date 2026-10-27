# Agile Team Charter Evidence

This page documents the foundational **Agile Team Charter** and collaboration framework established for the **B.E. Cortege** project within the Black Elegance Group ecosystem.

---

## 1. Completed Team Charter

The charter defines the team's shared mission, roles, working agreements, decision-making protocols, communication channels, Definition of Done, and operational boundaries.

- [**View completed Agile Team Charter markdown**](./agile_team_charter.md)
- [**View B.E. Cortege Source Code on GitHub**](https://github.com/Emeritus-Dev/beCortege)

### 1.1 Project Purpose & North Star
> **Mission:** To engineer a dignified, high-performance, community-centric luxury e-hailing platform for Black Elegance Group event-goers and premium commuters in Cape Town, delivered iteratively through reliable Agile engineering practices.

### 1.2 Team Composition & Responsibilities

| Role | Member Name | Core Focus Areas |
| :--- | :--- | :--- |
| **Full-Stack & Systems Lead** | **Tshegofatso Hlabela** | System architecture, React frontend, routing, Leaflet geospatial mapping, Netlify deployment pipeline |
| **Frontend & UI/UX Specialist** | Team Collaborator | Component design, Tailwind styling, brand theme consistency, accessibility UX |
| **Backend & Data Specialist** | Team Collaborator | Supabase/PostgreSQL schema modeling, REST API contracts, security & POPIA compliance |
| **Quality & Agile Coordinator** | Team Collaborator | Trello board maintenance, stand-up documentation, retrospective facilitation, user acceptance testing |

---

## 2. Working Agreements & Operational Rules

Our team committed to six non-negotiable operational agreements to ensure build integrity and continuous delivery:

1. **Card Ownership & Transparency:** Every active backlog card on Trello must have an assigned owner and clear acceptance criteria before work begins.
2. **Clean Version Control:** Developers must work on isolated feature branches (`feature/feature-name`). Direct pushes to `master` are strictly prohibited.
3. **Strict Build Integrity:** All code must compile cleanly via `npm run build` locally prior to pull requests to prevent case-sensitive import failures on Netlify's Linux environment.
4. **Environment & Data Security:** No private keys, database credentials, or API tokens may be committed to version control (`.env` ignored). Full credit card numbers and CVVs are never persisted.
5. **Continuous Communication:** Any blocker preventing progress for more than 4 hours must be immediately posted to the designated escalation channel.
6. **Constructive Code Reviews:** Pull requests require peer verification, checking code modularity, styling standards, and responsive viewport performance.

---

## 3. Definition of Done (DoD)

A user story or backlog task is classified as **Done** only when:
- [x] Code adheres to repository style guides and component modularity standards.
- [x] Tested and verified across major responsive breakpoints (desktop, tablet, and mobile).
- [x] Fully integrated and building cleanly without console errors or warnings (`npm run build`).
- [x] Netlify continuous integration build passes successfully.
- [x] Trello card moved to the "Done" list and referenced in the Git commit message.

---

## 4. Communication & Collaboration Evidence

The team coordinated all sprint iterations, reviews, and repository activities through a combination of asynchronous messaging and structured project management boards.

### 4.1 Communication & Stand-up Workflow

+-----------------------------------------------------------------------------------+
|                           COMMUNICATION CHANNELS                                  |
+--------------------------+----------------------------+---------------------------+
|      Async Updates       |       Sync Stand-ups       |     Code & Tasks          |
|  * WhatsApp Group        |  * Microsoft Teams         |  * GitHub PRs & Reviews   |
|  * Urgent Blockers       |  * 3x Weekly (15 mins)     |  * Trello Kanban Board    |
|  * Deployment Alerts     |  * Sprint Reviews & Retros |  * Markdown Documentation |
+--------------------------+----------------------------+---------------------------+


### 4.2 Trello Kanban Board Setup

The team established a visual Kanban board structure to manage work in flight:

[ Product Backlog ] ──> [ Sprint Backlog ] ──> [ In Progress ] ──> [ Code Review / QA ] ──> [ Done (DoD Met) ]


- **Trello Workspace Link:** [Open B.E. Cortege on Trello](https://trello.com) *(Insert direct Trello board link)*

### 4.3 Git & GitHub Collaboration Evidence

Branch governance, commit discipline, and continuous delivery rules were maintained on GitHub:

- **Repository Link:** [Emeritus-Dev/beCortege](https://github.com/Emeritus-Dev/beCortege)
- **Primary Branch:** `master`
- **Deployment Status:** Production automated CI/CD pipeline on Netlify Edge

---

## 5. Evidence Alignment to Charter Commitments

The operational artifacts directly support the commitments agreed upon in our charter:

- **Communication:** Microsoft Teams and WhatsApp provided immediate channels for daily coordination and blocker escalations.
- **Transparency:** Trello sprint lists made card ownership, task state, and milestone progress visible to all members.
- **Collaboration:** Pull requests and peer reviews guaranteed that UI styling and map tracking components integrated cleanly.
- **Accountability:** Single-owner assignments ensured clear ownership for each deliverable across Sprints 1 to 5.
- **Integrity & Quality:** Enforcing our Definition of Done prevented broken builds and missing dependencies fro
