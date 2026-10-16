---
name: distyra-feedback-submit-correction-and-confirmation
description: Submit a correction for an enriched transaction and then confirm the transaction was correct.
api: openapi/distyra-openapi.json
operations:
- submitCorrection
- submitConfirmation
generated: '2026-10-16'
method: generated
generator: extract-docs-artifacts.py skills (local)
source: openapi/distyra-openapi.json ; every operationId checked against the contract
---

# distyra-feedback-submit-correction-and-confirmation

Submit a correction for an enriched transaction and then confirm the transaction was correct.

## Steps

1. 1. Call `submitCorrection` with the required request body fields as defined in the contract.
2. 2. Call `submitConfirmation` with the required request body fields as defined in the contract.

## Rules

- Include an `Authorization: Bearer <token>` header for all requests (bearerAuth).
