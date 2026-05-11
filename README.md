# cpfull-1778507898

Full E2E demo: GitHub repo → AWS CodePipeline → CodeBuild → ArgoCD → K8s pod

Generated from the Backstage `java-service` scaffolder template.

- **Group:** `devex/scaffolder`
- **Markets:** `usa`
- **Owner:** `user:guest`

## Local development

```bash
mvn spring-boot:run
curl http://localhost:8080/
```

## CI/CD

- `.github/workflows/ci.yml` — build + test on every push and PR.
- `.github/workflows/cd.yml` — deploy across the configured markets (usa) on push to `main`.

## Backstage views

This service is registered in Backstage and surfaces:

- Pipeline Triage
- DORA Metrics
- Failure Intelligence
- Market Deployments

at both the unit (service) and group (`devex/scaffolder`) level.
