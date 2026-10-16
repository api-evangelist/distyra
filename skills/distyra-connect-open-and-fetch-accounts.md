---
name: distyra-connect-open-and-fetch-accounts
description: Open a bank connection for a user and retrieve the accounts linked to that connection.
api: openapi/distyra-openapi.json
operations:
- createConnection
- getConnection
- getConnectionAccounts
generated: '2026-10-16'
method: generated
generator: extract-docs-artifacts.py skills (local)
source: openapi/distyra-openapi.json ; every operationId checked against the contract
---

# distyra-connect-open-and-fetch-accounts

Open a bank connection for a user and retrieve the accounts linked to that connection.

## Steps

1. 1. Call `createConnection` with the required request body (e.g., bank ID, redirect URLs) and include the `Authorization: Bearer <token>` header.
2. 2. Call `getConnection` with the connection `id` returned from step 1, using the `Authorization` header.
3. 3. Call `getConnectionAccounts` with the same connection `id` to list the accounts, also sending the `Authorization` header.

## Rules

- All requests must include an `Authorization: Bearer <access-token>` header (bearerAuth).
- Use the base URL `https://api.distyra.com` for all calls.
