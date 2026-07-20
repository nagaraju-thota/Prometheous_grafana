# Commands Used

## Start Containers

```bash
docker compose up -d
```

## Verify Containers

```bash
docker ps
```

## Restart Prometheus

```bash
docker restart prometheus
```

## Verify Targets

Open

http://localhost:9090/targets

## Open cAdvisor

http://localhost:8080

## Execute PromQL

```promql
up
```

```promql
container_cpu_usage_seconds_total
```

```promql
container_memory_usage_bytes
```

```promql
container_network_receive_bytes_total
```

```promql
container_network_transmit_bytes_total
```
