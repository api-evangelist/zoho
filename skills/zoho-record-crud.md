---
name: zoho-record-crud
description: Create, retrieve, update, and delete a record in a Zoho module.
api: openapi/zoho-records-api-openapi.yml
operations:
- createRecords
- getRecord
- updateRecord
- deleteRecord
generated: '2026-10-04'
method: generated
generator: extract-docs-artifacts.py skills (local)
source: openapi/zoho-records-api-openapi.yml ; every operationId checked against the contract
---

# zoho-record-crud

Create, retrieve, update, and delete a record in a Zoho module.

## Steps

1. 1. Use `createRecords` with the request body containing the record fields.
2. 2. Use `getRecord` with the path parameters `module` and `recordID` to retrieve the created record.
3. 3. Use `updateRecord` with `module`, `recordID` and the request body containing the fields to modify.
4. 4. Use `deleteRecord` with `module` and `recordID` to remove the record.

## Rules

- Auth: Include an OAuth2 bearer token in the `Authorization` header as defined by the `iam-oauth2-schema` scheme.
- Idempotency: `createRecords` and `updateRecord` are not idempotent; repeat calls may create duplicate or additional updates.
