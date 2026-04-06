# Modelos e campos (orientação)

Repo sem ORM. Convenções para alinhar implementações:

- `tenant_id` / `org_slug` — identificador estável de empresa
- `portal_user_id` — utilizador portal (Odoo) quando aplicável
- Header `Idempotency-Key` — idempotência de escrita
- Header `X-Request-Id` — correlação em todas as respostas JSON
