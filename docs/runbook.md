---
category: runbook
title: Wallet Service runbook
description: On-call runbook for Wallet Service.
related_entities:
  - wallet-service
---

# Wallet Service runbook

On-call guide for `wallet-service` (Payments, tier critical).

## Alerts

- **wallet-service-high-error-rate** — 5xx over 2% for 5m. Check upstream dependencies.
- **wallet-service-latency** — p99 over SLO. Check resource saturation.

## Common issues

- **Pod OOMKilled** — check memory limits and recent traffic spikes.
- **Crashloop** — check the last deploy and roll back if needed.

## Escalation

No owning team. Escalate to Platform on-call.

