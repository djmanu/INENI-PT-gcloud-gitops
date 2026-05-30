# Group H GitOps Repository Scope

## Purpose
This directory contains the Day 2 GitOps scope for the Group H platform.

Managed resources:
- Argo CD applications for platform services
- platform configuration such as DNS and secret stores
- Crossplane providers and tenant API
- tenant manifests
- staging and production release manifests for tenant image promotion

## Promotion Flow
1. update `tenants/release-staging.yaml`
2. validate the staging tenant
3. promote the same image references into `tenants/release-production.yaml`

## Publication Target
The assignment requires IaC and GitOps code in separate public repositories.

This directory is prepared so it can be published as the dedicated GitOps repository with minimal restructuring.
