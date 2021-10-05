# Metrics Stack

This stack can be used to standup a close approximation to the SS Metrics stack if its ever needed for dev/debugging

It will spin up InfluxDB, Telegraf, and Grafana.

## Setup
1. Run `docker-compose up -d `
1. Set-up grafana by browsing to  `http://localhost:3000` and use `admin` for both user and password.
1. Setup a datasoyurce for influx, use `http://influxdb:8086` for the HTTP Url and `telegraf` for the InfluxDB Database name. No auth needed
1. Set `METRICS_HOST=telegraf` environment variable for Dreadnought
