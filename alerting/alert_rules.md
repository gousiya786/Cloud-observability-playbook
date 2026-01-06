# Alerting Rules (Starter)

These are general alerting guidelines for cloud services (Azure Monitor / Grafana style).

## Golden Signals
1) Latency
- Alert when P95 latency exceeds target for sustained period (e.g., 5–10 minutes)

2) Traffic
- Alert on unexpected drops/spikes in request rate

3) Errors
- Alert on error rate exceeding threshold (e.g., 5xx > 2% for 5 minutes)

4) Saturation
- CPU/memory/disk usage sustained high (e.g., CPU > 85% for 10 minutes)

## Recommended Alerts (Examples)
- API 5xx error rate > 2% for 5 minutes
- P95 latency > 1s for 10 minutes
- Pod restart count spike (possible crash loops)
- Node CPU > 85% for 10 minutes
- Disk usage > 80% sustained

## Alert Hygiene
- Avoid noisy alerts (tune thresholds and duration)
- Every alert should include: severity, impact, owner, runbook link
- Review alert effectiveness after incidents
