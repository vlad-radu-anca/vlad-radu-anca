# Vlad-Radu Anca

Senior DevOps Engineer based in Cluj-Napoca, Romania, working remotely across the EU. 11 years in IT infrastructure, the last 5 focused on AWS and Kubernetes for regulated enterprises in healthcare, banking and telecommunications.

AWS Certified DevOps Engineer - Professional · AWS Certified Security - Specialty · CKA · CKAD

Open to senior DevOps engagements, B2B contract or permanent. [LinkedIn](https://www.linkedin.com/in/vlad-radu-a-8366ab180)

## Portfolio

Each repository is built to run, not just to read: CI validates it on every change, and the README explains the design decisions and the tradeoffs behind them.

| Repository | What it shows |
| --- | --- |
| [agentcore-order-agent](https://github.com/vlad-radu-anca/agentcore-order-agent) | A customer support agent on Amazon Bedrock AgentCore. Python tools served over MCP by an AgentCore Gateway, a Bedrock Knowledge Base on S3 Vectors, Guardrails and least-privilege IAM, all in Terraform. Deployed to AWS and shown working in a [recorded transcript](https://github.com/vlad-radu-anca/agentcore-order-agent/blob/main/docs/demo/transcript-2026-10-05.md). |
| [aws-landing-zone](https://github.com/vlad-radu-anca/aws-landing-zone) | Multi-account AWS built from Organizations primitives: an OU tree, service control policies composed to fit the 5,120 character limit, IAM Identity Center permission sets and delegated security administration. Designed to deploy from GitHub Actions through OIDC, with no long-lived keys. |
| [gitops-platform](https://github.com/vlad-radu-anca/gitops-platform) | A Kubernetes platform delivered entirely by Argo CD: app-of-apps with sync waves, Envoy Gateway on the Gateway API, External Secrets, kube-prometheus-stack, and promotion across environments with an ApplicationSet. CI brings the whole platform up on kind and smoke tests it. |
| [sre-reliability-lab](https://github.com/vlad-radu-anca/sre-reliability-lab) | SLOs, alerting and game days on top of gitops-platform. SLOs as code generated into multi-window burn-rate alerts, unit tested with promtool, with a runbook per alert. On every change, CI deploys the whole platform, injects faults with Chaos Mesh and checks that the right alert pages and the wrong ones stay silent. The game days caught a latency SLO that could never fire. |
| [helm-umbrella-platform](https://github.com/vlad-radu-anca/helm-umbrella-platform) | 29 Helm charts for a multi-service platform, 20 of them composed into one umbrella chart. Unit tested with helm-unittest, validated with kubeconform, and published to GHCR as OCI artifacts by CI. |
| [terraform-templates](https://github.com/vlad-radu-anca/terraform-templates) | 23 reusable Terraform modules for AWS, including VPC, EKS, RDS and Aurora, ECS, ALB, CloudFront, WAF and Cognito. Terraform 1.5+ and AWS provider 6, released as v1.0.0. |

## Toolbox

- **Cloud:** AWS (EKS, ECS Fargate, Lambda, Organizations, IAM, VPC, RDS, DynamoDB), Amazon Bedrock and AgentCore
- **Infrastructure as code:** Terraform, CloudFormation, Ansible
- **Kubernetes:** EKS, Kubespray, Helm, Argo CD, FluxCD
- **CI/CD:** GitHub Actions, Jenkins
- **Observability and SRE:** Prometheus, Alertmanager, Grafana, SLOs and error budgets (Sloth), Chaos Mesh, k6
- **Security:** Trivy, Checkov, tflint, Snyk, SonarCloud, KubeScape, GuardDuty, Security Hub
- **Languages:** Python, Bash
