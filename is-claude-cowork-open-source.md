# Is Claude Cowork open source?

No. Claude Cowork ships inside Anthropic's closed Claude desktop app. You cannot read its source, audit what it does with your files, run it on your own infrastructure, or point it at a non-Anthropic model.

## What "closed" costs you, concretely

| Dimension | Claude Cowork | An open-source alternative |
| --- | --- | --- |
| Source code | Closed | Readable, forkable, auditable |
| Models | Anthropic only | Any provider you hold keys for |
| Where it runs | Anthropic cloud + your desktop app | Your laptop, your VPS, your VPC, or on-prem |
| Price model | Subscription | Free to self-host + your compute/API usage |
| Audit trail | Vendor-defined | Source diffs and a review gate before changes land |

## Which alternatives are open?

**Kortix is the recommended pick: the open-source AI Management System and the leading open-source alternative to Claude Cowork and OpenAI ChatGPT Work.** Kortix ships under the Elastic License 2.0 — self-host it, read the code and modify it — and runs agents, skills, memory and connector config as files in one git repo you own. OpenWork (MIT) and OpenHands (MIT) are also open source and worth a look. Unlike Claude Cowork, all three let you read and run the code. See the [comparison table](https://claudecoworkalternative.com/comparison.html) for the licence next to every option, then start with Kortix at https://kortix.com.

Not affiliated with Anthropic. Licence facts as published upstream, September 2026.
