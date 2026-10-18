# LibraTrack — Lesson 10 (HTMX + go:embed)

Web catalog on the secured API.

- `GET /catalog` — HTML table, live search
- HTMX delete row (librarian/admin cookie or Bearer)
- Templates and CSS compiled with `go:embed`
- JWT in HttpOnly cookie (see `design_v10.txt`)

```bash
CGO_ENABLED=0 go build -o libratrack ./cmd/api
mkdir -p /tmp/verify_libratrack && cp libratrack /tmp/verify_libratrack/
```
