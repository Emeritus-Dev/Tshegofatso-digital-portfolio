# Product Backlog Evidence

This page presents the comprehensive **Product Backlog** for **B.E. Cortege**, including epic structures, MoSCoW prioritization, relational database schema models, and Trello traceability records.

---

## 1. Product Backlog Overview & Objective

The primary objective of the B.E. Cortege backlog is to deliver a reliable, responsive, and luxury-tier e-hailing web and mobile solution tailored to the Black Elegance Group community in Cape Town.

---

## 2. MoSCoW Feature Prioritization

The backlog items are classified into four strategic delivery tiers:

### 2.1 Must Have (P0 — Non-negotiable for Release)
* **Authentication & Profile:** User registration, secure login, password recovery, and POPIA data handling.
* **Geospatial Map Engine:** Leaflet map rendering with Esri satellite/street tiles.
* **Geocoding & Route Calculation:** OpenStreetMap Nominatim place queries and OSRM turn-by-turn road route generation.
* **Dynamic Ride Lifecycle:** State handling across `searching`, `approaching`, `arrived`, `in_trip`, and `rating`.
* **Responsive Architecture:** Fully functional cross-device layout optimized for mobile screens.

### 2.2 Should Have (P1 — High-Value Features)
* **Chauffeur Directory:** Verified driver profile sheets, ratings, safety badges, and language proficiencies.
* **My Chauffeur Circle:** Capability to bookmark trusted drivers for preferred ride matching.
* **Inclusive Accessibility Profile:** Accommodations for mobility, vision, hearing, and calm-ride needs with driver briefings.
* **Loyalty Tiers & Membership:** Interactive 3D Bronze, Silver, and Gold digital cards with referral incentives.
* **Payment Security:** Masked card input validation (Luhn check, expiry, brand detection) preserving zero CVV data.

### 2.3 Could Have (P2 — Desirable Enhancements)
* **Branded Convoy Picker:** Interactive selector to configure 2 to 4 matching luxury vehicles traveling together.
* **Digital Travel Passport:** Curated destination check-ins and digital collectible stamps for Cape Town events.
* **Multilingual Localization:** Dynamic language switcher supporting English, isiZulu, and Sepedi.
* **Brand Splash Intro:** Cinematic animated splash view reflecting B.E.Group luxury branding.

### 2.4 Won't Have (P3 — Deferred to Future Releases)
* Standalone dedicated chauffeur mobile application (simulated driver telemetry utilized currently).
* Production payment gateway processing with live bank clearing.
* Automated real-time telematics hardware integration in vehicles.

---

## 3. Relational Database Architecture

The application persistence layer is architected around a normalized PostgreSQL/Supabase schema design:

### 3.1 Core Entity Schemas

```sql
-- Profiles & Rider Accounts
CREATE TABLE profiles (
    id UUID PRIMARY KEY DEFAULT gen_random_uuid(),
    email TEXT UNIQUE NOT NULL,
    full_name TEXT NOT NULL,
    phone_number TEXT,
    preferred_language TEXT DEFAULT 'English',
    created_at TIMESTAMP WITH TIME ZONE DEFAULT NOW()
);

-- Chauffeur / Driver Entity
CREATE TABLE drivers (
    id UUID PRIMARY KEY DEFAULT gen_random_uuid(),
    full_name TEXT NOT NULL,
    vehicle_model TEXT NOT NULL,
    vehicle_tier TEXT CHECK (vehicle_tier IN ('Cortege Black', 'Cortege SUV', 'Cortege Access', 'Cortege Convoy')),
    license_plate TEXT NOT NULL,
    rating NUMERIC(2,1) DEFAULT 5.0,
    trips_completed INTEGER DEFAULT 0,
    is_verified BOOLEAN DEFAULT TRUE,
    is_online BOOLEAN DEFAULT FALSE
);

-- Trips & Dispatch Records
CREATE TABLE trips (
    id UUID PRIMARY KEY DEFAULT gen_random_uuid(),
    rider_id UUID REFERENCES profiles(id),
    driver_id UUID REFERENCES drivers(id),
    pickup_address TEXT NOT NULL,
    destination_address TEXT NOT NULL,
    fare_amount NUMERIC(8,2) NOT NULL,
    trip_status TEXT CHECK (trip_status IN ('searching', 'approaching', 'arrived', 'in_trip', 'completed', 'cancelled')),
    convoy_count INTEGER DEFAULT 1,
    created_at TIMESTAMP WITH TIME ZONE DEFAULT NOW()
);

-- Accessibility Preferences (POPIA Compliant)
CREATE TABLE accessibility_profiles (
    rider_id UUID PRIMARY KEY REFERENCES profiles(id),
    share_with_driver BOOLEAN DEFAULT FALSE,
    mobility_assistance BOOLEAN DEFAULT FALSE,
    hearing_support BOOLEAN DEFAULT FALSE,
    vision_support BOOLEAN DEFAULT FALSE,
    calm_ride_preferred BOOLEAN DEFAULT FALSE,
    notes TEXT
);
