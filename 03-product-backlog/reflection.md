
# Product Backlog Reflection

## Situation
At the start of engineering B.E. Cortege, we had an ambitious scope of luxury transport features—including multi-car convoys, driver selection, accessibility profiles, complex map routing, and loyalty tiers. Without a disciplined framework to prioritize and structure these requirements, our team risked fragmenting engineering effort across secondary features before establishing a resilient, testable foundation.

## Task
As Full-Stack & System Lead, my task was to curate the complete Product Backlog, classify deliverables using the MoSCoW prioritization framework (Must Have, Should Have, Could Have, Won't Have), model our underlying PostgreSQL/Supabase database schema, and align engineering backlog items directly with verifiable Trello cards and technical assets.

## Action
I structured the product requirements into five primary epics:
1. **Foundation & Authentication:** Essential onboarding, secure login, password recovery, and POPIA consent.
2. **Core Ride Flow:** Map rendering with Leaflet, geocoding via Nominatim, road network paths using OSRM, and fare calculation.
3. **Chauffeur Directory & Trust:** Driver profiles, verification badges, performance metrics, and post-trip ratings.
4. **Inclusive Travel & Rewards:** Accessibility preferences, plain-language driver briefings, and 3D tier membership cards.
5. **Production Polish:** Mobile responsiveness, Netlify CI/CD pipeline integrity, and Capacitor Android runtime packaging.

I established clear database entity relationships across `profiles`, `member_accounts`, `drivers`, `trips`, and `ratings`. For each item, I defined technical constraints and linked each priority bucket directly to our Trello board tracking.

## Result
The structured Product Backlog gave our team clear visibility into development priorities, ensuring that our core ride engine and routing architecture were fully functional before implementing secondary tier animations. I learned that an effective backlog is not merely a feature wishlist, but an active architectural blueprint that balances user value against technical feasibility.
