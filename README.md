This docker compose environment contains the following services:
- Kafka Services
  - Zookeeper
  - Kafka
  - Schema Registry
  - Kafka Rest Proxy
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