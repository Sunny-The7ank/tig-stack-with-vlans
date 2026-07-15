# tig-stack-with-vlans
My TIG (Telegraf, InfluxDB, Grafana) stack with VLAN support

## What is this?
A TIG stack that took me way too much trial, error, and research with containerized components in different VLANs.
## Why?
¯\_(ツ)_/¯

For fun mostly. I wanted my telegraf agent to influxdb3 traffic to happen over a tagged VLAN that doesn't have internet access.

## Features
* Influxdb3 enterprise using the home license, no 3 day limitation
* Influxdb3 to grafana traffic occurs only over the internal private docker network
* Grafana is exposed on the host's native VLAN
