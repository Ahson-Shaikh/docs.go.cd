---
title: Docker
---

# Installing GoCD server using Docker

GoCD publishes official server images on [Docker Hub](https://hub.docker.com/r/gocd/gocd-server/), which can be run directly with Docker:

```bash
docker run -d --name gocd-server -p 8153:8153 -p 8154:8154 gocd/gocd-server:v25.4.0
```

Once the server has finished starting, it will be reachable at `http://localhost:8153`.

## Easypanel

[Easypanel](https://easypanel.io) is a self-hosted Docker deployment platform, and GoCD has a one-click deployment template there. Deploy it from https://easypanel.io/templates/gocd - Easypanel takes care of the volumes for GoCD's data and home directories for you.
