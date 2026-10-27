
# User Stories and Tasks Reflection

## Situation
In developing B.E. Cortege, we had to capture complex luxury e-hailing journeys spanning on-demand ride booking, driver reputation, inclusive travel accommodations, and client loyalty rewards. Without an explicit, user-centred breakdown, there was a substantial risk of scope creep and building features that prioritized backend complexity over the direct experiential needs of our passengers.

## Task
My responsibility was to define four core end-user stories representing the primary rider journeys, deconstruct each story into five concrete implementation tasks, and establish clear traceability between user requirements, Trello backlog tracking, and our React component interfaces.

## Action
I implemented the standard Agile narrative structure—**"As a [user], I want [capability] so that [benefit]"**—across four distinct functional areas:
1. **Core Ride Flow & Tracking:** Deconstructed into map initialization (Leaflet), routing queries (OSRM), driver car animation, ride state transitions, and dynamic destination updating.
2. **Chauffeur Selection & Trust:** Deconstructed into driver status cards, verified credentials, rating sheets, post-ride feedback loops, and Chauffeur Circle saved lists.
3. **Inclusive Travel & Accessibility:** Designed a dedicated profile system supporting mobility, vision, hearing, and calm-ride needs with POPIA-compliant driver briefings.
4. **Loyalty Tiers & Secure Payments:** Structured membership card flip animations, referral progression, and masked card input validation.

For each story, I linked the engineering tasks to our Trello board and connected the requirements to specific React UI components (`Home.jsx`, `DriverCard.jsx`, `AccessibilityProfile.jsx`, and `MembershipCard.jsx`).

## Result
Structuring user stories in this disciplined manner ensured that every interface component directly addressed a real passenger requirement. Traceability between Trello tasks and frontend code simplified debugging and sprint demos. This practice reinforced that software requirements should always be driven by user value rather than abstract technical ambition.
