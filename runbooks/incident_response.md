# Incident Response Runbook

This runbook provides a simple, repeatable process for handling incidents in cloud environments.

## 1. Triage (First 5–10 minutes)
- Confirm the incident is real (alerts, user reports, monitoring)
- Identify impacted services and severity (SEV1/SEV2/SEV3)
- Check recent changes (deployments, config changes, infrastructure updates)
- Start an incident channel and assign an incident lead

## 2. Diagnose
- Review key metrics (latency, error rate, traffic, saturation)
- Review logs (errors, timeouts, dependency failures)
- Validate upstream/downstream dependencies (identity, DB, network, third-party services)
- Identify if the issue is regional, global, or specific to a component

## 3. Mitigate
- Roll back the latest deployment or configuration change if needed
- Scale up/down services or worker nodes
- Restart unhealthy pods/services
- Disable a feature flag if applicable
- Apply a temporary workaround to restore service

## 4. Communicate
- Share clear updates with stakeholders on a fixed cadence (e.g., every 15–30 minutes)
- Communicate what is impacted, current status, and mitigation steps
- Avoid speculation; confirm before sharing causes

## 5. Resolve and Recover
- Validate service recovery via dashboards and user verification
- Continue monitoring for regression
- Close incident once stability is confirmed

## 6. Post-Incident
- Create a postmortem
- Track action items with owners and due dates
- Update runbooks and alert rules based on learnings
