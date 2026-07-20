# Hands-on

## Pull Prometheus Image

```bash
docker pull prom/prometheus
```

---

## Run Prometheus

```bash
docker run -d \
  --name prometheus \
  -p 9090:9090 \
  prom/prometheus
```

PowerShell

```powershell
docker run -d --name prometheus -p 9090:9090 prom/prometheus
```

---

## Verify

```bash
docker ps
```

---

## Open UI

http://localhost:9090

---

## Check Targets

Status

↓

Targets

---

## Query Metrics

```
up
```

```
prometheus_build_info
```

```
prometheus_tsdb_head_series
```

```
prometheus_engine_queries
```
