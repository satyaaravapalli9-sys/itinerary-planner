# Itinerary Planner - Smart Tour Recommendation System

A modern Java web application that recommends personalized tour packages based on user preferences. Built using Vaadin Flow, Spring Boot, and MongoDB.

---

## Features

- User Authentication (Login / Logout)
- Personalized Tour Recommendations
- Trip Type Filtering (Adventure, Relaxation, Cultural, etc.)
- Preference Management (budget, dates, accommodation, food)
- Dynamic Package Display using Vaadin Cards
- Responsive UI built entirely in Java (Vaadin Flow)
- Admin/Custom control over tour packages via MongoDB

---

## Tech Stack

| Layer | Technology |
|-------|------------|
| UI | Vaadin Flow (Java-based UI framework) |
| Backend | Spring Boot (REST-ready) |
| Database | MongoDB (NoSQL) using Spring Data |
| Styling | Custom CSS with CSS Variables |
| Authentication | Custom AuthService |
| Build Tool | Maven |
| Language | Java 17+ |

---

## Project Structure

```
src/
|-- main/
|   |-- java/
|   |   |-- org.vaadin.example/
|   |   |   |-- model/               # Data models (UserPreferences, TourPackage)
|   |   |   |-- repositories/        # MongoDB Repositories
|   |   |   |-- service/             # Filtering & Auth Services
|   |   |   |-- layout/              # MainLayout (Sidebar, Navigation)
|   |   |   `-- views/               # UI Views (Dashboard, Preferences, etc.)
|   `-- resources/
|       `-- application.properties   # MongoDB config
```

---

## Getting Started

### 1. Clone the Repository
```bash
git clone https://github.com/satya-kumar/itinerary-planner.git
cd itinerary-planner
```

### 2. Configure MongoDB
Set your MongoDB URI in application.properties:
```properties
spring.data.mongodb.uri=mongodb://localhost:27017/itinerary_planner
```

### 3. Run the App
Use your IDE or terminal:
```bash
./mvnw spring-boot:run
```

Access the app at: http://localhost:8080

---

## Test Data

- Tour packages and preferences can be seeded via MongoDB Compass or CLI.
- Sample package structure:
```json
{
  "packageId": "goa_adventure_3d_15k",
  "destination": "Goa",
  "budgetRange": [10000, 15000],
  "tripType": "Adventure",
  "tripDuration": 3,
  "accommodation": {
    "type": "Resort",
    "budgetAllocation": 5000,
    "ratings": [3, 4],
    "amenities": ["WiFi", "Breakfast"]
  }
}
```

---

## Future Enhancements

- Google Maps Integration for destinations
- AI-powered smart recommendations
- Custom Itinerary Planner

---

## Maintainer

**Satya Kumar**
Java Full Stack Developer | AWS | AI | SRE
Email: satyaaravapalli9@gmail.com

### About the Developer
I am a Java Full Stack Developer with over 5 years of experience building and supporting production systems using Java, Spring Boot, React, AWS, and Kubernetes. My background includes extensive work with microservices, distributed systems, and Site Reliability Engineering. I focus on delivering end-to-end solutions that emphasize system stability, performance, and deployment reliability in modern cloud environments.