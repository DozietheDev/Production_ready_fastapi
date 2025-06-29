```markdown
# Runbook: FastAPI Service

## Common Commands
- Deploy: `scripts/deploy.sh`
- Health Check: `scripts/health-check.sh`
- Rollback: `scripts/rollback.sh`

## Incident Response
- Use `kubectl logs` to check logs
- Use `kubectl describe` for resource issues
- Use `kubectl rollout restart deployment fastapi-service` to restart

## Scaling
- HPA automatically scales based on CPU
- Manual scale: `kubectl scale deployment fastapi-service --replicas=5`

## Monitoring
- Check Prometheus for live metrics
- Use Grafana dashboard for visualizations

## Secrets
- Store sensitive values in Kubernetes Secrets
- Use external managers like AWS Secrets Manager if required
```
