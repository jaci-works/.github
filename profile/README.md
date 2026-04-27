# JACI

**JACI** is a portfolio project composed of multiple applications that work together to support field data collection, environmental monitoring, and botanical/phenological analysis.

The system is designed around two main applications:

- **JACI Backend** — a Spring Boot application that provides the administrative web panel, REST API synchronization endpoints, authentication, database access.
  
- **JACI Android** — a native Android application used for offline field data collection, later synchronized with the backend API.

The goal of this project is to demonstrate a complete real-world system using modern backend architecture, mobile development, relational databases, containerized infrastructure, and clean project organization usimg hexagonal architecture.

---

## Project Architecture

```text
JACI
├── Backend - Spring Boot
│   ├── Admin web panel
│   ├── REST API
│   ├── Authentication and authorization
│   ├── PostgreSQL persistence
│   └── Future synchronization/event processing
│
└── Android App
    ├── Offline data collection
    ├── Local storage
    └── Backend synchronization
