# 🚨 Container Breakout Scenario

## Context

A Kubernetes pod is running with privileged access:

- privileged: true
- running as root

## Risk

This allows:

- Access to host resources
- Kernel-level interaction
- Potential node takeover

## Attack Path

1. Attacker gains access to container
2. Uses privileged mode to escape container
3. Gains access to host system

## Impact

- Full cluster compromise
- Data exfiltration
- Persistence

## Mitigation

- Disable privileged containers
- Enforce non-root execution
- Apply Pod Security Standards
