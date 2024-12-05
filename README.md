# caddy-prometheus-grafana

Instructions

Change Configurations:

Configure caddy proxy ports
Configure Prometheus file to target caddy metrics

Start the stack:

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

Import caddy dashboard from grafanaDashboards4caddy
