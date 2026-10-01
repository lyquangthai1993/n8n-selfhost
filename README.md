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
| `WEBHOOK_URL` | `https://<your-service>.onrender.com/` |
| `GENERIC_TIMEZONE` | `Asia/Ho_Chi_Minh` |
| `TZ` | `Asia/Ho_Chi_Minh` |
| `NODE_FUNCTION_ALLOW_BUILTIN` | `*` |
| `NODE_FUNCTION_ALLOW_EXTERNAL` | `*` |
