# HTTP methods and request basics

## Common methods

| Method | Typical intent | Notes |
| --- | --- | --- |
| `GET` | Retrieve a representation | Safe and idempotent by intended semantics |
| `HEAD` | Retrieve headers for a representation | Similar to `GET`, without response content |
| `POST` | Submit data or request processing | Not generally idempotent |
| `PUT` | Create or replace a resource at a known URI | Idempotent by intended semantics |
| `PATCH` | Apply a partial modification | Semantics depend on the patch format |
| `DELETE` | Remove a resource | Idempotent by intended semantics |
| `OPTIONS` | Discover communication options | Often used for CORS preflight |

Idempotence describes the intended effect of repeated requests, not whether every server implementation behaves correctly.

## Request and response

A request has a method, target URI, headers, and sometimes content. A response has a status code, headers, and sometimes content. `Content-Type` describes the representation; `Accept` indicates acceptable response types.

## Authentication basics

HTTP authentication may use mechanisms such as bearer tokens or cookies. Use HTTPS, protect credentials, follow the service's authorization rules, and avoid placing secrets in URLs or logs. Authentication establishes identity; authorization decides permitted actions.

Reference: [MDN HTTP overview](https://developer.mozilla.org/en-US/docs/Web/HTTP/Overview), [HTTP Semantics RFC 9110](https://www.rfc-editor.org/rfc/rfc9110.html).
