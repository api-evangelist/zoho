---
name: zoho-mark-invoices-sent
description: Mark a batch of invoices as sent and update their status.
api: openapi/zoho-finance-api-openapi.yml
operations:
- getInvoices
- markInvoicesAsSent
- updateInvoiceStatus
generated: '2026-10-04'
method: generated
generator: extract-docs-artifacts.py skills (local)
source: openapi/zoho-finance-api-openapi.yml ; every operationId checked against the contract
---

# zoho-mark-invoices-sent

Mark a batch of invoices as sent and update their status.

## Steps

1. 1. Retrieve the invoices to be processed using the `getInvoices` operation (path parameter `financeService`).
2. 2. Mark all retrieved invoices as sent with the `markInvoicesAsSent` operation (request body may contain invoice IDs).
3. 3. Update the status of each invoice using the `updateInvoiceStatus` operation (path parameters `financeService` and `id`, request body with the new status).

## Rules

- Auth: Include an OAuth2 bearer token in the `Authorization` header as required by the `iam-oauth2-schema` scheme.
- Idempotency: The `markInvoicesAsSent` POST operation should be called once per batch to avoid duplicate sent markings.
