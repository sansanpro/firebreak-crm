# Firebreak CRM

Funnel-audit lead pipeline. Static page, no build step, backed by Supabase (Postgres + Auth + PostgREST).

- `index.html` — the whole app. Plain `fetch`, no framework, no dependencies.
- Data lives in Supabase. Every table has RLS pinned to a single user id, so the
  anon key in this file returns `[]` on its own — verified before deploy.
- Schema and migrations: `projects/firebreak/ops-stack/schema_supabase.sql` in the vault.

Deployed via GitHub Pages.
