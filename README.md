# REST API Testing with Postman

An API testing portfolio covering HTTP methods, request/response validation, JSON assertions, negative cases, environment variables, and reusable Postman collections.

## Practice target
The collection uses JSONPlaceholder (https://jsonplaceholder.typicode.com), a public demo API. Its write endpoints return demonstration responses and do not guarantee persistent data changes.

## Skills demonstrated
- GET, POST, PUT, PATCH and DELETE
- Status code, header, response body and response-time checks
- JSON field and data-type validation
- Positive and negative test design
- Postman variables, collection runner and test scripts
- API test documentation and reporting

## Files
- `postman/REST-API-Testing.postman_collection.json` — importable starter collection
- `postman/Local.postman_environment.json` — demo base URL
- `docs/TEST-STRATEGY.md` — approach and checklist
- `test-cases/API-TEST-CASES.md` — API test matrix
- `reports/RUN-REPORT-TEMPLATE.md` — execution record

## Run
1. Install Postman.
2. Import the collection and environment.
3. Select the Local - Demo API environment.
4. Run the collection using Collection Runner.
5. Inspect assertion results and export the run report.
6. Record the date, environment, totals, and failures.

## Test checklist
| ID | Scenario | Expected |
|---|---|---|
| API-001 | GET /posts | 200 and JSON array |
| API-002 | GET /posts/1 | 200 with expected fields |
| API-003 | GET unknown post | 404 / documented not-found behavior |
| API-004 | POST valid JSON | 201 and created representation |
| API-005 | PUT existing resource | 200 and updated representation |
| API-006 | PATCH one property | 200 and changed property |
| API-007 | DELETE resource | Documented successful status |
| API-008 | Protected route without token | 401 on an authorized API |

## Security
Never commit real API keys, passwords, tokens, or private environment files. Authentication and authorization cases require a suitable API you own or have permission to test.

## Limitations
JSONPlaceholder is a learning service, not a production API. It does not demonstrate real authentication or durable CRUD persistence.

## Author
Michael Uma — API Testing Portfolio.
