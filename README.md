# FuelFindr

**Live Application:** https://fuelfindr.app

FuelFindr is a location-based web application that helps users discover nearby fuel stations through geolocation and mapping services. The application is designed to simplify station discovery with a fast, responsive interface while exploring future enhancements such as predictive refueling recommendations.

---

## Preview

> Add screenshots of the landing page, station search results, map view, and mobile interface here.

---

## Overview

FuelFindr was built to improve the experience of finding nearby fuel stations without requiring users to switch between multiple applications. By combining location services with modern web technologies, the application provides a simple and intuitive way to discover relevant stations based on the user's location.

---

## Why I Built This

Many navigation applications show nearby fuel stations, but they are often designed as secondary features. I wanted to build a focused application that provides a clean user experience while serving as a platform for future features such as route-aware recommendations, predictive refueling, and fuel analytics.

---

## Key Features

- Discover nearby fuel stations using browser geolocation
- Display station details and location information
- Responsive interface for desktop and mobile devices
- Integration with Google Places API
- Cloud-hosted deployment
- Designed for future predictive refueling functionality

---

## Technology Stack

**Frontend**

- React
- TypeScript
- Vite
- Tailwind CSS
- shadcn/ui

**Backend & Data**

- Supabase

**APIs**

- Google Places API
- Browser Geolocation API

**Infrastructure**

- Cloudflare

---

## Architecture

```text
User
   │
   ▼
React + Vite Frontend
   │
   ├── Google Places API
   │
   └── Supabase
          │
          ▼
Location Processing & Station Data
          │
          ▼
Interactive Fuel Station Results
```

---

## My Role

This is an independently developed project where I was responsible for:

- Designing the application architecture
- Developing the frontend
- Integrating third-party APIs
- Configuring backend services
- Deploying the application
- Improving the overall user experience

---

## Challenges

Some of the engineering challenges involved:

- Handling browser location permissions
- Managing third-party API usage efficiently
- Building a responsive interface across devices
- Designing the application for future scalability

---

## Future Enhancements

- Route-aware station recommendations
- Fuel price comparison
- Predictive refueling suggestions
- User accounts and saved stations
- Driving analytics
- EV charging station support

---

## Source Code

The production implementation is maintained in a private repository because it contains proprietary implementation details, backend configuration, and integrations with third-party services.

This repository is intended to showcase the project's architecture, functionality, and design. Additional implementation details can be discussed during interviews.

---

## Author

**Saad Bebal**

Portfolio: https://www.saadbebal.com

LinkedIn: https://linkedin.com/in/saad-bebal-a5a582268
