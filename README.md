# Sujaya Mindev

**Full-Stack & Cloud Development | Computer Science (SE) Undergraduate**

[sujaya.dev](https://sujaya.dev) · [LinkedIn](https://www.linkedin.com/in/sujayamindev)

Third-year BSc Computer Science with Software Engineering student at Coventry University, delivered by NIBM. I work across the stack and the infrastructure underneath it — the application, the cloud it runs on, and the pipelines that ship it.

## Featured Projects

### [Reclaima](https://reclaima.sujaya.dev) · [GitHub](https://github.com/sujayamindev/reclaima)

Flutter mobile app (offline-first via Drift/SQLite) on a FastAPI + PostgreSQL backend, behind a KrakenD gateway handling JWT validation and rate limiting. Receipt OCR runs through AWS Textract with a Claude Haiku cleanup layer, feeding per-item warranty and return-window tracking, deadline reminders, and one-tap PDF claim generation. Containerised on an OCI ARM VM with Terraform-managed infrastructure, Prometheus/Loki/Grafana and Sentry monitoring, and a multi-job CI/CD pipeline covering secret scanning, coverage gates, smoke tests, and auto-rollback.

`Flutter` `FastAPI` `PostgreSQL` `KrakenD` `Docker` `Terraform` `OCI` `AWS Textract` `Bedrock` `GitHub Actions`

### [Serverless media upload pipeline](https://media.sujaya.dev) · [GitHub](https://github.com/sujayamindev/serverless-media-upload-pipeline)

Serverless AWS architecture built on a zero-trust model: files upload straight from the browser to S3 via presigned POST, bypassing the API layer for the transfer itself, with a separate Lambda validating binary content on `ObjectCreated` through an approve/reject workflow. Upload status is tracked in DynamoDB behind an auto-polling API, with Cognito for authentication and CloudFront for delivery. Fully defined as Terraform IaC with a GitHub Actions CI pipeline and coverage reporting.

`AWS` `S3` `Lambda` `API Gateway` `DynamoDB` `CloudFront` `Cognito` `React` `Terraform` `GitHub Actions`