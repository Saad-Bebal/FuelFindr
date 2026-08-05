# FuelFindr

**Live Application:** https://fuelfindr.app

FuelFindr is a location-based web application that helps users discover nearby fuel stations through geolocation and mapping services. The application is designed to simplify station discovery with a fast, responsive interface while exploring future enhancements such as predictive refueling recommendations.

---

## Preview

<img width="1495" height="752" alt="image" src="https://github.com/user-attachments/assets/b800eee7-ca1e-44e1-814b-95789c7eb9d0" />
<img width="1489" height="858" alt="image" src="https://github.com/user-attachments/assets/1b542aa1-3937-4277-8124-7070c531652f" />
<img width="1496" height="858" alt="image" src="https://github.com/user-attachments/assets/d77bafa9-3e49-4a34-82c0-ae1916aaf6be" />
<img width="1489" height="703" alt="image" src="https://github.com/user-attachments/assets/28e0f999-6a51-4749-8b66-becd88b0f529" />
<img width="1492" height="654" alt="image" src="https://github.com/user-attachments/assets/9b2d8efb-7e8b-4a17-88e3-3f113fd53b53" />


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
