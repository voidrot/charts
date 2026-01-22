# cloudflared

![Version: 1.0.1](https://img.shields.io/badge/Version-1.0.1-informational?style=flat-square) ![Type: application](https://img.shields.io/badge/Type-application-informational?style=flat-square) ![AppVersion: 2026.1.1](https://img.shields.io/badge/AppVersion-2026.1.1-informational?style=flat-square)

Helm chart to deploy Cloudflare Tunnel (cloudflared) as a Kubernetes Deployment

**Homepage:** <https://github.com/cloudflare/cloudflared>

## Maintainers

| Name | Email | Url |
| ---- | ------ | --- |
| voidrot |  |  |

## Source Code

* <https://github.com/cloudflare/cloudflared>
* <https://github.com/cloudflare/helm-charts/tree/main/charts/cloudflare-tunnel-remote>

## Values

| Key | Type | Default | Description |
|-----|------|---------|-------------|
| affinity | object | `{}` |  |
| autoscaling.enabled | bool | `false` |  |
| autoscaling.maxReplicas | int | `100` |  |
| autoscaling.minReplicas | int | `1` |  |
| autoscaling.targetCPUUtilizationPercentage | int | `80` |  |
| extra_commands | list | `[]` |  |
| extra_labels | object | `{}` |  |
| fullnameOverride | string | `""` |  |
| image.pullPolicy | string | `"IfNotPresent"` |  |
| image.repository | string | `"cloudflare/cloudflared"` |  |
| image.tag | string | `""` |  |
| imagePullSecrets | list | `[]` |  |
| livenessProbe.httpGet.path | string | `"/ready"` |  |
| livenessProbe.httpGet.port | string | `"metrics"` |  |
| nameOverride | string | `""` |  |
| nodeSelector | object | `{}` |  |
| podAnnotations | object | `{}` |  |
| podLabels | object | `{}` |  |
| podSecurityContext | object | `{}` |  |
| readinessProbe.httpGet.path | string | `"/ready"` |  |
| readinessProbe.httpGet.port | string | `"metrics"` |  |
| replicaCount | int | `1` |  |
| resources | object | `{}` |  |
| securityContext.allowPrivilegeEscalation | bool | `false` |  |
| securityContext.capabilities.drop[0] | string | `"ALL"` |  |
| securityContext.readOnlyRootFilesystem | bool | `true` |  |
| securityContext.runAsNonRoot | bool | `true` |  |
| securityContext.runAsUser | int | `65532` |  |
| service.port | int | `2000` |  |
| service.type | string | `"ClusterIP"` |  |
| serviceAccount.annotations | object | `{}` |  |
| serviceAccount.automount | bool | `true` |  |
| serviceAccount.create | bool | `true` |  |
| serviceAccount.name | string | `""` |  |
| tolerations | list | `[]` |  |
| tunnel.createSecret | bool | `false` |  |
| tunnel.credentials | string | `""` |  |
| tunnel.enabled | bool | `true` |  |
| tunnel.mountPath | string | `"/etc/cloudflared"` |  |
| tunnel.secretKey | string | `"token"` |  |
| tunnel.secretName | string | `""` |  |
| volumeMounts | list | `[]` |  |
| volumes | list | `[]` |  |

