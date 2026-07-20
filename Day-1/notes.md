# Monitoring Fundamentals

## What is Monitoring?

Monitoring is the continuous process of collecting metrics from systems and applications to understand their health and performance.

---

## Monitoring vs Logging vs Tracing

| Monitoring | Logging | Tracing |
|------------|----------|----------|
| Metrics | Text Events | Request Flow |
| System Health | Application Events | End-to-End Request Tracking |

---

## Metrics

Metrics are numerical values collected over time.

Examples:

- CPU Usage
- Memory Usage
- Disk Usage
- HTTP Requests
- Active Users

---

## Time Series Database (TSDB)

A Time Series Database stores data with timestamps.

Example:

10:00 -> CPU = 30%

10:01 -> CPU = 40%

10:02 -> CPU = 65%

---

## What is Prometheus?

Prometheus is an open-source monitoring system that collects, stores, queries, and alerts on metrics.

---

## Prometheus Components

Prometheus Server – The core component that collects metrics from targets, stores them in a Time Series Database (TSDB), and evaluates queries and alert rules.
Exporters – Lightweight agents that expose metrics from applications or systems in a Prometheus-compatible format for scraping.
Alertmanager – Receives alerts from Prometheus, groups and filters them, then sends notifications through channels like Email, Slack, or Microsoft Teams.
Pushgateway – An intermediary that allows short-lived jobs (such as cron jobs or batch jobs) to push metrics, which Prometheus later scrapes.

---

## Pull vs Push

Pull:
Prometheus scrapes metrics from targets.

Push:
Applications push metrics to Pushgateway.

---

## Metric Types

### Counter

Only increases.

Example:
- Total Requests

### Gauge

Can increase or decrease.

Example:
- CPU Usage

### Histogram

Measures request duration in buckets.

### Summary

Calculates latency quantiles.