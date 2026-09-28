TITLE: Open Source Kortix Install: Quickstart in Three Commands
META: Install open-source Kortix in three commands: the CLI, a project, your first session. Self-host it or use managed cloud. Kortix is open source.

# Install open-source Kortix in three commands

Kortix is the open-source AI Management System, installed in three commands. It puts your agents, skills, company memory and connector config in one git repo you own, runs every session on its own isolated Linux machine, and lands work as a change request a human reads as a diff. This is the quickstart: install the CLI, scaffold a project, start a session.

## Install in three commands

1. Install the CLI, at the shell.

   ```bash
   curl -fsSL https://kortix.com/install | bash
   ```

   This downloads the prebuilt `kortix` binary for your OS and architecture and puts it on your PATH.

2. Scaffold a project.

   ```bash
   kortix init
   ```

   This creates `kortix.yaml` plus the agents, skills and runtime configuration for the project.

3. Bring it live.

   ```bash
   kortix ship
   ```

   This pushes the repo and brings the project live.

## Start your first session

Sessions run an agent on your project in an isolated sandbox on its own branch. Give it a prompt, then review what it proposes.

```bash
kortix sessions new --prompt "Summarize this week's commits and open a change request"
kortix cr ls
kortix chat
```

`kortix cr ls` lists the change requests your agents opened so you can review each one as a diff. `kortix chat` attaches you to a live session to steer it.

## Self-host instead

Self-host the same platform on your laptop, a VPS, your VPC or on-prem. The images pull from Docker Hub, so this is a self-hosted install rather than a disconnected one.

```bash
kortix self-host start
kortix hosts use selfhost
kortix hosts use cloud
```

`kortix self-host start` launches the stack and `kortix hosts use selfhost` points the CLI at it. Switch back to managed cloud with `kortix hosts use cloud`.

## Requirements

- A git repo project, created by `kortix init`.
- Model keys, or a ChatGPT subscription.
- Nothing to install for the managed cloud path: sign up at kortix.com and start a session.

> **Note:** work reaches main only through a change request you approve.

Get started with open-source Kortix at [kortix.com](https://kortix.com). Read the docs at [kortix.com/docs](https://kortix.com/docs) and the code at [Kortix on GitHub](https://github.com/kortix-ai/suna).
