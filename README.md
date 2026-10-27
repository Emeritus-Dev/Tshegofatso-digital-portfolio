# Entrepreneurial WIL GitHub Portfolio
## B.E. Cortege
> *"Arrive in procession"*

A portfolio of project evidence and reflections for **Project Presentation 3 (PRP370S / PRP372S)**.

---

## Student Details
- **Name and Surname:** Tshegofatso Hlabela
- **Student Number:** 222975016
- **Institution:** Cape Peninsula University of Technology (CPUT)
- **Course:** Diploma in ICT: Applications Development
- **Module:** Project Presentation 3
- **Module Code:** PRP370S / PRP372S

---

## Project Overview
This portfolio documents the Entrepreneurial Work-Integrated Learning (WIL) project completed for Black Elegance Group (B.E.Group). The project involved designing and developing a business concept, organising feature requirements into structured backlogs and sprints, and tracking progress through Agile project management practices.

**B.E. Cortege** is a premium, community-centred e-hailing web and mobile application engineered for the Black Elegance Group community and luxury event-goers in Cape Town. It addresses the lack of high-end, tailored ride services in South Africa by allowing riders to select their preferred chauffeur, travel in synchronised multi-car convoys to events, and configure personalized travel needs (including dedicated accessibility support, a custom Ride Signature, and a community loyalty programme). The initial launch scope targets major hubs in Cape Town (V&A Waterfront, Camps Bay, Bo-Kaap, Cape Town Stadium, Table Mountain, and Cape Town International Airport).

---

## Technology Stack

### Frontend & Client Development
- **React 18 & Vite 8** — Powers the fast, component-driven client architecture and state handling.
- **React Router (`react-router-dom`)** — Implements single-page application (SPA) client-side routing.
- **Tailwind CSS & CSS Variables** — Delivers a responsive dark-mode UI styled to the B.E.Group brand palette (teal, blue, and warm accent).
- **Leaflet & Esri Map Tiles** — Provides map rendering, interactive location picking, and vehicle tracking visualizations.
- **OSRM & Nominatim** — Facilitates OpenStreetMap-based address geocoding and real-distance route calculations.
- **Capacitor** — Packages the web application for native Android mobile deployment.

### Backend & Data Architecture
- **Supabase / PostgreSQL** — Cloud relational persistence managing schemas for `profiles`, `member_accounts`, `drivers`, `trips`, `ratings`, and `events` with Row Level Security (RLS).
- **Java & Spring Boot (Planned Architecture)** — RESTful microservice skeleton generated via Maven for enterprise domain service expansion.
- **Local State & Client Storage** — Browser-based state management and persistent local storage caching for immediate offline demo capabilities.
- **Security & POPIA Compliance** — Card tokenisation mask (storing only card brand and last 4 digits; CVV/full PAN never saved) and strict personal data handling.

### Hosting & DevOps
- **GitHub** — Version control, collaborative branch management, and portfolio documentation.
- **Netlify** — Production automated CI/CD pipeline building from the SPA distribution with custom redirect handling.

---

## Project Links
- **Live Application:** [B.E. Cortege on Netlify](https://becortege.netlify.app) *(Update with your live URL if different)*
- **GitHub Repository:** [Emeritus-Dev/beCortege](https://github.com/Emeritus-Dev/beCortege)
- **Project Board:** [B.E. Cortege on Trello](https://trello.com) *(Insert your Trello board URL)*

---

## Portfolio Sections

### 1. Agile Team Charter
The team charter defines our shared mission, communication channels, working agreements, and Definition of Done (DoD).
- [View Evidence](./01-agile-team-charter/evidence.md)
- [Reflection](./01-agile-team-charter/reflection.md)

### 2. User Stories and Tasks
Four end-user-centred user stories broken down into granular engineering tasks and UI flows.
- [View Evidence](./02-user-stories-and-tasks/evidence.md)
- [Reflection](./02-user-stories-and-tasks/reflection.md)

### 3. Product Backlog
Prioritized catalogue of features organised through MoSCoW prioritization, data schemas, and technical implementation evidence.
- [View Evidence](./03-product-backlog/evidence.md)
- [Reflection](./03-product-backlog/reflection.md)

### 4. Sprint Backlog
Tracking development progress across five focused sprints (Foundation, Core Ride Flow, Chauffeur Circle, Inclusion & Payments, and Production Polish).
- [View Evidence](./04-sprint-backlog/evidence.md)
- [Reflection](./04-sprint-backlog/reflection.md)

### 5. Agile Logbook
Documented stand-up cadences, Trello Kanban tracking, sprint reviews, and actionable sprint retrospective lessons.
- [View Evidence](./05-agile-logbook/evidence.md)
- [Reflection](./05-agile-logbook/reflection.md)
