# Crypto Trading Platform

This repository contains a microservice architecture for algorithmic trading and data analytics. Each service is isolated so components can be developed and scaled independently.

## Directory Overview

- `.github/` – GitHub configuration and workflows.
- `.kube/` – Kubernetes manifests for deployment.
- `data/` – storage for datasets and market data.
- `docs/` – additional project documentation.
- `scripts/` – helper scripts used across the project.
- `services/` – individual service implementations.
  - `01-data-collection/` – collects raw market data.
  - `02-indicator-engine/` – computes trading indicators.
  - `03-signal-generation/` – creates trading signals.
  - `04-execution-engine/` – executes orders on exchanges.
  - `05-order-manager/` – manages order lifecycle.
  - `06-risk-manager/` – enforces risk rules.
  - `07-trade-logger/` – persists executed trade data.
  - `08-performance-tracker/` – tracks portfolio metrics.
  - `09-report-service/` – generates periodic reports.
  - `10-alert-service/` – handles alerting and notifications.
  - `11-dashboard-frontend/` – user facing dashboard UI.
  - `12-dashboard-backend/` – API backend for the dashboard.
- `shared/` – common libraries shared across services.
  - `common/` and `utils/` – reusable functions and classes.

## Development

Build and run services locally with Docker Compose:

```bash
docker-compose build
docker-compose up
```
