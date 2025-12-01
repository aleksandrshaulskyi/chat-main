# Chat index repository.

This is my main demo project that is used for the representation of my skills.

⚠️ Disclaimer
This project is under active development. Some known issues and rough edges are expected and will be polished soon.
For development convenience, database containers are temporarily located next to their corresponding microservices.

## 🚀 Overview

This repository serves as the central entry point for my distributed chat system — a real-time messaging platform built as a set of independently deployable microservices, each responsible for a well-defined domain:
- Authentication
- Transportation (WebSocket + message routing)
- Messaging (persistent storage + event flow)
- Monitoring
- Logging
- Shared infrastructure
- React/TypeScript client

The goal of this repository is to link the ecosystem together, track updates across the services, and provide a simple way to run the full application locally.

## 🧩 Architecture Highlights

Clean Architecture + DDD-inspired boundaries, no business logic in frameworks

- Event-driven message flow through RabbitMQ (publisher confirms, ACK, DLX/TTL retries
- Sharded event delivery per-user using consistent hashing
- Transactional outbox for reliable message propagation
- MongoDB + PostgreSQL depending on service role
- Prometheus + OpenTelemetry + Grafana + Tempo for monitoring and tracing
- ELK stack (Filebeat → Logstash → Elasticsearch → Kibana) for structured logs
- React/TypeScript frontend with animated UI and WebSocket integration
- Full Docker-based environment with isolated Compose stacks per service

This platform is intentionally built as a demonstration of my experience in designing distributed, observable, fault-tolerant backend systems.

## Repositories of the project.

Authentication microservice: https://github.com/aleksandrshaulskyi/chat-auth  
Transportation microservice: https://github.com/aleksandrshaulskyi/chat-transportation  
Messaging microservice: https://github.com/aleksandrshaulskyi/chat-messaging  
Shared services: https://github.com/aleksandrshaulskyi/chat-shared-services  
React/Typescript service: https://github.com/aleksandrshaulskyi/chat-frontend  
Monitoring microservice: https://github.com/aleksandrshaulskyi/chat-monitoring  
Logging microservice: https://github.com/aleksandrshaulskyi/chat-logging  

## 💻 Run the Project Locally

  **Prerequisites:** Docker + Docker Compose installed

- Clone all repositories listed above.

- Switch into chat-shared-services.

- Run:

```docker-compose up -d --build```

- Repeat the same for all other repositories (auth, transportation, messaging, monitoring, logging, frontend).

After all stacks start, the application will be available at:

**👉 http://localhost:80/**

## Recent updates.

Not yet released.
