# Prometheus - Grafana - docker-compose

This is a basic example on how to configure Prometheues / Grafana with docker compose.
Rules for prometheus are empty, you have to configure them yourself and recreate the images.
Using [Promscale](https://github.com/timescale/promscale) which is deprecated, but is good to have a place where to store your metrics!

Simply run
```
docker compose -f docker-compose.yml up -d
```

Wait a couple of seconds because there are some things that need to be set on timescaledb

Run again
```
docker compose -f docker-compose.yml up -d
```
Now all the containers should be running.

You can access prometheus at

http://localhost:9090

Grafana at

http://localhost:3000

admin / admin

- Password must be changed but you can set again admin.
Prometheus Data Source will be visible at 

http://localhost:3000/datasources

Click on Prometheus

Scroll to the bottom, and Test

