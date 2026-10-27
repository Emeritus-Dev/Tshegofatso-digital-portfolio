
# User Stories and Tasks Evidence

This page presents the documented user stories, engineering task breakdowns, user interface implementations, and Trello traceability for **B.E. Cortege**.

---

## 1. Request a Ride and Live Driver Tracking

### 1.1 User Story
> **As a rider, I want to search for my pickup and destination and watch my driver arrive on a live interactive map, so that I know precisely when and where my ride will arrive.**

### 1.2 Task Breakdown
- [x] **Task 1.1:** Build the Home screen layout with route search input boxes and integrate OpenStreetMap Nominatim for live place geocoding.
- [x] **Task 1.2:** Integrate the OSRM (Open Source Routing Machine) engine to fetch true road network paths, calculate route geometry, and estimate trip fares.
- [x] **Task 1.3:** Animate vehicle marker progression along the calculated route coordinates with dynamic ETA and remaining distance countdowns.
- [x] **Task 1.4:** Implement state machine transitions for the complete ride lifecycle: `searching`, `approaching`, `arrived`, `in_trip`, and `rating`.
- [x] **Task 1.5:** Enable dynamic pickup and destination editing with saved frequent places (e.g., Waterfront, Camps Bay, CPUT Campus).

### 1.3 Technical Architecture & Traceability
- **Frontend Component:** `src/pages/Home.jsx`, `src/components/MapRoute.jsx`
- **Mapping Libraries:** Leaflet API, Esri Vector Tile Layer, OSRM Routing Service
- **Trello Card Reference:** [Ride Request and Live Tracking](https://trello.com) *(Update with your card link)*

---

## 2. Driver Reputation and Chauffeur Selection

### 2.1 User Story
> **As a rider, I want to choose a specific chauffeur and review their profile, credentials, and passenger ratings, so that I can travel with someone I trust.**

### 2.2 Task Breakdown
- [x] **Task 2.1:** Create responsive driver preview cards featuring vehicle tier, photo, verification badges, and real-time online status.
- [x] **Task 2.2:** Build an interactive driver profile sheet displaying completed trips, safety badges, language proficiencies, and rating breakdowns.
- [x] **Task 2.3:** Implement a post-trip feedback interface featuring dynamic star ratings and positive tag selections (e.g., *Smooth Drive*, *Punctual*).
- [x] **Task 2.4:** Build the "My Chauffeur Circle" feature allowing passengers to favourite preferred drivers for prioritized matching.
- [x] **Task 2.5:** Create reusable UI rating components supporting half-star rendering and custom luxury badge icons.

### 2.3 Technical Architecture & Traceability
- **Frontend Component:** `src/components/DriverCard.jsx`, `src/components/DriverProfileModal.jsx`
- **State Handling:** Active driver selection, cached rating metrics, and Chauffeur Circle local persistence.
- **Trello Card Reference:** [Driver Profiles and Ratings](https://trello.com) *(Update with your card link)*

---

## 3. Inclusive Travel & Accessibility Support

### 3.1 User Story
> **As a rider with accessibility needs, I want to communicate my travel requirements to my chauffeur in advance, so that every trip is safe, dignified, and comfortable.**

### 3.2 Task Breakdown
- [x] **Task 3.1:** Build an Accessibility Profile interface featuring an explicit consent toggle for sharing preferences with drivers (POPIA compliant).
- [x] **Task 3.2:** Implement preference categories for mobility assistance (folding wheelchair stowage), hearing support, vision accommodations, and a low-sensory "Calm Ride" mode.
- [x] **Task 3.3:** Generate an automated, non-clinical driver briefing that outlines practical passenger needs without disclosing private medical diagnoses.
- [x] **Task 3.4:** Add a Trusted Contacts module allowing riders to share live trip progress, vehicle details, and GPS tracking via SMS/WhatsApp.
- [x] **Task 3.5:** Implement high-contrast UI themes, customizable text size scaling, and reduced-motion display options.

### 3.3 Technical Architecture & Traceability
- **Frontend Component:** `src/pages/AccessibilitySettings.jsx`, `src/components/DriverBriefingCard.jsx`
- **Data Compliance:** Sensitive health data is never stored; only practical ride accommodations are shared.
- **Trello Card Reference:** [Accessibility and Inclusive Travel](https://trello.com) *(Update with your card link)*

---

## 4. Loyalty Membership & Account Management

### 4.1 User Story
> **As a rider, I want to earn loyalty points, save payment methods securely, and manage my profile preferences, so that I benefit from using the service regularly.**

### 4.2 Task Breakdown
- [x] **Task 4.1:** Design 3D-styled Bronze, Silver, and Gold digital membership cards with interactive flip animations and barcode identifiers.
- [x] **Task 4.2:** Build the membership progression ladder and an "Invite a Fan" referral reward engine.
- [x] **Task 4.3:** Build a secure Payment Management interface with real-time card validation (Luhn algorithm check, brand detection, expiry validation, and CVV masking).
- [x] **Task 4.4:** Implement localized multilingual support with a regional language switcher (English, isiZulu, and Sepedi).
- [x] **Task 4.5:** Build an "Explore" portal highlighting curated Cape Town destinations, event convoys, and digital Passport travel stamps.

### 4.3 Technical Architecture & Traceability
- **Frontend Component:** `src/pages/Membership.jsx`, `src/pages/PaymentMethods.jsx`
- **Security Constraint:** Full PAN and CVVs are discarded immediately following validation; only tokenized last-4 digits are persisted.
- **Trello Card Reference:** [Membership Tiers and Payments](https://trello.com) *(Update with your card link)*

---

## 5. Requirements Traceability Matrix

| User Story | Primary Component | Acceptance Criterion | Verification Status |
| :--- | :--- | :--- | :--- |
| **US-1: Ride & Tracking** | `Home.jsx` / Leaflet | Route renders with turn coordinates and simulated driver movement | Verified (UI Demo) |
| **US-2: Chauffeur Circle** | `DriverCard.jsx` | Chauffeur credentials, vehicle details, and ratings display accurately | Verified (UI Demo) |
| **US-3: Accessibility** | `Accessibility.jsx` | Preferences generate driver briefing without medical data exposure | Verified (UI Demo) |
| **US-4: Loyalty & Pay** | `Membership.jsx` | Tier calculations update points balance and apply card masking | Verified (UI Demo) |
