# PromQL Queries

## CPU Usage

```promql
sum(rate(container_cpu_usage_seconds_total[5m]))
```

## Memory Usage

```promql
sum(container_memory_working_set_bytes)
```

## Running Pods

```promql
count(kube_pod_info)
```

## Running Deployments

```promql
count(kube_deployment_status_replicas_available)
```

## Running Nodes

```promql
count(kube_node_info)
```

These queries help visualize Kubernetes resource utilization and cluster status in Grafana.