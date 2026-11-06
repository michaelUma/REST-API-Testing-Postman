# API Test Cases

| ID | Method | Scenario | Expected |
|---|---|---|---|
| API-001 | GET /posts | Retrieve collection | 200 and JSON array |
| API-002 | GET /posts/1 | Retrieve existing post | 200 with ID, title, body, userId |
| API-003 | GET /posts/999999 | Unknown post | 404 or documented empty-resource behavior |
| API-004 | POST /posts | Valid JSON payload | 201 and created representation |
| API-005 | POST /posts | Missing required field | Documented validation response |
| API-006 | PUT /posts/1 | Replace resource | Successful response matches submitted representation |
| API-007 | PATCH /posts/1 | Update one field | Only intended field changes |
| API-008 | DELETE /posts/1 | Delete resource | Documented successful status |
| API-009 | Any protected endpoint | Missing token | 401 |
| API-010 | Any protected endpoint | Authenticated user lacks permission | 403 or safely concealed 404 |
| API-011 | Any endpoint | Unsupported method | 405 |
| API-012 | Any endpoint | Unsupported content type | 415 where applicable |

Cases API-009 through API-012 require a suitable API contract and authorized target; they are not simulated by the JSONPlaceholder collection.
