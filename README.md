# SRETools

SRE tooling stack for NetDevOps — runs locally via Docker Compose.

## Stack
- **NetBox** — Network source of truth (IPAM + DCIM)
- **Jenkins** — CI/CD pipelines (Day 1, Day 2, Emergency)
- **Ansible** — NETCONF config push to routers
- **pyATS** — Pre/post deployment validation
- **Prometheus + Alertmanager** — Metrics + critical alerting
- **Grafana** — Monitoring dashboards
- **Zammad** — Incident ticketing

## Ports
| Service | URL |
|---------|-----|
| NetBox | http://localhost:8000 |
| Jenkins | http://localhost:8080 |
| Prometheus | http://localhost:9090 |
| Grafana | http://localhost:3000 |
| Alertmanager | http://localhost:9093 |
| Zammad | http://localhost:8090 |

## Usage
```bash
docker compose up -d
docker compose ps
docker compose down
```
