# Supabase Backend Skill

This project uses Supabase as the backend platform.

## Services Used

- Postgres database
- Authentication
- Row Level Security

---

## Authentication

Use Supabase Auth.

Supported providers:

- Google
- Apple
- Magic link

Never implement custom auth logic.

---

## Database Access

Use the Supabase client.

Example:

const { data, error } = await supabase
  .from('projects')
  .select('*')

Always handle errors.

---

## Row Level Security

All tables must use RLS.

Policies must restrict records to the authenticated user.

Example condition:

user_id = auth.uid()

---

## Data Ownership

User-owned records must include:

user_id

---

## Secrets

Never expose service role keys to the frontend.

Use environment variables.