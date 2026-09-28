TITLE: Open Source Claude Cowork Migration and Switch Guide
META: Kortix is the open source alternative to Claude Cowork. Map every Cowork feature to Kortix and follow the six-step switch checklist.

# Migrate from Claude Cowork to open source Kortix

Kortix is the open-source alternative to Claude Cowork, and it keeps the work Cowork does while handing you the whole system as files you own. If you already run Cowork, this page maps every part of it to Kortix and gives you a six-step switch.

Kortix is open source (Elastic License 2.0) — self-host, read and modify the code.

## What maps to what

Every piece of Claude Cowork has a direct equivalent in Kortix. The difference is ownership: the desktop app becomes a system you start from anywhere, and the folder you grant becomes one git repo the company owns.

| In Claude Cowork | In Kortix |
| --- | --- |
| Desktop app on your machine | Web, CLI, Slack, email, mobile and API — start the same session from any of them |
| A folder you grant | The whole company in one git repo you own — agents, skills, memory and connector config |
| Anthropic models only | Any model, your keys — Claude, OpenAI, Gemini or your own OpenAI-compatible endpoint, per agent, per session, per message |
| Anthropic's cloud only | Self-host on your laptop, a VPS, your VPC or on-prem — or managed cloud |
| A paid subscription | Open source: self-host free; managed cloud $40/seat/mo + usage |
| No source to read | Elastic License 2.0 — read, fork and audit the code |
| Vendor-managed permissions | Per-resource permissions and allow / ask / block per tool call |
| Work happens in the app | Every session gets its own isolated Linux machine; work lands as a change request a human reads as a diff |

## Six steps to switch

1. Inventory what Cowork does today — folders, recurring jobs, connectors.
2. Bring the company up as one repo: `curl -fsSL https://kortix.com/install | bash` then `kortix init` (creates kortix.yaml plus your agents, skills and runtime config).
3. Add your model keys, or sign in with the ChatGPT subscription you already pay for; pick a model per agent.
4. Wire the connectors you used — 3,000+ apps, plus any MCP, OpenAPI, GraphQL or HTTP API; credentials are brokered server-side.
5. Move one job first. Run it beside Cowork and compare output.
6. Ship it: `kortix ship`, then let every change land as a change request you review as a diff.

## What you keep

You keep the files: the company is one git repo holding your agents, skills, memory, connector config and triggers. You keep your model keys, so Claude, OpenAI, Gemini or your own OpenAI-compatible endpoint stays your choice. You keep your infrastructure, whether that is your laptop, a VPS, your VPC or on-prem. And you keep an audit trail — every session runs on its own isolated Linux machine and nothing reaches main until a human approves the change request.

Get started with open-source Kortix at [kortix.com](https://kortix.com). Set up your own host with [self-hosting](/self-hosting.html), or follow the [installation guide](/install.html).
