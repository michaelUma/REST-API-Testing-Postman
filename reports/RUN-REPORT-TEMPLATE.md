# Postman Run Report

> Complete this report only after executing the collection. Replace every placeholder with observed values. Use `Not run`, `Blocked`, or `Not applicable` where appropriate; do not estimate counts or describe expected results as actual results.

## 1. Run metadata

| Field | Value |
|---|---|
| Report ID | `[e.g. POSTMAN-YYYY-MM-DD-01]` |
| Run date and time (include timezone) | |
| Tester | |
| Collection name | REST API Testing - JSONPlaceholder |
| Collection version / Git commit | |
| Postman version | |
| Runner | Desktop / Web / Newman / Postman CLI |
| Environment name | |
| Target API | |
| Base URL | `[public URL only; remove credentials and sensitive query parameters]` |
| Application build / release | `Not applicable for public demo API` |
| Authentication state | `None for JSONPlaceholder; never record tokens or passwords` |

## 2. Execution summary

| Metric | Observed result |
|---|---:|
| Requests attempted | |
| Requests completed | |
| Requests blocked / not sent | |
| Assertions passed | |
| Assertions failed | |
| Requests with transport errors | |
| Total duration | |
| Overall result | Pass / Fail / Blocked / Not run |

**Result rule:** mark the run as Pass only when all in-scope requests and assertions completed successfully and no unresolved release-blocking issue remains. A network or third-party service failure should be recorded separately from an application defect until the cause is established.

## 3. Request-level results

| Test / request ID | Method and path | HTTP status | Response time | Assertions passed / failed | Result | Evidence |
|---|---|---:|---:|---:|---|---|
| API-001 | GET /posts | | | | | |
| API-002 | GET /posts/1 | | | | | |
| API-003 | GET /posts/999999 | | | | | |
| API-004 | POST /posts | | | | | |
| API-005 | PUT /posts/1 | | | | | |
| API-006 | PATCH /posts/1 | | | | | |
| API-007 | DELETE /posts/1 | | | | | |

Add rows for any additional requests. Record actual status codes and timings from the run; do not copy expected values into the actual-result columns.

## 4. Failed assertions and defects

| Defect ID | Request | Failed assertion | Expected result | Actual result | Severity | Reproduction / evidence link |
|---|---|---|---|---|---|---|
| | | | | | | |

For each confirmed defect, include:
- Preconditions and sanitized test data
- Exact reproduction steps
- Expected versus actual behaviour
- Relevant request method and path
- Sanitized response excerpt or screenshot
- Environment and time observed
- Whether the issue was reproduced on a second run

Do not paste API keys, bearer tokens, passwords, session cookies, personal data, or full unredacted headers into this report.

## 5. Environment and service observations

| Observation | Evidence | Classification |
|---|---|---|
| DNS / connection / timeout / TLS issue | | Environment / Service / Unknown |
| Rate limit or throttling | | Environment / Service / Unknown |
| Unexpected 5xx response | | Service / Application / Unknown |
| Test-data or setup issue | | Test setup / Unknown |
| Other | | |

Do not classify a third-party outage, DNS failure, rate limit, or local connectivity problem as an application defect without evidence.

## 6. Test data and cleanup

- Test data used:
- Synthetic accounts or records created:
- Cleanup performed:
- Cleanup result:
- Any residual data or state:

JSONPlaceholder is a public demo service. Its POST, PUT, PATCH, and DELETE responses are illustrative and do not guarantee persistent data changes. Do not infer durable CRUD behaviour from a successful demo response.

## 7. Limitations and risks

- Target/API limitations:
- Scenarios not covered:
- Authentication / authorization not tested:
- Browser, device, or network limitations:
- Known external dependencies:

## 8. Evidence and reproducibility

- Postman collection export:
- Runner result export:
- Sanitized screenshots:
- Newman / Postman CLI command (if used):
- Related issue or defect links:
- Git commit / branch:

Store evidence in the repository only after removing secrets, tokens, cookies, personal data, and confidential payloads.

## 9. Conclusion and next steps

**Conclusion:** `[Summarize only what the observed run supports.]`

**Recommended next steps:**
1. 
2. 
3. 

**Reviewer / review date:** 
