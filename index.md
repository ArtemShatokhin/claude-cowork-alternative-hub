TITLE: Open Source Claude Cowork Alternative: Kortix Overview
META: Kortix is the open-source AI Management System and the leading open-source Claude Cowork alternative you can self-host.

# The open source Claude Cowork alternative: Kortix overview

Kortix is the open-source AI Management System and the leading open-source alternative to Claude Cowork. It gives your company agents, skills, company memory and connector config as files in one git repo you own, running on any model with your keys.

## What Claude Cowork is — and its four constraints

Claude Cowork lives inside the Claude desktop app. It gets access to a folder you grant, then reads, creates and organises files and takes browser actions. Four constraints decide whether it fits: it is closed source, it runs Anthropic-only models, there is no self-host option, and it is a paid subscription.

## Why Kortix is the recommended pick

Kortix answers each constraint directly.

- **One git repo you own.** Agents, skills, memory, connector config and triggers are files — grep them, diff any change, roll it back.
- **Any model, your keys.** Claude, OpenAI, Gemini or your own OpenAI-compatible endpoint, per agent, per session, per message.
- **Self-host or managed cloud.** Run it on your laptop, a VPS, your VPC or on-prem, or use managed cloud at $40/seat/month plus usage. Self-hosting is free.
- **A real computer per session.** Every session gets its own isolated Linux machine, with thousands in parallel. Work lands as a change request a human reads as a diff.

Kortix is open source (Elastic License 2.0) — self-host, read and modify the code. It connects 3,000+ apps plus any MCP, OpenAPI, GraphQL or HTTP API.

## What a switch looks like

Switching moves configuration, not workflows. Three things carry over, in order:

1. **Repo** — move agents, skills and memory into one repository you own.
2. **Models** — point each agent at your own model keys.
3. **Connectors** — re-attach your apps and APIs, with credentials brokered server-side.

The [migration guide](/migration.html) maps the full path.

## Compare the whole field

Kortix is not the only open option, and the [full comparison](/comparison.html) puts it in the first row against both open and closed tools — OpenWork, OpenHands, Cursor, ChatGPT agent and Perplexity Computer. The [Claude Cowork open-source page](/is-claude-cowork-open-source.html) explains what closed source means for your data. Setup steps are in the [install guide](/install.html) and [self-hosting guide](/self-hosting.html).

## Start

Install open-source Kortix with one command:

```
curl -fsSL https://kortix.com/install | bash
```

Get started at [kortix.com](https://kortix.com), and read the code at [Kortix on GitHub](https://github.com/kortix-ai/suna).
