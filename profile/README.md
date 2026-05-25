<div align="center">

# genATP

### Building the unified web-access layer for AI agents.

*Generative Agent Test Protocol — one install, any agent, any LLM, 10× fewer tokens.*

[![License: Personal Use](https://img.shields.io/badge/license-Personal%20Use-orange.svg)](https://github.com/genatp/genatp/blob/main/LICENSE)
[![Status](https://img.shields.io/badge/status-pre--alpha-orange.svg)](https://github.com/genatp/genatp#roadmap)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-blue.svg)](https://github.com/genatp/genatp#contributing)

</div>

---

## Why we exist

Every AI agent that touches the web today is duct-taped together from six different vendors — a browser driver, a perception layer, a stealth proxy, a captcha solver, an auth manager, a benchmark harness — and burns ~2 million tokens to do what a human does in 30 seconds.

We think that's nuts.

**genATP is one install that replaces the whole stack** — and adds the two things nothing else has: deterministic, self-healing **Action Cassettes** that replay with zero LLM calls, and a declarative **ATP Spec** that doubles as test, automation, and production agent tool.

The web speaks human. Agents speak structured data. We're the translator everybody else forgot to build.

---

## What we're building

<table>
<tr>
<td width="60%" valign="top">

### [`genatp/genatp`](https://github.com/genatp/genatp) — the flagship

A single binary that gives any AI agent fast, cheap, reliable web access:

- 🎞️ **Action Cassettes** — record-once, replay-forever workflows (0 LLM tokens, self-heal on drift)
- 📜 **ATP Spec** — declarative YAML/JSON for tests, automations, and agent tools
- 🪙 **Token-optimized snapshots** — ~600 tokens/step vs ~50,000 raw
- 🔐 **Encrypted auth vault** — log in once, ever (OS keychain backed)
- 🧠 **DOM ↔ vision auto-switch** — never wastes tokens, never misses canvas pages
- 🥷 **Stealth by default** — good enough out of the box for ~80% of common defenses
- 🔌 **MCP server, Python SDK, TypeScript SDK, CLI** — all in one binary

</td>
<td width="40%" valign="top">

**Real numbers**

| Task (20 steps) | Tokens |
|---|---:|
| Playwright MCP | 2.28M |
| browser-use | 1.40M |
| **genATP — first run** | **34k** |
| **genATP — cassette replay** | **0** ✨ |

Self-hosted. Source-available. Written in Rust.

</td>
</tr>
</table>

---

## What we believe

1. **A web-access tool that needs six vendors is broken.** It should be one install.
2. **Tokens are a real cost.** Every snapshot, every prompt, every retry — measured, compressed, justified.
3. **Workflows shouldn't pay the LLM tax twice.** Record once, replay forever.
4. **Determinism is a feature.** Agents that drift silently are worse than agents that fail loudly.
5. **The same spec should run as a test, an automation, and an agent tool.** Three formats for one workflow is two too many.
6. **Source-available beats closed-source for trust, and trust beats marketing.**

---

## Getting started

```bash
# Pick your flavor
pip install genatp        # Python
npm install genatp        # TypeScript / Node
brew install genatp       # CLI on macOS

genatp init               # one-time setup
```

Then point your agent — Claude Desktop, Cursor, LangChain, your own — at the MCP server, SDK, or HTTP endpoint. Full quickstart in the [project README](https://github.com/genatp/genatp).

---

## Roadmap highlights

| Tag | Milestone |
|---|---|
| **v0.1** | MCP server + token-optimized snapshots — first public release |
| v0.3 | Encrypted Auth Vault |
| **v0.5** | Action Cassettes (record + replay + self-heal) + ATP Spec |
| v0.6 | TypeScript SDK |
| v0.7 | Stealth engine + DOM ↔ vision auto-switch |
| v0.8 | Cassette Registry + time-travel debugger |
| **v1.0** | GA — full WebVoyager benchmark (≥ 85% / ≤ 35k tokens) |

Full phased plan: [`docs/DEVELOPMENT_PLAN.md`](https://github.com/genatp/genatp/blob/main/docs/DEVELOPMENT_PLAN.md).

---

## Get involved

- ⭐ **Star [genatp/genatp](https://github.com/genatp/genatp)** — it genuinely helps
- 📖 **Read the [PRD](https://github.com/genatp/genatp/blob/main/docs/PRD.md)** before opening an issue — most "feature ideas" are already answered
- 🐛 **File an issue** with a failing repro for bugs, with a use case for proposals
- 🤝 **Open a PR** — see [`CONTRIBUTING.md`](https://github.com/genatp/genatp/blob/main/CONTRIBUTING.md)
- 🔐 **Report a security issue** privately — see [`SECURITY.md`](https://github.com/genatp/genatp/blob/main/SECURITY.md)


---

<div align="center">

**The web speaks human. Agents speak structured data.**
**genATP is the translator everybody else forgot to build.**

[Flagship repo](https://github.com/genatp/genatp) · [Docs](https://github.com/genatp/genatp/tree/main/docs) · [Roadmap](https://github.com/genatp/genatp#roadmap)

</div>
