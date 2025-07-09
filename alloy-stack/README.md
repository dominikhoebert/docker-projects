# Grafana-Alloy System Monitoring Stack

- Alloy: Metrics and Logs collection, pushes to prometheus and loki
- Loki: Logs DB
- Prometheus: Metrics DB
- Grafana: Data Visualisation

## Setup

1. Run compose
2. Open [Grafana Dashboard](http://localhost:3000)
3. Add new prometheus connection: Connections -> Add new Datasource -> search for "prometheus" -> http://prometheus:9090 -> Test & Save
4. Same for Loki -> http://loki:3100

Use Drilldown to look through your data

## Links

- https://grafana.com/docs/alloy/latest/
- https://www.youtube.com/watch?v=E654LPrkCjo
- https://github.com/ChristianLempa/boilerplates/tree/main/docker-compose/alloy
- https://github.com/grafana/alloy-scenarios
