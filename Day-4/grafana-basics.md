# Grafana Basics

## What is Grafana?

Grafana is an open-source visualization tool used to display metrics collected from monitoring systems like Prometheus.

## Architecture

Grafana retrieves metrics from Prometheus and displays them as dashboards.

## Data Sources

A data source tells Grafana where monitoring data is stored. In this project, Prometheus is used as the data source.

## Dashboards

A dashboard contains multiple panels that provide an overview of system and Kubernetes metrics.

## Panels

Panels are individual visualizations such as graphs, gauges, and tables.

## Variables

Variables allow dashboards to filter metrics dynamically by namespace, pod, or node.

## Time Range

The time range selector lets users view metrics over different periods such as the last 5 minutes or last 24 hours.

## Transformations

Transformations help modify and organize query results without changing the original PromQL query.