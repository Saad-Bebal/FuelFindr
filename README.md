# FuelFindr

Live app: [fuelfindr.app](https://fuelfindr.app/)

This repository is private to protect API keys and credentials used in the project. Reach out if you'd like a code walkthrough or live demo.

A location-based web application that helps users discover nearby fuel stations in real time, compare pricing and availability, and predict when they'll next need to refuel based on their driving patterns.

---

## Preview

<!-- Add screenshots here, e.g.: -->
<!-- ![FuelFindr home screen](./screenshots/home.png) -->

*(Screenshots coming soon — try the [live app](https://fuelfindr.app/) in the meantime.)*

---

## The Problem

Drivers often default to the first or nearest gas station out of habit, missing better prices or more convenient options just minutes away. FuelFindr surfaces real-time station data and turns "where should I fill up" into a data-informed decision instead of a guess.

## Approach

- Pull live station data (location, ratings, availability) via the Google Places API rather than maintaining a static, quickly-outdated database.
- Layer a lightweight predictive model on top of driving pattern and fuel usage data to estimate a user's next likely refuel point, rather than only reacting to a manual search.
- Build the front end with React, Vite, shadcn/ui, and Tailwind CSS for a fast, component-driven UI, backed by Supabase for auth, data storage, and real-time sync.
- Deploy behind Cloudflare for DNS and edge performance.

## Architecture

```
User (browser)
      |
      v
React + Vite front end (shadcn/ui, Tailwind)
      |
      |--> Google Places API  -> live station data (location, ratings, availability)
      |
      \--> Supabase            -> auth, user data, usage history
                    |
                    v
          Predictive refuel logic -> estimated next fill-up point
```

## Challenges and Tradeoffs

- Balancing live-data freshness against API cost and rate limits — tuned how often station data is re-fetched vs. cached client-side to keep the app responsive without over-calling the Google Places API.
- Designing the predictive refuel model with limited historical data per user — relied on driving-pattern heuristics early on rather than a data-hungry ML model, with room to make it more sophisticated as usage data accumulates.

## Results

<!-- Add real metrics here if you have them, e.g.: -->
<!-- - X active users since launch -->
<!-- - Average station lookup response time: Xms -->
<!-- - X% of users returned within a week -->

## Tech Stack

**Frontend:** React, TypeScript, Vite, shadcn/ui, Tailwind CSS
**Backend/Data:** Supabase (Auth, Postgres, real-time)
**APIs:** Google Places API
**Infrastructure:** Cloudflare (DNS)

---

## About This Repo

The source code is kept private since it contains live API keys and database credentials. If you'd like to see the code directly, walk through the architecture, or get a live demo, reach out — happy to share more.

## Author

**Saad Bebal**
[Portfolio](https://www.saadbebal.com) · [LinkedIn](https://linkedin.com/in/saad-bebal-a5a582268)   │
   ▼
Browser Geolocation
   │
   ▼
Google Places API
   │
   ▼
Process Station Data
   │
   ▼
Display Nearby Fuel Stations
```

---

## Screenshots

### Home Page

![Home Page](screenshots/home-page.png)

---

### Nearby Fuel Stations

![Nearby Stations](screenshots/search-results.png)

---

### Station Details

![Station Details](screenshots/station-details.png)

---

### Map View

![Map View](screenshots/map-view.png)

---

### Mobile Experience

![Mobile View](screenshots/mobile-view.png)

---

## My Contributions

- Designed and developed the complete application
- Built the frontend interface and responsive layouts
- Integrated Google Places API for nearby station discovery
- Implemented browser geolocation functionality
- Configured Supabase backend services
- Managed deployment and production configuration
- Improved overall user experience and application performance

---

## Challenges

During development, several technical challenges were addressed, including:

- Managing browser location permissions
- Handling external API responses efficiently
- Optimizing performance across devices
- Creating a responsive user interface
- Designing a scalable application architecture

---

## Future Enhancements

Future improvements planned for FuelFindr include:

- Smarter fuel price comparison
- Route-based fuel recommendations
- Personalized user accounts
- Favorite stations
- Historical fuel usage analytics
- EV charging station support

---

## Source Code

The production implementation is maintained in a private repository.

The application contains proprietary implementation details, backend services, deployment configuration, and integrations with third-party platforms that are not included in this public repository.

This repository is intended to showcase the project's functionality, architecture, technology stack, and overall design. Additional implementation details can be discussed during interviews.

---

## Contact

**Portfolio**

https://saadbebal.com

**LinkedIn**

https://linkedin.com/in/saad-bebal-a5a582268

**Email**

saadbebal.work@gmail.com
