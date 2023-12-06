# Example curl commands for testing your server

Run these commands from your host machine, not your server.

## Testing your frontend

```bash
curl http://24.199.71.168
```

## Testing your backend

```bash
curl http://24.199.71.168/hey
```

```bash
curl -X POST -H "Content-Type: application/json" \
  -d '{"message": "Hello from your server"}' \
  http://24.199.71.168/echo
```
