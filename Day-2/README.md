# 📅 Day 2: Monitor Docker Containers Using Prometheus & cAdvisor

## 🎯 Objective

The objective of Day 2 is to monitor Docker containers using Prometheus and cAdvisor. In this project, Prometheus is configured to scrape metrics exposed by cAdvisor, allowing us to monitor CPU, memory, filesystem, and network usage of running Docker containers. This setup follows the official Prometheus cAdvisor monitoring guide. :contentReference[oaicite:0]{index=0}

---

## 📚 Topics Covered

- Prometheus Configuration
- cAdvisor
- Docker Monitoring
- Scrape Targets
- PromQL
- Counter Metrics
- Gauge Metrics

---

## 🏗️ Architecture

                    +----------------------+
                    |   Docker Desktop     |
                    |                      |
                    | Docker Containers    |
                    +----------+-----------+
                               |
                               |
                        Container Metrics
                               |
                        +------v------+
                        |   cAdvisor  |
                        |   Port 8080 |
                        +------+------+
                               |
                        Prometheus Pull
                               |
                        +------v------+
                        | Prometheus  |
                        |   Port 9090 |
                        +------+------+
                               |
                        Prometheus UI

---

## 🛠 Steps Performed

1. Started the cAdvisor container.
2. Configured Prometheus to scrape cAdvisor metrics.
3. Restarted Prometheus.
4. Verified Prometheus targets.
5. Executed PromQL queries.
6. Explored CPU, Memory and Network metrics.

---

## 📊 PromQL Queries

### Check Target Status

```promql
up
```

### CPU Usage

```promql
container_cpu_usage_seconds_total
```

### Memory Usage

```promql
container_memory_usage_bytes
```

### Network Receive

```promql
container_network_receive_bytes_total
```

### Network Transmit

```promql
container_network_transmit_bytes_total
```

---

## 📖 Learning Outcome

After completing Day 2, I learned:

- How Prometheus scrapes metrics.
- What cAdvisor is.
- How Docker container monitoring works.
- Difference between Counter and Gauge metrics.
- How to explore metrics using PromQL.

---

## 📸 Screenshots

- Prometheus Targets
- cAdvisor UI
- CPU Metrics
- Memory Metrics
- Network Metrics
