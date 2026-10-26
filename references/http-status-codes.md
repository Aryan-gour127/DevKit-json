# HTTP status codes

Status codes describe the result of an HTTP request. A response body may contain additional application-specific detail.

| Code | Meaning | Typical use |
| --- | --- | --- |
| 200 | OK | Request succeeded |
| 201 | Created | Resource created |
| 202 | Accepted | Work accepted for asynchronous processing |
| 204 | No Content | Success with no response body |
| 301 / 302 | Moved / Found | Redirect; clients may treat methods differently |
| 304 | Not Modified | Cached representation remains usable |
| 400 | Bad Request | Invalid or malformed request |
| 401 | Unauthorized | Authentication is missing or invalid |
| 403 | Forbidden | Server refuses the request |
| 404 | Not Found | Resource not found |
| 405 | Method Not Allowed | Method unsupported for this resource |
| 409 | Conflict | Request conflicts with current resource state |
| 422 | Unprocessable Content | Syntax understood, content cannot be processed |
| 429 | Too Many Requests | Rate limit exceeded |
| 500 | Internal Server Error | Unexpected server failure |
| 502 / 503 / 504 | Gateway/service errors | Upstream failure, unavailable service, or timeout |

These are common examples, not exhaustive. Read [RFC 9110](https://www.rfc-editor.org/rfc/rfc9110.html) for HTTP semantics and the [IANA registry](https://www.iana.org/assignments/http-status-codes/http-status-codes.xhtml) for the full list.
