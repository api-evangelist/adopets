---
name: Refund an adoption payment with Adopets
description: Connect a staff user, look up a payment transaction, and issue a full or partial refund via the Adopets External API.
api: openapi/adopets-external-openapi.yml
operations: [connectExternalSystemUser, getPaymentTransaction, refundPaymentTransaction]
---

# Refund an adoption payment transaction (Adopets External API)

Use this skill to refund a completed adoption payment. Refunds move money — confirm intent before executing.

## Auth
Send `x-api-key: <ORG_API_KEY>` on every call. Get a session token first:
1. `POST /organization/external/system-auth/connect` (`connectExternalSystemUser`) → read `data.authorization` and send it as `Authorization: Bearer <token>` on the next steps.

## Refund
2. `POST /organization/external/payment-transaction/get` (`getPaymentTransaction`) with `{ uuid }` to confirm the transaction exists and its amount.
3. `POST /organization/external/payment-transaction/refund` (`refundPaymentTransaction`) with:
   - `uuid` — the transaction uuid
   - `type_key` — refund source, e.g. `SHELTER_FUNDS`
   - `reason` — e.g. `requested_by_customer`
   - `amount` — full or partial amount to refund

## Rules
- All calls are HTTP POST + JSON; success envelope is `prefix: "2xx"`, `message: "OK"`.
- This is a money-moving operation (see `agentic-access/adopets-agentic-access.yml`, consequence `physical`) — require human confirmation for agent-initiated refunds and never retry automatically on ambiguous errors.
