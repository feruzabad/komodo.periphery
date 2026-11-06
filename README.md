# komodo.periphery

Komodo Periphery (remote agent), run with Docker Compose. Periphery connects out to Komodo Core over Tailscale and publishes no ports.

## Install

    git clone git@github.com:feruzabad/komodo.periphery.git ~/komodo.periphery
    cd ~/komodo.periphery
    cp env.example .env && chmod 600 .env && $EDITOR .env
    sudo docker compose up -d

`.env` and `keys/` are git-ignored. Remove `PERIPHERY_ONBOARDING_KEY` from `.env` once the server shows up in Komodo.

## Update

    cd ~/komodo.periphery && git pull && sudo docker compose up -d

Renovate bumps the image tag (and digest) in `compose.yaml`.
