# Postgres MCP Demo

```bash
export MODEL=granite3.3:2b
docker compose up --build
```

```bash
curl http://localhost:11434/api/generate \
  -H "Content-Type: application/json" \
  -d '{
    "model": "granite3.3:2b",
    "prompt": "How are you today?",
    "stream": false
  }' | jq
```
