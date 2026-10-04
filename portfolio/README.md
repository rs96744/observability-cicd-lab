# Observability CI/CD Lab

## Purpose

This project demonstrates an industrial CI/CD approach for a cloud-native, OpenTelemetry-instrumented microservices application.

It extends the official OpenTelemetry Demo in an isolated personal lab. The implementation uses synthetic application traffic and does not connect to corporate monitoring systems or use production data.

## Objectives

The project will demonstrate:

* Git feature-branch and pull-request workflows
* Automated code-quality and test validation
* Container image building and versioning
* Security and dependency scanning
* Immutable artifact promotion
* Development and Production environments
* Manual Production approval
* Post-deployment smoke and health tests
* Metrics, logs, and distributed traces
* Deployment monitoring and rollback
* Prometheus and Grafana integration
* Optional Dynatrace OpenTelemetry integration
* GitHub Actions and Azure DevOps pipelines

## Planned Delivery Flow

1. Create a short-lived feature branch.
2. Implement and test a controlled change.
3. Open a pull request.
4. Run automated quality, test, and security checks.
5. Build a versioned container image.
6. Deploy the verified artifact to Development.
7. Run smoke and telemetry validation tests.
8. Require approval before Production.
9. Promote the same immutable artifact to Production.
10. Validate application health and roll back if necessary.

## Security Boundaries

This project must not contain:

* Corporate monitoring data
* Employer or customer information
* Internal hostnames, IP addresses, or URLs
* Production logs or telemetry
* Passwords, API keys, access tokens, or certificates
* Private container-registry credentials
* Cloud service credentials

Only synthetic telemetry and publicly available demo data may be used.

Secrets required by personal lab integrations must be stored in approved secret-management mechanisms and injected at runtime. They must never be committed to Git.

## Attribution

This repository is derived from the open-source OpenTelemetry Demo. Original project ownership and licensing remain with the OpenTelemetry contributors.

Portfolio-specific pipeline, security, deployment, and observability changes are maintained separately in this fork.

## Current Status

The project is under active development as a personal hands-on implementation. It must not be represented as an employer production deployment.
