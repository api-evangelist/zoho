---
name: zoho-write-bulk-job
description: Create a bulk write job and then retrieve its details.
api: openapi/zoho-write-api-openapi.yml
operations:
- createBulkWriteJob
- getJobDetails
generated: '2026-10-04'
method: generated
generator: extract-docs-artifacts.py skills (local)
source: openapi/zoho-write-api-openapi.yml ; every operationId checked against the contract
---

# zoho-write-bulk-job

Create a bulk write job and then retrieve its details.

## Steps

1. 1. `createBulkWriteJob` – no request fields or headers are documented.
2. 2. `getJobDetails` – requires the path parameter `jobId`.

## Rules

- Authenticate using the iam‑oauth2‑schema OAuth2 bearer token in the Authorization header.
- No rate‑limit or pagination details are provided.
