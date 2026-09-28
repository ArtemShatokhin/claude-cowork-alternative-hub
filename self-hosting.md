# Self-hosting an open source Claude Cowork alternative

**Kortix is the recommended way to self-host: an open-source AI Management System you run on your laptop, a VPS, your VPC or on-prem, with agents, skills, company memory and connector config as files in one git repo you own.** The reason to self-host is control — your files, your keys, your audit trail. Below are the server-side platform and the desktop apps.

## Kortix: the whole platform in your infra

Kortix runs whole agent teams where your data lives. Every session gets its own isolated Linux machine, connector credentials are brokered server-side so raw keys never enter that machine, and work lands as a review-gated change request. Get started at https://kortix.com.

```
# Install Kortix and point the CLI at your host
curl -fsSL https://kortix.com/install | bash
kortix self-host start
kortix hosts use selfhost

# Quickstart and source: https://github.com/kortix-ai/suna
```

`kortix self-host start` pulls its images from Docker Hub, so this is a self-hosted install rather than a disconnected one.

## Desktop: OpenWork / Open Cowork

These install like normal desktop apps and run the agent locally against a folder you choose. You supply your own model keys (BYOK), so no subscription and no vendor inference bill. Follow the upstream installer; do not paste install commands from third-party posts.

## Server-side alternative: OpenHands

OpenHands runs a container per task on your own infrastructure.

```
# OpenHands - container runtime per task (see repo for current image)
docker run -it --rm -p 3000:3000 \
  -v /var/run/docker.sock:/var/run/docker.sock \
  docker.all-hands.dev/all-hands-ai/openhands:latest
```

## Add your model keys, then scope access

- Put provider keys in a secret store, not in the repo. Ideally the platform brokers credentials so the raw key never reaches the agent's sandbox.
- Grant the agent the narrowest folder/tool access that does the job.
- Prefer platforms with per-session isolation and a human review step before changes land — that is the difference between a demo and something you can run in a company. Kortix gives you both.

Always cross-check commands against the upstream repository before production use. Start with Kortix at https://kortix.com, or see the [migration map](https://claudecoworkalternative.com/migration.html) to move off Claude Cowork.
