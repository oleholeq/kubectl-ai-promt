# Kubectl-AI Prompts Cheat Sheet

This document contains useful prompts for kubectl-ai to help you generate Kubernetes manifests and commands.

## Basic Resources

| NAME | PROMPT | DESCRIPTION | EXAMPLE |
|------|---------|-------------|----------|
| `deployment.yaml` | create an nginx deployment with 2 replicas | Creates a basic deployment with specified replicas | `kubectl-ai "create an nginx deployment with 2 replicas" > deployment.yaml` |
| `deployment-probes.yaml` | create an nginx deployment with liveness and readiness probes | Creates a deployment with health check probes | `kubectl-ai "create an nginx deployment with liveness and readiness probes" > deployment-probes.yaml` |
| `service.yaml` | create a ClusterIP service for nginx deployment | Creates a service to expose the deployment | `kubectl-ai "create a ClusterIP service for nginx deployment" > service.yaml` |
| `configmap.yaml` | create a configmap with environment variables | Creates a ConfigMap with specified environment variables | `kubectl-ai "create a configmap with environment variables" > configmap.yaml` |
| `secret.yaml` | create a secret with database credentials | Creates a Secret with sensitive data | `kubectl-ai "create a secret with database credentials" > secret.yaml` |

## Advanced Resources

| NAME | PROMPT | DESCRIPTION | EXAMPLE |
|------|---------|-------------|----------|
| `hpa.yaml` | create a HorizontalPodAutoscaler for nginx deployment | Creates HPA for automatic scaling | `kubectl-ai "create a HorizontalPodAutoscaler for nginx deployment" > hpa.yaml` |
| `ingress.yaml` | create an ingress resource for nginx service | Creates Ingress for external access | `kubectl-ai "create an ingress resource for nginx service" > ingress.yaml` |
| `pvc.yaml` | create a PersistentVolumeClaim for database storage | Creates PVC for persistent storage | `kubectl-ai "create a PersistentVolumeClaim for database storage" > pvc.yaml` |
| `job.yaml` | create a Kubernetes job to run a batch process | Creates a Job for batch processing | `kubectl-ai "create a Kubernetes job to run a batch process" > job.yaml` |
| `cronjob.yaml` | create a CronJob to run a task every hour | Creates a CronJob for scheduled tasks | `kubectl-ai "create a CronJob to run a task every hour" > cronjob.yaml` |

## Security Resources

| NAME | PROMPT | DESCRIPTION | EXAMPLE |
|------|---------|-------------|----------|
| `rbac.yaml` | create a Role and RoleBinding for a service account | Creates RBAC resources | `kubectl-ai "create a Role and RoleBinding for a service account" > rbac.yaml` |
| `networkpolicy.yaml` | create a NetworkPolicy to restrict pod communication | Creates network policies | `kubectl-ai "create a NetworkPolicy to restrict pod communication" > networkpolicy.yaml` |
| `psp.yaml` | create a PodSecurityPolicy for restricted pods | Creates pod security policies | `kubectl-ai "create a PodSecurityPolicy for restricted pods" > psp.yaml` |

## Troubleshooting Commands

| NAME | PROMPT | DESCRIPTION | EXAMPLE |
|------|---------|-------------|----------|
| `debug-pod.sh` | generate commands to debug a failing pod | Generates debugging commands | `kubectl-ai "generate commands to debug a failing pod" > debug-pod.sh` |
| `logs.sh` | generate commands to get logs from multiple pods | Generates log collection commands | `kubectl-ai "generate commands to get logs from multiple pods" > logs.sh` |
| `describe.sh` | generate commands to describe resources and their events | Generates resource inspection commands | `kubectl-ai "generate commands to describe resources and their events" > describe.sh` |

## Tips
1. Always review the generated manifests before applying them
2. Use specific prompts to get more accurate results
3. Combine prompts for complex scenarios
4. Use the `--explain` flag to understand the generated resources
