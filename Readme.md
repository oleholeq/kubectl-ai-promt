# Kubectl-AI Prompts Cheat Sheet

This document contains useful prompts for kubectl-ai to help you generate Kubernetes manifests and commands.


Examples:
`kubectl-ai "create an nginx deployment with 2 replicas" > app.yaml`

## Basic Resources

| NAME | PROMPT | DESCRIPTION | EXAMPLE |
|------|---------|-------------|----------|
| app.yaml | create an nginx deployment with 2 replicas | Creates a basic deployment with specified replicas | [app.yaml](yaml/app.yaml) |
| app-livenessProbe.yaml | add liveness probes | Creates  liveness probes | [app-livenessProbe.yaml](yaml/app-livenessProbe.yaml) |
| app-readinessProbe.yaml | add readiness probes | Creates yaml with readiness probes | [app-readinessProbe.yam](yaml/app-readinessProbe.yaml) |
| app-volumeMounts.yaml | configure volume mounts | Configures yaml with volume mounts | [app-volumeMounts.yaml](yaml/app-volumeMounts.yaml) |
| app-cronjob.yaml | create a cronjob | Creates a CronJob for scheduled tasks | [app-cronjob.yaml](yaml/app-cronjob.yaml) |
| app-job.yaml | create a job | Creates a Job for batch processing | [app-job.yaml](yaml/app-job.yaml) |
| app-multicontainer.yaml | set Up Multi-container Pods | Creates yaml with pod that runs more than one container | [app-multicontainer.yaml](yaml/app-multicontainer.yaml) |
| app-resources.yaml | configure Resource Usage | Configure resource requests and limits for your application | [app-resources.yaml](yaml/app-resources.yaml) |
| app-secret-env.yaml | create a secret with database credentials| Creates a Secret with sensitive data | [app-secret-env.yaml](app-secret-env.yaml) |