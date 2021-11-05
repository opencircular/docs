---
layout: page
title: Monitoring
permalink: /monitoring
nav_order: 8
has_children: false
---

Monitoring
====================

- Grafana Dashboard https://plasticoinapp.grafana.net/


https://grafana.com/go/webinar/guide-grafana-cloud-exploring-kubernetes-metrics-and-logs/ 


1. Kubernetes Integration install via https://plasticoinapp.grafana.net/a/grafana-easystart-app/?page=integrations-management 
2. Configure 
3. Restart
```
kubectl rollout restart deployment/grafana-agent
```
4. Configure Kubernetes Workload Logging (Loki Agent)
https://grafana.com/docs/grafana-cloud/quickstart/agent-k8s/k8s_agent_logs/
5. Explore logs and metrics
```
https://plasticoinapp.grafana.net/goto/9ftOSQK7k?orgId=1 
```
6. Loki Query to search the plasticoin node app for a log that contains the word "gateway"
```
{app="node"} |= "gateway"
```
7. Setup alert rules
https://www.youtube.com/watch?v=GdgX46KwKqo 
```
count_over_time(({app="node"} |= "Gateway ready")[60s])
```
