# 🔍 Kubernetes Security Audit Checklist

## Containers
- Running as root?
- Privileged mode enabled?

## RBAC
- Wildcards (*) used?
- Cluster-admin overly assigned?

## Network
- Default deny policy applied?
- Unrestricted pod communication?

## Risk Indicators

- privileged: true
- runAsUser: 0
- verbs: ["*"]
- resources: ["*"]
