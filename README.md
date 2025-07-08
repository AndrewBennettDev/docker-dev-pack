# Docker Dev Pack

## Description
The Docker Dev pack is something I used in my first job. We often needed services running locally to test changes,
so this was an easy way to spin up most of the things you needed. I am regularly adding services that I find
helpful, but if you see this and use it please feel free to recommend other services!

## NOTE:
If this line is still here, there are issues. Use are your own discretion...

This docker compose environment contains the following services:
- Data/Messaging Services
  - Kafka
  - Schema Registry
  - Kafka Rest Proxy
  - Spark
- Persistence
  - MySql
  - BigTable
  - Redis
  - Elasticsearch
- Metrics & Monitoring
  - Prometheus
  - Grafana

## Container Specific Notes
#### MySql
- Mounts `/Users/Shared/dkr-mysql` as a persistent volume
  - Empty this directory to clear all data

## Troubleshooting
Some of these containers use a lot of memory. Be sure to allocate your Docker env enough memory to handle your workload.

Increase in the docker dashboard:
settings cog (top right) --> Resources --> CPU/Memory/Disk
