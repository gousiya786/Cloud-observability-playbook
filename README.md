# Cloud Observability Playbook

This repository provides practical templates and examples for cloud observability,
including monitoring, alerting, incident response, and postmortems. The content is
Azure Monitor and Grafana friendly and reflects real-world production operations.

---

## What This Project Demonstrates

- Monitoring and observability fundamentals (golden signals)
- Alert design and alert hygiene
- Incident response processes and runbooks
- Postmortem structure and continuous improvement

---

## Contents

- runbooks/incident_response.md  
  Step-by-step incident response workflow (triage → diagnosis → mitigation → communication → recovery)

- runbooks/postmortem_template.md  
  A structured template for documenting incidents and tracking preventative actions

- alerting/alert_rules.md  
  Starter alerting rules using golden signals (latency, traffic, errors, saturation)

- dashboards/grafana_dashboard_sample.json  
  Example dashboard export format (safe public sample)

---

## Repository Structure

cloud-observability-playbook/
- runbooks/
  - incident_response.md
  - postmortem_template.md
- alerting/
  - alert_rules.md
- dashboards/
  - grafana_dashboard_sample.json
- README.md

---

## Why This Repository Matters

Observability is critical for reliable cloud services. This repository shows a production mindset:
clear runbooks, actionable alerts, and structured postmortems that drive continuous improvement.

---

Author  
Fathima Gousiya  
DevOps / Systems Engineer  
LinkedIn: https://linkedin.com/in/Fathima-gousiya
