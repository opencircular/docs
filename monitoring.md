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

1. Kubernetes Integration install via https://plasticoinapp.grafana.net/a/grafana-easystart-app/?page=integrations-management 
2. Configure 
3. Restart
```
kubectl rollout restart deployment/grafana-agent
```