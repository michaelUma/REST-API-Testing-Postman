# API Test Strategy

## Scope
Resource retrieval, single-resource lookup, unknown-resource behavior, request payload handling, HTTP methods, JSON schema expectations, and response-time observation.

## Request checklist
- Method and URL are correct.
- Headers include appropriate Accept and Content-Type values.
- Query parameters and path parameters are encoded correctly.
- Request body is valid JSON and uses expected field names and types.
- Authentication is supplied only when the target requires it.

## Response checklist
- Status code matches the contract.
- Content-Type is appropriate.
- JSON structure and required fields are present.
- Field types and values are valid.
- Error responses do not disclose secrets or stack traces.
- Response time is recorded against a stated threshold.

## Method expectations
GET retrieves; POST creates or triggers processing; PUT replaces; PATCH partially updates; DELETE removes or deactivates. Confirm the API contract because implementation semantics can differ.

## Authentication and authorization
For an owned/authorized API, test missing, malformed, expired, and valid tokens, plus access to resources owned by another test user. Never use another person's token or data.

## Execution
Import the collection, select the environment, run the collection, save the runner result, and record any environment or service instability. The demo API does not demonstrate real authentication.
