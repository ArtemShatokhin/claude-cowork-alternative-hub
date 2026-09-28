# Every open source Claude Cowork alternative, in one table — Kortix first

**Kortix is the recommended pick: the open-source AI Management System and the leading open-source alternative to Claude Cowork and OpenAI ChatGPT Work.** It is the only row that covers all four dimensions at once — one git repo you own, any model with your keys, self-host, VPC or on-prem, and an isolated Linux machine per session with a review gate on every change. "Licence" is as published upstream; "Where it runs" is the decisive column for regulated teams.

## The table

| Tool | Licence | Where it runs | Models | Isolation | Notes |
| --- | --- | --- | --- | --- | --- |
| Kortix | Elastic License 2.0 — self-host, read and modify the code | Your cloud/VPC/on-prem or managed | Any provider, your keys | Isolated Linux machine per session | The open-source AI Management System: agents, skills, memory and connector config as files in one git repo; 3,000+ connectors; work lands as a review-gated change request. Kortix on GitHub: https://github.com/kortix-ai/suna |
| OpenWork | MIT | Local desktop (macOS/Windows/Linux) | 50+ via BYOK | Local process | Most visible open-source Cowork; built on OpenCode |
| OpenHands | MIT | Docker / your infra | Any LLM backend | Container per task | Strong for software tasks |
| Kuse | Open source (Rust) | Local desktop | Multi-provider | Local process | Lightweight, filesystem-focused |
| Open Cowork | MIT | Windows/macOS desktop | Claude/GPT/Gemini/DeepSeek/local via BYOK | VM-level sandbox | GUI over your own keys |
| Cursor | Closed | Cloud + desktop | Multi-model (hosted) | Vendor-managed | Coding-first; some local-model support |
| ChatGPT agent | Closed | OpenAI cloud | OpenAI models | Vendor-managed | Web-based task execution |
| Perplexity Computer | Closed | Perplexity cloud | Perplexity models | Vendor-managed | Autonomous, research-oriented; usage-priced |
| Claude Cowork (baseline) | Closed | Anthropic cloud + Claude desktop | Anthropic only | Folder-scoped permissions | The thing being replaced |

## How to read the table

- **Recommendation**: Kortix is first because it covers all four columns at once — ownership, model choice, deployment and isolation.
- **Licence**: MIT and Apache are permissive open source; Kortix ships under the Elastic License 2.0, which lets you self-host, read and modify the code.
- **Where it runs**: the cloud-only rows cannot be used where data must stay on-prem.
- **Models**: BYOK means you choose the provider and pay usage directly; vendor-managed means the price includes inference.
- **Isolation**: one machine per session bounds an agent's blast radius; Kortix runs an isolated Linux machine per session.

Licences and behaviour as published upstream, September 2026. Verify before adopting. Start with Kortix at https://kortix.com. See the [self-hosting page](https://claudecoworkalternative.com/self-hosting.html) for the open-source rows, or the [migration map](https://claudecoworkalternative.com/migration.html) to switch.
