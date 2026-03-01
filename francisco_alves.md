# https://papichickens.github.io/data.ttl

## `curl -I https://papichickens.github.io/data.ttl` output:

```http
HTTP/2 200 
server: GitHub.com
content-type: text/turtle; charset=utf-8
last-modified: Sun, 01 Mar 2026 13:17:56 GMT
access-control-allow-origin: *
strict-transport-security: max-age=31556952
etag: "69a43c84-727"
expires: Sun, 01 Mar 2026 13:30:07 GMT
cache-control: max-age=600
x-proxy-cache: MISS
x-github-request-id: 54D8:37E47F:7AAB6B:7BE73E:69A43D07
accept-ranges: bytes
age: 0
date: Sun, 01 Mar 2026 13:20:08 GMT
via: 1.1 varnish
x-served-by: cache-bru1480036-BRU
x-cache: MISS
x-cache-hits: 0
x-timer: S1772371208.904217,VS0,VE119
vary: Accept-Encoding
x-fastly-request-id: 80ca5d2c6a57299b73c6f60b5201759b6435cae9
content-length: 1831
```

## Comments
- Content-type: text/turtle
- CORS: access-control-allow-origin: * enables cross-origin access from any website.
- HTTPs: includes strict-transport-security: max-age=31556952, meaning browsers will enforce HTTPS for this domain for about 1 year.
- Caching is enabled via cache-control: max-age=600 (10 minutes) and an expires timestamp.
- Compression currently isn't supported, likely due to the fact that, for Github, compressions only happen above a certain threshold of size (currently just 1831B)
