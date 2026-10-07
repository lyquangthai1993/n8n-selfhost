# n8n Self-hosted on Render

Deploy n8n lên Render bằng Docker image chính thức.

## Cấu hình

- **Image**: `docker.n8n.io/n8nio/n8n:latest`
- **Port**: 5678
- **Region**: Singapore

## Environment Variables cần set trên Render

| Key | Value |
|-----|-------|
| `N8N_PORT` | `5678` |
| `N8N_PROTOCOL` | `https` |
| `N8N_HOST` | `<your-service>.onrender.com` |
| `N8N_WEBHOOK_URL` | `https://<your-service>.onrender.com/` |
| `N8N_ENCRYPTION_KEY` | `<master-encryption-key-hex>` |
| `N8N_PROXY_HOPS` | `1` |
| `GENERIC_TIMEZONE` | `Asia/Ho_Chi_Minh` |
| `TZ` | `Asia/Ho_Chi_Minh` |
| `NODE_FUNCTION_ALLOW_BUILTIN` | `*` |
| `NODE_FUNCTION_ALLOW_EXTERNAL` | `*` |
| `EXECUTIONS_DATA_PRUNE` | `true` |
| `EXECUTIONS_DATA_MAX_AGE` | `168` |
| `N8N_METRICS` | `false` |
| `DB_POSTGRESDB_HOST` | `<neon-pooler-host>` |
| `DB_POSTGRESDB_PORT` | `5432` |
| `DB_POSTGRESDB_DATABASE` | `neondb` |
| `DB_POSTGRESDB_USER` | `neondb_owner` |
| `DB_POSTGRESDB_PASSWORD` | `<neon-password>` |
| `DB_POSTGRESDB_SSL_REJECT_UNAUTHORIZED` | `false` |

