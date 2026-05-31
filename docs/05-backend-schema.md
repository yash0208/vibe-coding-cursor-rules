# Document 05 — Backend Schema (Data Model & Auth)

> Define tables and security before writing migrations.

## Tables

### Table: users

| Column | Type | Notes |
|--------|------|-------|
| id | uuid | PK |
| email | text | |
| name | text | |
| created_at | timestamp | |
| role | text | |

### Table: [your_table]

| Column | Type | Notes |
|--------|------|-------|
| id | uuid | PK |
| user_id | uuid | FK → users.id |
| created_at | timestamp | |

## Architecture

| Field | Your answer |
|-------|-------------|
| **Relationships** | e.g. projects.user_id → users.id (many-to-one) |
| **Auth Provider** | e.g. Supabase Auth — JWT, email/OAuth |
| **Row Level Security** | e.g. Users can only read/write their own rows |
| **User Roles** | e.g. admin: full access, user: own data only |
| **File Storage** | e.g. Supabase Storage — `/avatars/{user_id}` |
| **Sensitive Fields** | e.g. payment_method — stored via Stripe, not in DB |
