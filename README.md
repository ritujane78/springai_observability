# SpringAI Observability 

SpringAI Observability is a Spring Boot–based project that exposes **Spring AI–related metrics** and makes them available to popular observability tools such as **Prometheus** and **Grafana**.

The goal of this project is to demonstrate how AI-powered Spring applications can be monitored, measured, and analyzed using industry-standard observability tooling.

---

## Features

- Exposes **Spring AI metrics** via **Spring Boot Actuator**
- Metrics compatible with **Prometheus**
- Preconfigured **Grafana dashboards** (screenshots attached)
- Fully containerized observability stack using **Docker**
- Designed for experimentation and extension 

---

## 🛠 Tech Stack

- **Spring Boot**
- **Spring AI**
- **Spring Boot Actuator**
- **Micrometer**
- **Prometheus**
- **Grafana**
- **Docker & Docker Compose**

---

## Observability Stack

The following tools are provided via Docker images:

| Tool        | Docker Image          | Port |
|------------|-----------------------|------|
| Prometheus | `prom/prometheus`     | 9090 |
| Grafana    | `grafana/grafana`     | 3000 |

---

##  Getting Started

### Prerequisites
- Java 21+
- Spring AI: 1.1.2
- Maven
- Docker & Docker Compose

---

### Accessing the tools

1. Actuator
```bash
http://localhost:8080/actuator
```
2. Metrics
```bash
http://localhost:8080/actuator/metrics
http://localhost:8080/actuaor/metrics/<metric_name>
http://localhost:8080/actuaor/metrics/<metric_name>?tag=<tag_name>:<value>
```
---

Clone the repository:
   ```bash
   git clone <repository-url>
   cd springai-observability
```