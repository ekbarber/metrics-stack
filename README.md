# Metrics Stack

This is a simple metrics stack

It will spin up InfluxDB, Telegraf, and Grafana.

## Setup
1. Run `docker-compose up -d `
1. Set-up grafana by browsing to  `http://localhost:3000` and use `admin` for both user and password.
1. Setup a datasource for influx, use `http://influxdb:8086` for the HTTP Url and `telegraf` for the InfluxDB Database name. No auth needed
1. Set `METRICS_HOST=telegraf` environment variable for the service you need
