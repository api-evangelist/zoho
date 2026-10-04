---
name: zoho-manage-account
description: Create a new account, retrieve its details, update it, and then list all accounts.
api: openapi/zoho-account-api-openapi.yml
operations:
- createAccount
- getAccount
- updateAccount
- getAccounts
generated: '2026-10-04'
method: generated
generator: extract-docs-artifacts.py skills (local)
source: openapi/zoho-account-api-openapi.yml ; every operationId checked against the contract
---

# zoho-manage-account

Create a new account, retrieve its details, update it, and then list all accounts.

## Steps

1. 1. Use `createAccount` with the request body fields required for creating an account.
2. 2. Use `getAccount` with the path parameter `accountId` returned from the create step.
3. 3. Use `updateAccount` with the same `accountId` and the fields to modify in the request body.
4. 4. Use `getAccounts` to list all accounts, optionally using query parameters for pagination if supported.

## Rules

- Include the OAuth2 access token in the `Authorization` header as `Bearer <token>` (auth scheme: iam-oauth2-schema).
- All write operations (`createAccount`, `updateAccount`) are not idempotent; repeat calls may create duplicate resources.
