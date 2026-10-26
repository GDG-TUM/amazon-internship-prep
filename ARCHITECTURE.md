# CloudPulse Architecture

## Goal
Accept synthetic application events, store structured records, archive raw events, calculate aggregates, and expose health information.

```text
Client / test generator
        | HTTP
        v
API / reverse proxy (later milestone)
        +----> PostgreSQL: structured event records
        +----> JSONL archive -> local storage / later S3
        v
Batch processor -> aggregated operational metrics
        v
Health checks, logs, demo and incident evidence
```

## Stages
1. Linux/network experiments.
2. Local API + PostgreSQL using Docker Compose.
3. Synthetic event generator and batch processor.
4. Backup/restore, health checks and incidents.
5. Cloud mapping and optional AWS deployment.

## Boundaries
- Secrets belong in ignored local environment files or a secret manager.
- Do not expose PostgreSQL publicly.
- Use synthetic data only.
- Use persistent volumes and test restore.
- Health checks must not reveal credentials.
- Avoid Kubernetes, message brokers and complex frontend work until the core is complete.

## Planned cloud mapping
| Local component | Possible AWS mapping | Learning objective |
|---|---|---|
| Linux app/container | EC2 or managed compute | Compute and operations |
| Local network | VPC, subnets, route tables | CIDR and routing |
| PostgreSQL | Managed or self-managed PostgreSQL | Database operations |
| JSONL archive | S3 | Object storage/lifecycle |
| Logs and metrics | CloudWatch | Observability |
| Credentials/permissions | IAM role and policy | Least privilege |

This is a design plan, not evidence that AWS resources have been created.