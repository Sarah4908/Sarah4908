<div align="center">
# Sarah Susan George

**Computer Science Undergraduate**

Backend Systems · Distributed Systems · Machine Learning

[![Email](https://img.shields.io/badge/Email-sarahsusan.george.4908%40gmail.com-0d1117?style=flat-square&logo=gmail&logoColor=white&labelColor=161b22)](mailto:sarahsusan.george.4908@gmail.com)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-sarah--susan--george-0d1117?style=flat-square&logo=linkedin&logoColor=white&labelColor=161b22)](https://www.linkedin.com/in/sarah-susan-george-b4114830b)
[![GitHub](https://img.shields.io/badge/GitHub-Sarah4908-0d1117?style=flat-square&logo=github&logoColor=white&labelColor=161b22)](https://github.com/Sarah4908)

</div>

---

## About

I'm a Computer Science undergraduate focused on building robust backend systems and exploring the intersection of distributed architecture and machine learning. I enjoy working across the full stack — from designing service-oriented architectures to training ML models and integrating them into production pipelines.

Currently deepening my knowledge in machine learning fundamentals, distributed systems design, and open-source collaboration.

---

## Featured Projects

### [Satellite Telemetry Monitoring & Anomaly Detection System](https://github.com/Sarah4908)

> A containerised, multi-service telemetry processing platform for real-time anomaly detection and contextual fault explanation.

Accepts manually submitted telemetry readings (temperature, voltage, altitude) via a dashboard form, scores them for anomalies using a trained ML model, and retrieves the 2 most similar fault descriptions via an RAG pipeline.

**Architecture highlights:**
- Spring Boot orchestrates all service communication — the frontend never calls the ML service directly
- FastAPI ML service runs an `IsolationForest` model (300 estimators) with per-satellite stateful feature engineering: `temp_delta`, `volt_delta`, `rolling_temp_mean`
- RAG layer uses `sentence-transformers/all-MiniLM-L6-v2` + FAISS for offline retrieval, with GPT-4o-mini for explanation generation
- PostgreSQL persists telemetry history across restarts; ML service seeds its in-memory state from the DB on startup
- Full Docker Compose setup reduces a four-runtime stack (Java, Python, Node, PostgreSQL) to a single command

**Tech stack:**

![Java](https://img.shields.io/badge/Java-0d1117?style=flat-square&logo=openjdk&logoColor=white&labelColor=161b22)
![Spring Boot](https://img.shields.io/badge/Spring_Boot-0d1117?style=flat-square&logo=springboot&logoColor=white&labelColor=161b22)
![FastAPI](https://img.shields.io/badge/FastAPI-0d1117?style=flat-square&logo=fastapi&logoColor=white&labelColor=161b22)
![Python](https://img.shields.io/badge/Python-0d1117?style=flat-square&logo=python&logoColor=white&labelColor=161b22)
![React](https://img.shields.io/badge/React-0d1117?style=flat-square&logo=react&logoColor=white&labelColor=161b22)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-0d1117?style=flat-square&logo=postgresql&logoColor=white&labelColor=161b22)
![Docker](https://img.shields.io/badge/Docker-0d1117?style=flat-square&logo=docker&logoColor=white&labelColor=161b22)
![scikit-learn](https://img.shields.io/badge/scikit--learn-0d1117?style=flat-square&logo=scikitlearn&logoColor=white&labelColor=161b22)

---

### [WebPisi](https://webpisi.onrender.com/)

> A full-stack web application demonstrating backend fundamentals — authentication, session management, and database integration.

**Tech stack:**

![Node.js](https://img.shields.io/badge/Node.js-0d1117?style=flat-square&logo=nodedotjs&logoColor=white&labelColor=161b22)
![Express](https://img.shields.io/badge/Express-0d1117?style=flat-square&logo=express&logoColor=white&labelColor=161b22)
![MongoDB](https://img.shields.io/badge/MongoDB-0d1117?style=flat-square&logo=mongodb&logoColor=white&labelColor=161b22)
![Redis](https://img.shields.io/badge/Redis-0d1117?style=flat-square&logo=redis&logoColor=white&labelColor=161b22)

- bcrypt password hashing and secure credential storage
- Redis-backed session management with protected routing
- Mongoose ODM for MongoDB integration

---

## Open Source

**MDN Web Docs** — Corrected incorrect `load_dotenv()` usage in the Django deployment tutorial, updating the documentation to properly handle environment variable loading with `python-dotenv`.

---

## Tech Stack

| Domain | Technologies |
|---|---|
| **Languages** | Java · Python · JavaScript |
| **Backend** | Spring Boot · FastAPI · Node.js · Express |
| **ML / Data** | Scikit-Learn · FAISS · sentence-transformers |
| **Databases** | PostgreSQL · MongoDB · Redis |
| **Infrastructure** | Docker · Docker Compose · Git |

---

## Currently Learning

- Machine learning fundamentals and model deployment patterns
- Distributed systems architecture and consensus algorithms
- Open-source contribution workflows

---

<div align="center">

*Open to collaboration, feedback, and interesting problems.*

</div>
