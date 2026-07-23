---
name: Collect an adoption payment with Adopets
description: Connect an external staff user, create an adoption payment request with line items, and confirm it — using the Adopets External API.
api: openapi/adopets-external-openapi.yml
operations: [connectExternalSystemUser, createPaymentRequest, getPaymentRequest]
---

# Collect an adoption payment (Adopets External API)

Use this skill to charge an adopter for an adoption through Adopets.

## Auth (do this first)
Every request needs the organization key header `x-api-key: <ORG_API_KEY>`. Payment-request read/change operations also need a session bearer token.

1. **Connect** — `POST /organization/external/system-auth/connect` (`connectExternalSystemUser`) with `{ email, first_name, last_name, role }`. `role` is one of `staff, super_user, editor, owner, foster_admin, admin`. Read `data.authorization` from the response — that JWT is your `Authorization: Bearer <token>` for later steps.

## Create the payment request
2. `POST /organization/external/payment-request/create` (`createPaymentRequest`) with:
   - `adopter_email`, `adopter_first_name`, `adopter_last_name`
   - `type_key: EXTERNAL_ADOPTION`
   - `items[]` — each with `name`, `type_key` (`ADOPTION_FEE` | `LICENSE` | `PRODUCT`), `base_amount`, `charge_amount`, `is_required`.
   Read `data.uuid` from the response.

## Confirm
3. `POST /organization/external/payment-request/get` (`getPaymentRequest`) with `{ uuid }` (send the bearer token). Check `data.status_key`.

## Rules
- All calls are HTTP POST with a JSON body; success is `message: "OK"`, `prefix: "2xx"`.
- Errors come back in the same envelope with a `4xx`/`5xx` prefix and a `message` — do not retry blindly (no client idempotency key is documented). See `errors/adopets-problem-types.yml`.
- Amounts are decimal numbers in the request's `currency`.
