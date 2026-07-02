# Grafana & Prometheus Quick Start

A Docker Compose-based monitoring stack that deploys **Grafana** alongside multiple **Prometheus** instances with a simple and consistent setup.

This project provides a quick way to bring up a monitoring environment whenever Grafana and Prometheus are required without the need for additional infrastructure or orchestration.

---

## Features

- Grafana dashboard service
- Four independent Prometheus instances
- Docker Compose deployment
- Persistent Grafana storage
- Lightweight and easy to deploy
- Simple configuration using YAML files

---

## Prerequisites

Before deploying the stack, ensure the following requirements are met:

- Linux server
- Docker
- Docker Compose (v2)

Verify the installation:

```bash
docker --version
docker compose version
```

---

## Project Structure

```text
.
├── compose.yaml
├── prometheus-1.yml
├── prometheus-2.yml
├── prometheus-3.yml
├── prometheus-4.yml
└── README.md
```

---

## Deployment

Clone the repository:

```bash
git clone <repository-url>
cd <repository-name>
```

Start the monitoring stack:

```bash
docker compose up -d
```

Verify that all containers are running:

```bash
docker ps
```

---

## Services

| Service      | Endpoint              |
| ------------ | --------------------- |
| Grafana      | http://SERVER_IP:3000 |
| Prometheus 1 | http://SERVER_IP:9091 |
| Prometheus 2 | http://SERVER_IP:9092 |
| Prometheus 3 | http://SERVER_IP:9093 |
| Prometheus 4 | http://SERVER_IP:9094 |

Replace `SERVER_IP` with the IP address or hostname of your server.

---

## Managing the Stack

Stop all services:

```bash
docker compose down
```

Stop services and remove volumes:

```bash
docker compose down -v
```

Restart the stack:

```bash
docker compose restart
```

View container logs:

```bash
docker compose logs -f
```

---

## Configuration

Each Prometheus instance loads its configuration from its corresponding YAML file:

- `prometheus-1.yml`
- `prometheus-2.yml`
- `prometheus-3.yml`
- `prometheus-4.yml`

Grafana data is stored in a persistent Docker volume to preserve dashboards and configuration across container restarts.

---

## Notes

- Designed for fast and straightforward deployment.
- Easy to customize by editing the Prometheus configuration files.
- Suitable for environments where a monitoring stack needs to be available with minimal setup.
