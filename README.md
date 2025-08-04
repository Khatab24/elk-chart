# ELK Stack Helm Deployment

This repo contains Helm chart configurations to deploy the ELK Stack (Elasticsearch, Logstash, Kibana, and Filebeat) on a Kubernetes cluster using Helm.

## 📦 Components

- **Elasticsearch**: Central log storage and search engine
- **Kibana**: UI for visualizing logs
- **Logstash**: Log processing pipeline
- **Filebeat**: Lightweight shipper to send logs to Logstash

---

## 🚀 Installation Command Example

We used Helm with specific value files and version pinning:

```bash
helm upgrade filebeat elastic/filebeat \
  -n elk \
  -f filebeat-values.yaml \
  --version 7.17.3
