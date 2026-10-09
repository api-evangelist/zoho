---
name: zoho-read-bulk-job
description: Create a bulk read job, poll for its completion, and download the resulting data.
api: openapi/zoho-read-api-openapi.yml
operations:
- createBulkReadJob
- getBulkReadJobDetails
- downloadResult
generated: '2026-10-04'
method: generated
generator: extract-docs-artifacts.py skills (local)
source: openapi/zoho-read-api-openapi.yml ; every operationId checked against the contract
---

# zoho-read-bulk-job

Create a bulk read job, poll for its completion, and download the resulting data.

## Steps

1. 1. `createBulkReadJob` – no specific request fields or headers are documented.
2. 2. `getBulkReadJobDetails` – no specific request fields or headers are documented.
3. 3. `downloadResult` – no specific request fields or headers are documented.

## Rules

- Include an OAuth2 Bearer token in the `Authorization` header as defined by the iam-oauth2-schema.
