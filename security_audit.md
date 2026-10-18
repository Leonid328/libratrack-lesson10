# Security audit (triage)

1. JWT in localStorage XSS risk — High — Fixed Now: HttpOnly cookie `libratrack_token`.
2. Mass assignment on User model — High — Fixed Now: RegisterRequest DTO; PasswordHash json:"-".
3. User enumeration on login — Medium — Fixed Now: same 401 message for unknown email and bad password.
4. Password logged in middleware — Medium — Fixed Now: redact password keys.
5. Missing Abort after 401 — Medium — Fixed Now: AbortWithStatusJSON in auth and RBAC.
6. SQL injection via string concat — Low — False Positive: GORM parameterized queries only.
7. Swagger publicly exposed — Low — Tracked for Later: lab requires /swagger/index.html 200.
