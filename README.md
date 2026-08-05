# ⛽ FuelFindr

**Live app:** [fuelfindr.app](https://fuelfindr.app/)

> 🔒 This repository is private to protect API keys and credentials used in the project. Feel free to reach out for a code walkthrough or live demo.

A location-based web application that helps users discover nearby fuel stations in real time, compare pricing and availability, and predict when they'll next need to refuel based on their driving patterns.

---

## 📸 Preview

<!-- Add 2-4 screenshots or a short GIF here, e.g.: -->
<!-- ![FuelFindr home screen](./screenshots/home.png) -->
<!-- ![Station detail view](./screenshots/station-detail.png) -->

*(Screenshots coming soon — try the [live app](https://fuelfindr.app/) in the meantime.)*

---

## 🎯 The Problem

Drivers often default to the first or nearest gas station out of habit, missing better prices or more convenient options just minutes away. FuelFindr surfaces real-time station data and turns "where should I fill up" into a data-informed decision instead of a guess.

## 🧠 Approach

- Pull live station data (location, ratings, availability) via the **Google Places API** rather than maintaining a static, quickly-outdated database.
- Layer a lightweight predictive model on top of driving pattern and fuel usage data to estimate a user's next likely refuel point, rather than only reacting to a manual search.
- Build the front end with **React + Vite + shadcn/ui + Tailwind CSS** for a fast, component-driven UI, backed by **Supabase** for auth, data storage, and real-time sync.
- Deploy behind **Cloudflare** for DNS and edge performance.

## 🏗 Architecture

```
User (browser)
      │
      ▼
React + Vite front end (shadcn/ui, Tailwind)
      │
      ├──► Google Places API  → live station data (location, ratings, availability)
      │
      └──► Supabase            → auth, user data, usage history
                    │
                    ▼
          Predictive refuel logic → estimated next fill-up point
```

## 🧩 Challenges & Tradeoffs

- **Balancing live-data freshness vs. API cost/rate limits** — tuned how often station data is re-fetched vs. cached client-side to keep the app responsive without hammering the Google Places API.
- **Designing the predictive refuel model with limited historical data per user** — had to lean on driving-pattern heuristics early on rather than a data-hungry ML model, with room to make it more sophisticated as usage data accumulates.
