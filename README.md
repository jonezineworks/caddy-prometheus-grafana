# caddy-prometheus-grafana

Instructions
Set up the environment:

Save docker-compose.yml, Caddyfile, and prometheus.yml in the same directory.
Start the stack:

bash
Copiar código
docker-compose up -d
Access the services:

Caddy: Accessible on port 8888 (proxying to 3443).
Prometheus: http://localhost:9090
Grafana: http://localhost:3000
Default credentials: admin / admin
Add Prometheus to Grafana:

Log into Grafana.
Add a new data source: Prometheus.
URL: http://prometheus:9090.
Visualize metrics:

Create dashboards in Grafana to visualize Caddy metrics (e.g., HTTP requests, response durations, etc.).

add grafana dashboards to visualize caddy data