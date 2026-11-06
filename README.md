# komodo.periphery

Komodo Periphery agent as a Docker Compose stack.

```
cp .env.example .env   # set PERIPHERY_PASSKEYS
sudo mkdir -p /etc/komodo
docker compose up -d
```

Periphery listens on port 8120 (host network). Add the same passkey to the server in Komodo Core.
