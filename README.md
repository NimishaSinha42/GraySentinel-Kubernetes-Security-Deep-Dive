# GraySentinel Kubernetes Security Deep-Dive

A hands-on Kubernetes security assessment project focused on identifying cluster misconfigurations, container image vulnerabilities, insecure access controls, and software supply-chain risks using industry-standard security tools.

## Overview

This project demonstrates a complete Kubernetes security audit workflow using multiple open-source tools:

- kube-hunter
- kube-bench
- Trivy
- Syft
- Grype

The audit covers Kubernetes cluster security, CIS benchmark checks, container image vulnerability scanning, SBOM generation, vulnerability correlation, automated reporting, and remediation documentation.

## Objectives

The main objectives of this lab were to:

- Identify exposed Kubernetes services and risky configurations
- Assess Kubernetes security posture using CIS Benchmarks
- Scan container images for known CVEs
- Generate a Software Bill of Materials (SBOM)
- Analyze SBOM components for vulnerabilities
- Automate multiple security scans using Bash
- Consolidate findings into a structured HTML security report
- Document remediation steps for identified misconfigurations

## Tools Used

| Tool | Purpose |
|---|---|
| kube-hunter | Kubernetes penetration testing and attack-surface discovery |
| kube-bench | CIS Kubernetes Benchmark compliance assessment |
| Trivy | Container image and vulnerability scanning |
| Syft | SBOM generation |
| Grype | Vulnerability scanning using SBOM data |
| Bash | Security audit automation |
| Python | Consolidated report generation |

## Lab Workflow

The complete workflow followed in this project:

```text
Kubernetes Environment
        |
        v
kube-hunter
        |
        +--> Exposed services / security weaknesses
        |
        v
kube-bench
        |
        +--> CIS Benchmark configuration findings
        |
        v
Trivy
        |
        +--> Container image CVEs
        |
        v
Syft
        |
        +--> SBOM
        |
        v
Grype
        |
        +--> Vulnerabilities in packages/components
        |
        v
Bash Automation
        |
        v
Python Report Generator
        |
        v
Consolidated HTML Security Report
