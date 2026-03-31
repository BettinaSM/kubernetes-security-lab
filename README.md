# 🔐 Kubernetes Security Lab

A hands-on project demonstrating Kubernetes security best practices, common misconfigurations, and real-world attack scenarios.

---

##  Overview

This project simulates real-world Kubernetes security risks and demonstrates how to secure workloads using:

* Pod Security Contexts
* RBAC (Role-Based Access Control)
* Network Policies
* Secure configuration patterns

---

##  Objectives

* Identify insecure Kubernetes configurations
* Apply security best practices
* Simulate real attack scenarios
* Demonstrate container and cluster hardening

---

##  Technologies

* Kubernetes (YAML manifests)
* RBAC
* Network Policies

---

##  Real-World Security Simulation

This project simulates real-world Kubernetes security risks commonly found in production environments, including:

- Privileged containers
- RBAC misconfigurations
- Open network communication
- Container breakout scenarios

Designed to reflect enterprise-grade Kubernetes security challenges.

---

##  Project Structure

```text
.
├── manifests/
│   ├── insecure-pod.yaml
│   ├── secure-pod.yaml
├── rbac/
│   ├── insecure-role.yaml
│   ├── secure-role.yaml
├── network/
│   ├── insecure-networkpolicy.yaml
│   ├── secure-networkpolicy.yaml
├── scenarios/
│   ├── container-breakout.md
└── README.md
```

---

##  Key Security Risks Demonstrated

###  Privileged Containers

Containers running with elevated privileges can:

* Access host resources
* Escape container isolation
* Compromise the node

---

###  Overly Permissive RBAC

```yaml
verbs: ["*"]
resources: ["*"]
```

Grants full control over the cluster.

---

###  Open Network Policies

Allow unrestricted communication between pods, increasing lateral movement risk.

---

##  Security Best Practices

* Run containers as non-root
* Disable privilege escalation
* Apply least privilege RBAC
* Restrict network traffic
* Use read-only filesystems

---

##  Attack Scenario: Container Breakout

This project includes a real-world scenario where:

* A privileged container is compromised
* The attacker escapes to the host
* Full control over the node is achieved

---

##  Hardening Techniques

* Pod Security Standards (baseline/restricted)
* RBAC minimization
* Network segmentation
* Secure defaults

---

##  Future Improvements

* Integration with security tools (Falco, Kyverno, OPA)
* Runtime threat detection
* Kubernetes audit logging
* CI/CD security scanning

---

##  Topics

kubernetes, security, devsecops, rbac, containers, cloud-security, k8s, network-policy

---

##  Author

Bettina Santana de Meirelles
Unix/Linux Infrastructure | DevOps | Security | Cloud

🔗 https://github.com/BettinaSM

---

##  Key Takeaways

✔ Kubernetes security in practice
✔ Real misconfiguration scenarios
✔ Attack simulation mindset
✔ Secure workload design

---

##  Conclusion

This project demonstrates how insecure Kubernetes configurations can lead to critical security risks and how applying security best practices can significantly improve cluster protection.
