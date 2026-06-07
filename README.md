# Docker Monitoring Stack

## Overview

This project demonstrates how to deploy a monitoring and observability stack using Docker Compose.

The solution includes:

- Prometheus for metrics collection
- Grafana for visualization and dashboards
- Docker Compose for service orchestration
- GitHub Actions for Continuous Integration (CI)

The objective is to showcase practical DevOps skills related to monitoring, automation, and containerized deployments.

---

## Architecture

```text
Docker Host
│
├── Prometheus
│   └── Collects metrics
│
└── Grafana
    └── Visualizes metrics and dashboards
```

---

## Technologies Used

| Technology | Purpose |
|------------|----------|
| Docker | Containerization |
| Docker Compose | Service orchestration |
| Prometheus | Metrics collection |
| Grafana | Monitoring dashboards |
| GitHub Actions | Continuous Integration |
| Linux | Deployment platform |

---

## Repository Structure

```text
docker-monitoring-stack/
│
├── .github/
│   └── workflows/
│       └── docker-ci.yml
│
├── prometheus/
│   └── prometheus.yml
│
├── docs/
│   ├── architecture.md
│   └── deployment.md
│
├── docker-compose.yml
├── README.md
└── .gitignore
```

---

## Deployment

### Clone Repository

```bash
git clone https://github.com/<your-username>/docker-monitoring-stack.git
cd docker-monitoring-stack
```

### Start Services

```bash
docker compose up -d
```

### Verify Containers

```bash
docker ps
```

Expected containers:

- Prometheus
- Grafana

---

## Access Services

### Grafana

```text
http://localhost:3000
```

Default credentials:

```text
Username: admin
Password: admin
```

### Prometheus

```text
http://localhost:9090
```

---

## CI Pipeline

GitHub Actions automatically validates the Docker Compose configuration on every push and pull request.

Pipeline checks:

- Repository checkout
- Docker Compose validation
- Configuration verification

Workflow file:

```text
.github/workflows/docker-ci.yml
```

---

## Skills Demonstrated

- Containerization
- Monitoring and Observability
- Infrastructure Operations
- Docker Compose
- CI/CD Automation
- GitHub Actions
- Linux Administration

---

## Future Improvements

Planned enhancements:

- Node Exporter integration
- Alertmanager integration
- Custom Grafana dashboards
- Terraform deployment automation
- AWS EC2 deployment
- Kubernetes migration

---

## Author

Yusdel Concepcion

Cloud & DevOps Engineer

